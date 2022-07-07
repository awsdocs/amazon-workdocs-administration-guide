# Creating an Amazon WorkDocs site<a name="cloud_quick_start"></a>

The steps in the following sections explain how to set up a new Amazon WorkDocs site\.

**Topics**
+ [Before you begin](#quick-setup-prereqs)
+ [Creating an Amazon WorkDocs site](#quick-setup-launch-site)

## Before you begin<a name="quick-setup-prereqs"></a>

You must have the following items before you create an Amazon WorkDocs site\.
+ An AWS account for creating and administering Amazon WorkDocs sites\. However, users do not need an AWS account to connect to and use Amazon WorkDocs\. For more information, see [Prerequisites for Amazon WorkDocs](prereqs.md)\.
+ If you plan to use Simple AD, you must meet the prerequisites identified in [Simple AD Prerequisites](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/prereq_simple.html) in the *AWS Directory Service Administration Guide*\.
+ An AWS Managed Microsoft AD Directory if you belong to a compliance program such as PCI, FedRAMP, or DoD\. The steps in this section explain how to use an existing Microsoft AD Directory\. For information about creating a Microsoft AD Directory, see [AWS Managed Microsoft AD](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/directory_microsoft_ad.html) in the *AWS Directory Service Administration Guide*\.
+ Profile information for the administrator, including first and last name, and an email address\. 

## Creating an Amazon WorkDocs site<a name="quick-setup-launch-site"></a>

Follow these steps to create an Amazon WorkDocs site in minutes\.

**To create the Amazon WorkDocs site**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. On the console's Home page, under **Create a WorkDocs site**, choose **Get Started now**\. 

   —OR—

   In the navigation pane, choose **My sites**, and on the **Manage your WorkDocs sites** page, choose **Create a WorkDocs site**\.

   What happens next depends on whether you have a directory\. 
   + If you have a directory, The **Select a directory** page appears and allows you to choose an existing directory or create a directory\.
   + If you don't have a directory, the **Set up a directory type** page appears and allows you to create a Simple AD or AD Connector directory

   The following steps explain how to do both tasks\. 

   

**To use an existing directory**

   1. Open the **Available directories** list and choose the directory that you want to use\.

   1. Choose **Enable directory**\.

   

**To create a directory**

   1. Repeat steps 1 and 2 above\.

      At this point, what you do depends on whether you want to use Simple AD or create an AD Connector\.

      

**To use Simple AD**

      1. Choose **Simple AD**, then choose **Next**\.

         The **Create Simple AD site page appears\.**

      1. Under **Access point**, in the **Site URL** box, enter the URL for the site\.

      1. Under **Set WorkDocs administrator**, enter the administrator's email address, first name, and last name\. 

      1. As needed, complete the options under **Directory details** and **VPC configuration**\.

      1. Choose **Create Simple AD site**\.

      

**To create an AD Connector directory**

      1. Choose **AD Connector**, then choose **Next**\.

         The **Create AD Connector site** page appears\.

      1. Complete all the fields under **Directory details**\.

      1. Under **Access point**, in the **Site URL** box, enter your site's URL\.

      1. As desired, complete the optional fields under **VPC configuration**\.

      1. Choose **Create AD Connector site**\.

Amazon WorkDocs does the following:
+ If you chose **Set up a VPC on my behalf** in step 4 above, Amazon WorkDocs creates a VPC for you\. A directory in the VPC stores user and Amazon WorkDocs site information\.
+ If you used Simple AD, Amazon WorkDocs creates a Directory User and sets that user as an Amazon WorkDocs administrator\. If you created an AD Connector directory, Amazon WorkDocs sets the exisitng directory user that you provided as a WorkDocs administrator\. 
+ If you used an existing directory, Amazon WorkDocs prompts you to enter the user name of the Amazon WorkDocs administrator\. The user must be a member of the directory\.

**Note**  
Amazon WorkDocs doesn't notify users about the new site\. You need to communicate the URL to them, and let them know that they don't need a separate login to use the site\. 