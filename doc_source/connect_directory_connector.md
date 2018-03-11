# Connecting to Your On\-Premises Directory with AWS Directory Service AD Connector<a name="connect_directory_connector"></a>

You can use an AWS Directory Service AD Connector directory to connect to your on\-premises directory\. To use AD Connector to connect to your on\-premises directory, you must meet the prerequisites identified in [AD Connector Prerequisites](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/connect_prereq.html) in the *AWS Directory Service Administration Guide*\.

**Note**  
If you use AD Connector with Amazon WorkDocs, you won’t be able to share file view links outside the company or invite external users to become contributors\.

To connect to your on\-premises directory, perform the following steps\.

**To connect to your on\-premises directory**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

   If you have never created or connected a directory in the selected region, you see the Amazon WorkDocs start page\. After you create a directory in a particular region, the start page is no longer available and you see the **Manage Your WorkDocs Sites** page instead\.

1. If you are on the Amazon WorkDocs start page, perform the following steps:

   1. Choose **Get Started Now**\.

   1. On the **Get Started with WorkDocs** page, choose **Launch** under **Standard Setup**\.

   If you are on the **Manage Your WorkDocs Sites** page, perform the following steps:

   1. Choose **Create a New WorkDocs Site**\.

   1. On the **Get Started with WorkDocs** page, choose **Launch** under **Standard Setup**\.

1. In the **Set up a Directory** page, choose **Create AD Connector**\.

1. Enter the following values and then choose **Continue**\.

   1. Enter the following values in the **Directory Details** section:  
**Directory DNS**  
The fully\-qualified name of the on\-premises directory, such as corp\.example\.com\. Amazon WorkDocs can only access user accounts in this directory\. User accounts cannot be contained in a parent directory, such as example\.com\.  
**NetBIOS Name**  
The NetBIOS name of the on\-premises directory, such as CORP\.  
**Account Username**  
The username of a user in the on\-premises directory\.   
**Account Password**  
The password for the on\-premises user account\.  
**Confirm Password**  
Re\-enter the password for the on\-premises user account\. This is required to prevent typing errors before the directory is connected\.  
**DNS Address**  
The IP address of a DNS server or domain controller in your on\-premises directory\. This server must be accessible from each subnet specified below\.

     Enter the following values in the **Access Point** section:  
**Region**  
Verify the region\.  
**Site URL**  
Enter the URL for your Amazon WorkDocs site\.

     Enter the following values in the **VPC Configuration** section:  
**VPC**  
The VPC that the directory is connected to\.  
**Subnets**  
The subnets in the VPC to use to connect to your on\-premises directory\. The two subnets must be in different Availability Zones\.

1. Review the directory information and make any necessary changes\. When the information is correct, click **Connect Directory**\.

   It takes several minutes for the directory to be connected and the Amazon WorkDocs site to be created\. When the directory has been successfully connected, the **Status** value of the site changes to `Active`\.