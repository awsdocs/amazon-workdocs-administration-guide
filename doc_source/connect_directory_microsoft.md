# Getting Started with AWS Managed Microsoft AD<a name="connect_directory_microsoft"></a>

In this tutorial, you'll learn how to set up an Amazon WorkDocs site by connecting to your on\-premises AWS Managed Microsoft AD directory\.

**Note**  
If you are part of a compliance program, such as PCI, FedRAMP, or DoD, you must set up a AWS Managed Microsoft AD Directory to meet compliance requirements\.

**Topics**
+ [Before You Begin](#microsoft-dir-prereqs)
+ [Step 1: Launch the Amazon WorkDocs Site](#microsoft-dir-site)
+ [Step 2: Enable AWS Managed Microsoft AD and Set Administrator](#microsoft-dir-enable)
+ [Step 3: Complete Admin Control Panel Setup](#microsoft-dir-admin-panel)

## Before You Begin<a name="microsoft-dir-prereqs"></a>
+ You must create an AWS Managed Microsoft AD\. For more information, see [How to Create a Microsoft AD directory](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/create_managed_ad.html)\.
+ You must create a Trust Relationship between your AD directory and the AWS Managed Microsoft AD\. For more information, see [When to Create a Trust Relationship](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/setup_trust.html)\.
+ When you launch a new Amazon WorkDocs site, you must specify profile information for the administrator, including first and last name and an email address\. 

## Step 1: Launch the Amazon WorkDocs Site<a name="microsoft-dir-site"></a>

Follow the steps below to launch your Amazon WorkDocs site\.

**To launch the Amazon WorkDocs site**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

   If you have never created or connected a directory in the selected region, you see the Amazon WorkDocs start page\. After you create a directory in a particular region, the start page is no longer available and you see the **Manage Your WorkDocs Sites** page instead\.

1. Choose **Get Started Now** from the Amazon WorkDocs start page or choose **Create a New WorkDocs Site** from the **Manage Your WorkDocs Sites** page\.

1. On the **Get Started with WorkDocs** page, next to **Standard Setup**, choose **Launch**\.

## Step 2: Enable AWS Managed Microsoft AD and Set Administrator<a name="microsoft-dir-enable"></a>

Follow the steps below to enable your AWS Managed Microsoft AD and set an administrator\.

**To enable your AWS Managed Microsoft AD**

1. From the list of available directories, select the AWS Managed Microsoft AD to use for your Amazon WorkDocs site\.
**Note**  
Make sure that site is being created in the same region as the AWS Managed Microsoft AD\. 

1. Choose **Enable directory**\.

1. On the **Set WorkDocs Administrator** page, enter a username from the AWS Managed Microsoft AD directory to be your Amazon WorkDocs administrator and choose **Select Administrator**\. 

   It takes several minutes for the directory to be connected and the Amazon WorkDocs site to be created\. When the directory has been successfully connected, the **Status** value of the site changes to `Active`\.

## Step 3: Complete Admin Control Panel Setup<a name="microsoft-dir-admin-panel"></a>

After you receive the administrator registration email, connect to the Amazon WorkDocs site using the client of your choice and complete setup from your admin control panel\.

**To complete admin control panel setup**

1. In the administrator registration email, use the link to sign in to Amazon WorkDocs\.

1. Under **My account**, choose **Open admin control panel**\.

1. Change settings for preferred language, storage, security, and recovery bin\. For more information, see [Managing Site Settings](manage-sites.md)\.

1. Under **Manage Users**, invite new users\. You can also edit user settings\. 

For more information, see [Inviting and Managing Amazon WorkDocs Users](users.md)\.