# Creating a Simple AD Directory<a name="create_directory"></a>

Amazon WorkDocs uses an AWS Directory Service Simple AD directory to store user information in the cloud\. You can create a Simple AD directory in one of two ways\. The [Quick Start procedure](cloud_quick_start.md) is used to get set up quickly and is designed for small organizations\. The Quick Start procedure creates and configures a VPC for use with the directory, and also creates the administrator account\. After you create a directory in a particular region, the Quick Start option is no longer available\.

When you create a Simple AD directory, Amazon WorkDocs performs the following tasks on your behalf:

+ Sets up a Simple AD directory within the VPC that is used to store user information\.

+ Creates a directory administrator account with the administrator email as the username\. An email is sent to the administrator with instructions to complete registration\. You use this account to manage your directory\.

If you need more control over the directory configuration, you can choose the [standard setup](cloud_standard_setup.md), which allows you to specify your own directory domain name, as well as one of your existing VPCs to use with the directory\. There is also an option to have Amazon WorkDocs create and configure a VPC for you\. 


+ [Creating a Simple AD Directory Using the Quick Start](cloud_quick_start.md)
+ [Creating a Simple AD Directory Using the Standard Setup](cloud_standard_setup.md)