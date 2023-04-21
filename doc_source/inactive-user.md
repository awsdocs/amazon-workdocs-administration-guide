# Disabling users<a name="inactive-user"></a>

You disable a user's access by changing their status to **Inactive**\.

**To change user status to **Inactive****

1. Choose the profile icon in the upper\-right corner of the WorkDocs client\.

   ![\[The default profile icon in the Amazon WorkDocs web client.\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/wd-profile-default.png) 

1. Under **Admin**, choose **Open admin control panel**\.

1. Under **Manage Users**, choose the pencil icon \(![\[pencil icon\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/pencil_icon.png)\) next to the user's name\.

1. Choose **Inactive**, and choose **Save Changes**

The inactivated user can't access your Amazon WorkDocs site\.

**Note**  
Changing a user to **Inactive** status does not delete their files, folders, or feedback from your Amazon WorkDocs site\. However, you can transfer an inactive user's files and folders to an active user\. For more information, see [Transferring document ownership](transfer-docs.md)\.

## Deleting pending users<a name="delete_user_cloud"></a>

You can delete Simple AD, AWS Managed Microsoft, and AD Connector users in **Pending** status\. To delete one of those users, choose the trash can icon \(![\[trash can icon\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/trash_can_icon.png)\) next to the user's name\.

Your Amazon WorkDocs site must always have at least one active user who is not a guest user\. If you need to delete all users, [delete the entire site](delete_site.md)\.

We do not recommend that you delete registered users\. Instead, you should switch a user from **Active** to **Inactive** status to prevent them from accessing your Amazon WorkDocs site\. 