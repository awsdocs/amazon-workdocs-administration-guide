# Creating a Simple AD Directory Using the Standard Setup<a name="cloud_standard_setup"></a>

To create a Simple AD directory, you must meet the prerequisites identified in [Simple AD Prerequisites](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/cloud_prereq.html) in the *AWS Directory Service Administration Guide*\.

To create an Amazon WorkDocs cloud directory using the standard setup, perform the following steps\.

**Note**  
If you are part of a compliance program, such as PCI, FedRAMP, or DoD, you must set up a Microsoft AD Directory to meet compliance requirements\.

**To create a cloud directory using the standard setup**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

   If you have never created or connected a directory in the selected region, you see the Amazon WorkDocs start page\. After you create a directory in a particular region, the start page is no longer available and you see the **Manage Your WorkDocs Sites** page instead\.

1. If you are on the Amazon WorkDocs start page, perform the following steps:

   1. Choose **Get Started Now**\.

   1. On the **Get Started with WorkDocs** page, choose **Launch** under **Standard Setup**\.

   If you are on the **Manage Your WorkDocs Sites** page, perform the following steps:

   1. Choose **Create a New WorkDocs Site**\.

   1. On the **Get Started with WorkDocs** page, choose **Launch** under **Standard Setup**\.

1. In the **Set up a Directory** page, choose **Create Simple AD**\.

1. Enter the following values and then choose **Continue**\.

   1. Enter the following values in the **Access Point** section:  
**Region**  
Verify the region\.  
**Site URL**  
Enter the URL for your Amazon WorkDocs site\.

   1. Enter the following values in the **Directory Details** section:  
**Directory DNS**  
The fully\-qualified name of the directory, such as `corp.example.com`\.  
**NetBIOS name**  
The NetBIOS name of the directory, such as `CORP`\.

   1. Enter the following values in the **Set WorkDocs Administrator** section:  
**Email**  
The email address of the directory administrator\. The registration email is sent to this email address\.  
**First Name**  
The first name of the directory administrator\.  
**Last Name**  
The last name of the directory administrator\.

   1. For **VPC Details**, you can either use an existing VPC, or have Amazon WorkDocs create and configure a VPC for you\. To have Amazon WorkDocs create the VPC for you, select **Set up a new VPC on my behalf**\. To use an existing VPC, select **Select an existing VPC to use with WorkDocs** and enter the following values\.  
**VPC**  
The VPC that the directory is created in\.  
**Subnets**  
The subnets in the VPC that the directory is created in\. The two subnets must be in different Availability Zones\. If you choose **No Preference**, two different subnets are randomly selected\.

1. Review the directory information and make any necessary changes\. When the information is correct, choose **Create Directory**\.

   It takes several minutes for the directory to be connected and the Amazon WorkDocs site to be created\. When the directory has been successfully connected, the **Status** value of the site changes to `Active`\.