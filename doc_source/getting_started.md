# Getting started with Amazon WorkDocs<a name="getting_started"></a>

Amazon WorkDocs uses a directory to store and manage organization information for your users and their documents\. In turn, you attach a directory to a site when you provision that site\. When you do, an Amazon WorkDocs feature called Auto activation adds the users in the directory to the site as managed users, meaning they don't need separate credentials to log in to your site, they can share and collaborate on files, and they have 1 TB of storage\.

You no longer need to add and activate users manually, though you still can\. You can also change user roles and permissions whenever you need to\. For more information about doing that, see [Inviting and managing Amazon WorkDocs users](users.md), later in this guide\.

If you need to create directories, you can:
+ Create a Simple AD directory using Quick Start or Standard Setup\.
+ Create an AD Connector directory to connect to your on\-premises directory\.
+ Enable Amazon WorkDocs to work with an existing AWS directory\.
+ Have Amazon WorkDocs create a directory for you\.

You can also create a trust relationship between your AD directory and an AWS Managed Microsoft AD Directory\.

**Note**  
If you belong to a compliance program such as PCI, FedRAMP, or DoD, you must set up an AWS Managed Microsoft AD Directory to meet compliance requirements\.

**Topics**
+ [Getting started with Quick Start](cloud_quick_start.md)
+ [Getting started with Simple AD: Standard Setup](cloud_standard_setup.md)
+ [Getting started with an existing directory](existing-dir-setup.md)
+ [Getting started with AD Connector](connect_directory_connector.md)
+ [Getting started with AWS Managed Microsoft AD](connect_directory_microsoft.md)
+ [Enabling single sign\-on](single_sign_on.md)
+ [Enabling multi\-factor authentication](connect_mfa.md)
+ [Promoting a user to administrator](manage_set_admin.md)