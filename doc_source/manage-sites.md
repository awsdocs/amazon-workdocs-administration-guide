# Managing Sites<a name="manage-sites"></a>

Administrators can manage site\-wide operations, such as choosing a preferred language for site content and email notifications, setting storage limits, and specifying recovery bin retention policy\. They can also change settings for [Managing Security Settings](security-settings.md) and [Inviting and Managing Amazon WorkDocs Users](users.md)\.

**Topics**
+ [Language Settings](#language-settings)
+ [Storage Settings](#storage-limits)
+ [Security Settings](#manage-security-settings)
+ [Recovery Bin Retention Settings](#recovery-bin)
+ [Manage Users Settings](#manage-users-settings)
+ [Deleting a Site](#delete_site)

## Language Settings<a name="language-settings"></a>

Specify the language to use for site content and email notifications\.

**To change language settings**

1. Under **My Account**, choose **Open admin control panel**\.

1. For **Preferred Language Settings**, choose your preferred language\.

## Storage Settings<a name="storage-limits"></a>

Specify the amount of storage that new users receive\.

**To change storage settings**

1. Under **My Account**, choose **Open admin control panel**\.

1. For **Storage**, choose **Change**\.

1. In the **Storage Limit** dialog box, choose whether to give new users unlimited or limited storage\.

1. Choose **Save Changes**\.

Changing the storage setting affects only users that are added after the setting is changed\. It does not change the amount of storage allocated to existing users\. To change the storage limit for an existing user, see [Editing Users](edit_user.md)\.

## Security Settings<a name="manage-security-settings"></a>

You can manage security settings for users, including setting up external sharing and publicly shareable link options, and configuring default settings for user invites, new users, and enabled users\. For more information, see [Managing Security Settings](security-settings.md)\.

## Recovery Bin Retention Settings<a name="recovery-bin"></a>

Files deleted by a user are stored in the user’s recycle bin for 30 days\. Afterwards, the files are temporarily moved to a recovery bin for 60 days before they are permanently deleted\. The recovery bin is visible only to administrators\. By changing the site\-wide data retention policy, site administrators can change the recovery bin retention period, up to a maximum of 365 days\. Files are permanently deleted at the end of the retention period\.

**To change the recovery bin retention period**

1. Under **My Account**, choose **Open admin control panel**\.

1. Next to **Recovery bin retention**, choose **Change**\.

1. Enter the number of days to retain files in the recovery bin, and choose **Save**\.
**Note**  
The default retention period is 60 days\. This can be changed to 0–365 days\.

You can restore user files from the recovery bin before they are permanently deleted\.

**To restore a user's file**

1. Under **My Account**, choose **Open admin control panel**\.

1. Under **Manage Users**, choose the user's folder icon\.

1. Under **Recovery bin**, choose any of the user's files to restore\.

1. On the **Restore file** page, choose the location to restore the file, and choose **Restore**\.

## Manage Users Settings<a name="manage-users-settings"></a>

You can manage settings for users, including changing user roles and inviting, enabling, or disabling users\. For more information, see [Inviting and Managing Amazon WorkDocs Users](users.md)\.

## Deleting a Site<a name="delete_site"></a>

Use the Amazon WorkDocs console to delete an Amazon WorkDocs site\.

**Warning**  
Deleting a site causes the loss of all user information and all files\. Only delete a site if you are absolutely sure that this information is no longer needed\.

**To delete a site**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the **Manage Your WorkDocs Sites** page, select the desired site and choose **Actions** and **Delete WorkDocs Site**\.

1. In the **Delete Selected WorkDocs Site** dialog box, choose whether to delete the user directory at the same time\. This deletes the AWS Directory Service Simple AD or AD Connector directory that is used to store the Amazon WorkDocs user information\. To delete the directory, it cannot have any other AWS applications enabled\. For more information, see [Deleting a Simple AD Directory](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/simple_ad_delete.html) or [Deleting an AD Connector Directory](http://docs.aws.amazon.com/directoryservice/latest/admin-guide/ad_connector_delete.html) in the *AWS Directory Service Administration Guide*\.

1. Verify that you are deleting the proper site, enter **DELETE** in the confirmation field, and choose **Delete WorkDocs Site**\. 

   The site is immediately deleted and is no longer available\.