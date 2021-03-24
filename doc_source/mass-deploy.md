# Mass deploying Amazon WorkDocs Backup with Amazon WorkDocs Companion<a name="mass-deploy"></a>

You can deploy Amazon WorkDocs Backup as part of a mass deployment of Amazon WorkDocs Companion\. When you mass deploy Amazon WorkDocs Companion, you can download and run an installer that supports optional parameters, such as SITEID, that enable you to install Amazon WorkDocs Backup and configure it so that it starts without customer input\. When you run the installer, it generates a transform file that contains the desired parameters\.

## Generating the MSI and transform file<a name="generate-transform"></a>

Follow these steps to generate the MSI and transform file\.

1. Download the [Companion MSI Transform Tool\.](https://d1d0sl5loepvwt.cloudfront.net/windows/CompanionMsiTransformTool.zip)

1. Extract the \.zip file and follow the instructions in the Readme\.md file\.

1. Start PowerShell, navigate to the folder containing the extracted installer, then run the following command\. Remember to replace "my\-critical\-site," with the name of your site: **\.\\tools\\create\-companion\-msi\-and\-transform\-bundle\.ps1 \-SiteId "my\-critical\-site" \-Verbose** 

 Example output: 

```
.\output\2020-02-03 15.20.34.1581\AmazonWorkDocsCompanion.msi
.\output\2020-02-03 15.20.34.1581\AmazonWorkDocsCompanion.mst
.\output\2020-02-03 15.20.34.1581\AmazonWorkDocsCompanion-ParamsInfo.txt
```

The output includes:
+ The Amazon WorkDocs Companion MSI installer\.
+ The \.mst file that allows you to apply parameters to an installation when using deployment tools such as Group Policy\.
+ A text file containing the values of any parameters\. This is only informational\.

If you ran the command as shown in the example, the file AmazonWorkDocsCompanion\-ParamsInfo\.txt would contain `SITEID = 'my-critical-site'`\.

Next, you use Group Policy to deploy Amazon WorkDocs Companion and set the options for Amazon WorkDocs Backup\.

## Using Group Policy to deploy Amazon WorkDocs Companion<a name="use-group-policy"></a>

To start, place the MSI and the MST files on a network share that *everyone* in the organization can read\. You can place both files in the same folder\. For example:

```
 \\server-01\AmazonWorkDocsCompanion\AmazonWorkDocsCompanion.msi
 \\server-01\AmazonWorkDocsCompanion\AmazonWorkDocsCompanion.mst
```

You're now ready to create the Group Policy object\.

**Create the Group Policy object \(GPO\)**

1. Start the **Group Policy Management** widget\.

1. Expand your Forest, right\-click the top level domain or organizational unit, then select **Create a GPO in this domain, and link it here**\.

1. Enter a name for your GPO and choose **OK**\.

1. Right\-click the new GPO and choose **Edit**\.

1. Under **Computer Configuration**, expand **Software Settings**, choose **Software Installation**, right\-click **New**, then choose **Package**\.

   The network share that you created in the previous section appears\.

1. On that share, choose the \.msi file, choose **Advanced**, then choose **OK**\. This attaches the MSI transform file to the GPO\.

1. Choose the **Modifications** tab, then **Add**, choose the \.mst file from the network share, then choose **OK**\.

To ensure that your GPO doesn't require user input, add your web site to the Local Intranet security zone\. This stops the Windows login prompt\.

**Add your site to the safe zone**

1. Expand the **User Configuration** node, then the **Preferences** and **Windows Settings** nodes\.

1. Right\-click **Registry**, choose **New**, then choose **Registry Item**\.

1. Enter these values for the new registry key:

   ```
   Action: Update
   Hive: HKEY_CURRENT_USER
   Key Path: Software\Microsoft\Windows\CurrentVersion\Internet Settings\ZoneMap\Domains\awsapps.com\my-critical-site
   Value name: https
   Value type: REG_DWORD
   Value data: 00000001
   Base: Hexadecimal
   ```

1. Choose **OK**\.

 To add your site to the Local Intranet security zone on Windows servers, repeat these steps but use this key path:

```
Software\Microsoft\Windows\CurrentVersion\Internet Settings\ZoneMap\EscDomains\awsapps.com\my-critical-site
```

Notice that this key path uses EscDomains instead of Domains\.