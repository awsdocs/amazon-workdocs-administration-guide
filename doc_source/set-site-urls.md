# Setting site URLs<a name="set-site-urls"></a>

**Note**  
If you followed the site creation process in [Getting started with Amazon WorkDocs](getting_started.md), you entered a site URL\. As a result, Amazon WorkDocs makes the **Set site URL** command unavailable, because you can only set a URL once\. You only follow these steps if you deploy Amazon WorkSpaces and integrate it with Amazon WorkDocs\. The Amazon WorkSpaces integration process has you enter a serial number instead of a site URL, so you have to enter a URL after you finish the integration\. For more information about integrating Amazon WorkSpaces and Amazon WorkDocs see [Integrate with WorkDocs](https://docs.aws.amazon.com/workspaces/latest/userguide/workspaces-user-getting-started.html#workdocs-integration) in the *Amazon WorkSpaces User Guide*\.

**To set a site URL**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the navigation pane, choose **My sites**\.

   The **Manage your WorkDocs sites** page appears and displays a list of your sites\. 

1. Select the site that you integrated with Amazon WorkSpaces\. The URL contains the directory ID of your Amazon WorkSpaces instance, such as **https://\{directory\_id\}\.awsapps\.com**\.

1. Choose the button next to that URL, open the **Actions** list, and choose **Set site URL**\.

   The **Set site URL** dialog box appears\.

1. In the **Site URL** box, enter the URL for the site, then choose **Set site URL**\.

1. On the **Manage your WorkDocs sites** page, choose **Refresh** to see the new URL\.