# Amazon WorkDocs Connected Directories<a name="admin_dashboard_connect"></a>

In the administration dashboard for a connected directory, you can manage the following\.


+ [Storage](#storage_connect)
+ [Security](#security_connect)
+ [Connected Directory Users](#manage_users_connect)

## Storage<a name="storage_connect"></a>

In the **Storage** section, you can specify the amount of storage that new users receive\. To change this setting, choose **Change** in the **Storage** section\. In the **Storage Limit** dialog box, give new users unlimited storage or limit users to a specific amount of storage\. This setting only affects users that are enabled after the setting is changed\. It does not change the amount of storage allocated to currently enabled users\. To change the storage limit for an enabled user, see [Edit Users](#edit_user_connect)\.

## Security<a name="security_connect"></a>

In the **Security** section, you can specify the following\.

### External Share Settings<a name="external_share_settings_connect"></a>

Specifies if users can send file view links to people outside of the organization\. Choose from the following settings:

**Users can send external view links to anyone **  
Users can send links to anyone outside the organization\. 

**Users can send external view links to a few specific domains**  
Users can send links to people who are members of the specified domains\. 

**Users cannot send external view links**  
Users cannot send view links to anyone outside the organization\.

### Invite Settings<a name="invite_settings_connect"></a>

For connected directories, you don't invite new users to join your directory\. You can only enable users that already exist in your directory to use Amazon WorkDocs\. For a connected directory, choose from the following settings:

**Users can enable new people from your directory by sharing files or folders with them**  
Users can enable people that already exist in your directory to use Amazon WorkDocs by sharing files or folders with them\.

**Only administrators can enable new users**  
Only Amazon WorkDocs administrators can enable users to use Amazon WorkDocs\.

## Connected Directory Users<a name="manage_users_connect"></a>

In the **Manage Users** section for a connected directory, you can perform the following tasks\.


+ [Enable Users](#enable_user_connect)
+ [Edit Users](#edit_user_connect)

### Enable Users<a name="enable_user_connect"></a>

For connected directories, you don't invite new users to join your directory, you enable users that already exist in your directory to use Amazon WorkDocs\. For more information about enabling a user, see [Edit Users](#edit_user_connect)\.

### Edit Users<a name="edit_user_connect"></a>

You can modify an existing user by choosing the pencil icon \(![\[pencil icon\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/pencil_icon.png)\) next to the user's name\.

In the **Edit User** dialog box, you can change the following settings:

**Status**  
Specifies if the user is active or inactive\.

**Role**  
Specifies whether the user is a user or administrator\. You can also upgrade or downgrade a user that has an Amazon WorkSpaces WorkSpace assigned to them\. For more information, see [Amazon WorkDocs User Types and Roles](users_ovw.md)\.

**Storage**  
Specifies the storage limit for an existing user\.