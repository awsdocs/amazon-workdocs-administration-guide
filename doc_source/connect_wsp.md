# Enabling an Existing AWS Directory Service Directory<a name="connect_wsp"></a>

If you have an existing AWS Directory Service directory in the current region, you can connect Amazon WorkDocs to your existing directory\. This can be either a Simple AD directory or an AD Connector directory\. To connect to an existing AWS Directory Service directory, perform the following steps\.

**To connect to an existing directory**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. On the **Manage Your WorkDocs Sites** page, choose **Create a New WorkDocs Site**\.

1. On the **Select a Directory** page, select your AWS Directory Service directory from the **Available Directories** list and choose **Enable Directory**\.
**Note**  
If you are part of a compliance program, such as PCI, FedRAMP, or DoD, you must set up a Microsoft AD Directory to meet compliance requirements\.

1. On the **Set WorkDocs Administrator** page, enter a username from the AWS Directory Service directory to be your Amazon WorkDocs administrator and choose **Select Administrator**\.

   It takes several minutes for the directory to be connected and the Amazon WorkDocs site to be created\. When the directory has been successfully connected, the **Status** value of the site changes to `Active`\.