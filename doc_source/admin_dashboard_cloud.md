# Amazon WorkDocs Cloud Directories<a name="admin_dashboard_cloud"></a>

In the Amazon WorkDocs administration dashboard for a cloud directory, you can manage the following\.


+ [Storage](#storage_cloud)
+ [Security](#security_cloud)
+ [Cloud Directory Users](#manage_users_cloud)

## Storage<a name="storage_cloud"></a>

In the **Storage** section, you can specify the amount of storage that new users receive\. To change this setting, choose **Change** in the **Storage** section\. In the **Storage Limit** dialog box, give new users unlimited storage or limit users to a specific amount of storage\. This setting only affects users that are added after the setting is changed\. It does not change the amount of storage allocated to existing users\. To change the storage limit for an existing user, see [Edit Users](#edit_user_cloud)\.

## Security<a name="security_cloud"></a>

In the **Security** section, you can specify the following\.

### External Share Settings<a name="external_share_settings"></a>

Specifies if users can send file view links to people outside of the organization\. Choose from the following settings:

**Users can send external view links to anyone **  
Users can send links to anyone outside the organization\. 

**Users can send external view links to a few specific domains**  
Users can send links to people who are members of the specified domains\. 

**Users cannot send external view links**  
Users cannot send view links to anyone outside the organization\.

### Invite Settings<a name="invite_settings"></a>

Specifies how users can invite new users to the cloud organization, if applicable\. For a cloud directory, choose from the following settings:

**Users can invite new people from anywhere by sharing files or folders with them**  
Users can invite new people from outside the organization by sharing files or folders with them\. 

**Users can invite new people from a few specific domains by sharing files or folders with them**  
Users can invite new people from the specified domains by sharing files or folders with them\. 

**Only administrators can invite new users**  
Users cannot invite new users\.

## Cloud Directory Users<a name="manage_users_cloud"></a>

In the **Manage Users** section for a cloud directory, you can perform the following tasks\.


+ [Invite New Users](#invite_user)
+ [Edit Users](#edit_user_cloud)
+ [Delete Users](#delete_user_cloud)

### Invite New Users<a name="invite_user"></a>

For cloud directories, you invite new users to join your directory\. 

**To invite new users to a cloud directory**

1. In the **Manage Users** section, choose **Invite Users**\.

1. In the **Invite Users** dialog box, enter the email address of the person you would like to invite in the **Who would you like to invite** field, and press **Enter**\. Repeat for each person you would like to invite\.

1. Enter a customized subject and message body, if desired, and choose **Send**\. An invitation email is sent to each recipient with instructions about how to create an Amazon WorkDocs account\.

### Edit Users<a name="edit_user_cloud"></a>

You can modify an existing user by clicking on the pencil icon \(![\[pencil icon\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/pencil_icon.png)\) next to the user's name\.

In the **Edit User** dialog box, you can change the following settings:

**First Name**  
The user's first name\.

**Last Name**  
The user's last name\.

**Status**  
Specifies if the user is active or inactive\.

**Role**  
Specifies whether the user is a user or administrator\. You can also upgrade or downgrade a user that has an Amazon WorkSpaces WorkSpace assigned to them\. For more information, see [Amazon WorkDocs User Types and Roles](users_ovw.md)\.

**Storage**  
Specifies the storage limit for an existing user\.

### Delete Users<a name="delete_user_cloud"></a>

Using the Amazon WorkDocs administration dashboard, you can only delete a cloud user that has not created their Amazon WorkDocs account yet\. To delete one of these users, choose the trash can icon \(![\[trash can icon\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/trash_can_icon.png)\) next to the user's name\.

We do not recommend that you delete registered users\. Instead, you should deactivate users, so they do not have access to your Amazon WorkDocs site\. For more information about deactivating a user, see [Edit Users](#edit_user_cloud)\.

You must always have at least one active user for your Amazon WorkDocs site\. If you want to delete all users, you must delete your entire Amazon WorkDocs site\.