# Connecting to Your On\-Premises Directory with AWS Microsoft AD<a name="connect_directory_microsoft"></a>

You can also use AWS Microsoft AD to connect to your on\-premises Active Directory\.

**Note**  
If you are part of a compliance program, such as PCI, FedRAMP, or DoD, you must set up a Microsoft AD Directory to meet compliance requirements\.

To connect to your directory, perform the following steps\.

**To connect to your directory**

1. Create a Trust Relationship between your AWS Directory service and Microsoft AD\. For more information, see [When to Create a Trust Relationship](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/setup_trust.html)\.

1. Create a Microsoft AD\. For more information, see [How to Create a Microsoft AD directory](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/create_managed_ad.html)\.

1. If you want to set up your Microsoft AD to use Amazon WorkDocs with a new Amazon WorkDocs site, follow these steps:

   1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

   1. Choose **Create a new WorkDocs site**\.

   1. From the list of available directories, select the Microsoft AD you want to use for your Amazon WorkDocs site\.
**Note**  
Make sure that site is being created in the same region as the Microsoft AD\. 

   1. Choose **Enable directory**\.

   1. Enter the administrator's username that will be used to log into Amazon WorkDocs\. 