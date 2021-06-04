# Deploying Amazon WorkDocs Drive to multiple computers<a name="mass-deploy-drive"></a>

If you have a domain\-joined machine fleet, you can use Group Policy Objects \(GPO\) or System Center Configuration Manager \(SCCM\) to install the Amazon WorkDocs Drive client\. You can download the client from [ https://amazonworkdocs\.com/en/clients ](https://amazonworkdocs.com/en/clients)\.

As you go, remember that Amazon WorkDocs Drive requires HTTPS access on port 443 for all AWS IP addresses\. You'll also want to confirm that your target systems meet the installation requirements for Amazon WorkDocs Drive\. For more information, see [Installing Amazon WorkDocs Drive](https://docs.aws.amazon.com/workdocs/latest/userguide/drive_install.html) in the *Amazon WorkDocs User Guide*\.

**Note**  
As a best practice when using GPO or SCCM, install the Amazon WorkDocs Drive client after users log in\.

The MSI installer for Amazon WorkDocs Drive supports the following optional installation parameters:
+ **`SITEID`** – Pre\-populates the Amazon WorkDocs site information for users during registration\. For example, `SITEID=`*site\-name*\.
+ **`DefaultDriveLetter`** – Pre\-populates the drive letter to be used for mounting Amazon WorkDocs Drive\. For example, `DefaultDriveLetter=`*W*\. Remember, each user must have a different drive letter\. Also, users can change the drive name, but not the drive letter, after they start Amazon WorkDocs Drive for the first time\.

The following example deploys Amazon WorkDocs Drive with no user interfaces and no restarts\. Note that it uses the MSI file's default name:

`msiexec /i "AWSWorkDocsDriveClient.msi" SITEID=`*your\_workdocs\_site\_ID* `DefaultDriveLetter=`*your\_drive\_letter *`REBOOT=REALLYSUPPRESS /norestart /qn`