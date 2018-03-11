# Amazon WorkDocs Console<a name="admin_console"></a>

The Amazon WorkDocs console is used to manage your Amazon WorkDocs directories and sites\. The following operations can be performed with the Amazon WorkDocs console:


+ [Create or Connect to a Directory](#manage_create_directory)
+ [Promote a User to Administrator](#manage_set_admin)
+ [Delete a Site](#manage_deactivate)
+ [Multi\-Factor Authentication](#connect_mfa)
+ [Single Sign\-On](#single_sign_on)

## Create or Connect to a Directory<a name="manage_create_directory"></a>

You use the Amazon WorkDocs console to create a cloud directory, or connect to your on\-premises directory\. For more information about creating a directory in the cloud, see [Creating a Simple AD Directory](create_directory.md)\. For more information about connecting to your on\-premises directory, see [Connecting to an On\-Premise Directory](connect_directory.md)\.

## Promote a User to Administrator<a name="manage_set_admin"></a>

Use the Amazon WorkDocs console to promote a user to administrator\. The user must be active to be promoted\. For more information about activating a user, see [Edit Users](admin_dashboard_cloud.md#edit_user_cloud)\.

**To promote a user to administrator**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the **Manage Your WorkDocs Sites** page, select the desired directory and choose **Actions** and **Set an Administrator**\.

1. In the **Set WorkDocs Administrator** page, enter the user name to promote and choose **Set Administrator**\.

You can also use the Amazon WorkDocs administration dashboard to demote an administrator\. For more information, see [Edit Users](admin_dashboard_cloud.md#edit_user_cloud)\.

## Delete a Site<a name="manage_deactivate"></a>

Use the Amazon WorkDocs console to delete an Amazon WorkDocs site\.

**Warning**  
Deleting a site causes the loss of all user information and all files\. Only delete a site if you are absolutely sure that this information is no longer needed\.

**To delete a site**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the **Manage Your WorkDocs Sites** page, select the desired site and choose **Actions** and **Delete WorkDocs Site**\.

1. In the **Delete Selected WorkDocs Site** dialog box, choose to also want delete the user directory\. This deletes the AWS Directory Service Simple AD or AD Connector directory that is used to store the Amazon WorkDocs user information\. To delete the directory, it cannot have any other AWS applications enabled\. For more information, see [Deleting a Simple AD Directory](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/cloud_delete.html) or [Deleting an AD Connector Directory](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/connect_delete.html) in the *AWS Directory Service Administration Guide*\.

1. Verify that you are deleting the proper site, enter **DELETE** in the confirmation field, and choose **Delete WorkDocs Site**\. 

   The site is immediately deleted and is no longer available\.

## Multi\-Factor Authentication<a name="connect_mfa"></a>

You can enable multi\-factor authentication for your AD Connector directory by performing the following procedure\. 

**Note**  
Multi\-factor authentication is not available for Simple AD directories\.

**To enable multi\-factor authentication**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the **Manage Your WorkDocs Sites** page, select the desired site and choose **Actions** and **Manage MFA**\.

1. Enter the following values and choose **Update MFA**\.   
**Enable Multi\-Factor Authentication**  
Check to enable multi\-factor authentication\.  
**RADIUS server IP address\(es\)**  
The IP addresses of your RADIUS server endpoints, or the IP address of your RADIUS server load balancer\. You can enter multiple IP addresses by separating them with a comma \(for example, **192\.0\.0\.0,192\.0\.0\.12**\)\.  
**Port**  
The port that your RADIUS server is using for communications\. Your on\-premises network must allow inbound traffic over the default RADIUS server port \(1812\) from the AD Connector servers\.  
**Shared secret code**  
The shared secret code that was specified when your RADIUS endpoints were created\.  
**Confirm shared secret code**  
Confirm the shared secret code for your RADIUS endpoints\.  
**Protocol**  
Select the protocol that was specified when your RADIUS endpoints were created\.  
**Server timeout**  
The amount of time, in seconds, to wait for the RADIUS server to respond\. This must be a value between 1 and 60\.  
**Max retries**  
The number of times that communication with the RADIUS server is attempted\. This must be a value between 0 and 10\.

   Multi\-factor authentication is available when the **RADIUS Status** changes to **Enabled**\. While multi\-factor authentication is being set up, your users are not able to log in to their Amazon WorkDocs site\.

## Single Sign\-On<a name="single_sign_on"></a>

AWS Directory Service allows users to access Amazon WorkDocs from a computer joined to the same directory with which Amazon WorkDocs is registered, without entering credentials separately\. For more information, see [Single Sign\-On](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/single_sign_on.html) in the *AWS Directory Service Administration Guide*\.

Your Amazon WorkDocs users may need to modify their web browser settings to enable single sign\-on\. For more information, see [Enabling Single Sign\-On](http://docs.aws.amazon.com/workdocs/latest/userguide/web_client_help.html#single_sign_on) in the *Amazon WorkDocs User Guide*\.