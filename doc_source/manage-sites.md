# Managing Amazon WorkDocs from the site admin control panel<a name="manage-sites"></a>

You use these tools to manage your Amazon WorkDocs sites:
+ The site admin control panel, available to administrators on all Amazon WorkDocs sites, and described in the following topics\.
+ The AWS console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

Each of those tools provides a different set of actions\. The topics in this section explain the actions provided by the site admin control panel\. For information about the tasks available in the console, see [Managing Amazon WorkDocs from the AWS console](console-administration.md)\.

## Preferred language settings<a name="language-settings"></a>

You can specify the language for email notifications\.

**To change language settings**

1. Under **My Account**, choose **Open admin control panel**\.

1. For **Preferred Language Settings**, choose your preferred language\.

## Hancom Online Editing and Office Online<a name="online-editing"></a>

Enable or disable **Hancom Online Editing** and **Office Online** settings from the **Admin control panel**\. For more information, see [Enabling collaborative editing](collab-editing.md)\.

## Storage<a name="storage-limits"></a>

Specify the amount of storage that new users receive\.

**To change storage settings**

1. Under **My Account**, choose **Open admin control panel**\.

1. For **Storage**, choose **Change**\.

1. In the **Storage Limit** dialog box, choose whether to give new users unlimited or limited storage\.

1. Choose **Save Changes**\.

Changing the storage setting affects only users that are added after the setting is changed\. It does not change the amount of storage allocated to existing users\. To change the storage limit for an existing user, see [Editing users](edit_user.md)\.

## IP allow list<a name="ipfiltering"></a>

Amazon WorkDocs site administrators can add **IP Allow List** settings to restrict site access to an allowed range of IP addresses\. You can add up to 32 **IP Allow List** settings per site\.

**Note**  
The **IP Allow List** currently works for IPv4 addresses only\. IP address denylisting is not currently supported\.

**To add an IP range to the **IP Allow List****

1. Under **My Account**, choose **Open admin control panel**\.

1. For **IP Allow List**, choose **Change**\.

1. For **Enter CIDR value**, enter the Classless Inter\-Domain Routing \(CIDR\) block for the IP address ranges, and choose **Add**\.

   1. To allow access from a single IP address, specify `/32` as the CIDR prefix\.

1. Choose **Save Changes**\.

1. Users who connect to your site from the IP addresses on the **IP Allow List** are allowed access\. Users who attempt to connect to your site from unauthorized IP addresses receive an unauthorized response\.

**Warning**  
If you enter a CIDR value that blocks you from using your current IP address to access the site, a warning message appears\. If you choose to continue with the current CIDR value, you will be blocked from accessing the site with your current IP address\. This action can only be reversed by contacting AWS Support\.

## Security – public share settings<a name="external_share_settings"></a>

In the **Admin control panel**, under **Security**, choose **Who should be allowed to create publicly shareable links?** to specify which users are allowed to send file view links to people outside of the organization\. Choose from the following settings:

**No public sharing**  
Users cannot send view links to anyone outside the organization\.

**All managed users can share publicly **  
All users can send view links to anyone outside the organization\. 

**Only Power users can share publicly**  
Only Power users can send view links to people outside the organization\. 

## Security – invitation settings<a name="invitation-settings"></a>

Choose from the following settings for **Who should be allowed to join your WorkDocs site?**\.

**Users can invite people from anywhere by sharing files or folders with them**  
Users can invite people from anywhere outside the organization by sharing files or folders with them\.

**Users can invite new people from a few specific domains by sharing files or folders with them**  
Users can invite new people from the specified domains by sharing files or folders with them\. 

## Security – external invitations<a name="ext-invite-settings"></a>

Choose from the following settings for **Who should be allowed to invite external users to your WorkDocs site?**

**Only administrators can invite new external users**  
Only administrators can invite external users to use Amazon WorkDocs\.

**All managed users can invite new external users**  
All users can invite new external users to use Amazon WorkDocs\.

**Only Power users can invite new external users**  
Only Power users can invite new external users to use Amazon WorkDocs\.

## Recovery bin retention<a name="recovery-bin"></a>

When a user deletes a file, Amazon WorkDocs stores the file in the user’s recycle bin for 30 days\. Afterwards, Amazon WorkDocs moves the files to a temporary recovery bin for 60 days, then deletes them permanently\. Only administrators can see the temporary recovery bin\. By changing the site\-wide data retention policy, site administrators can change the recovery bin retention period to a minimum of zero days and maximum of 365\.

**To change the recovery bin retention period**

1. Under **My Account**, choose **Open admin control panel**\.

1. Next to **Recovery bin retention**, choose **Change**\.

1. Enter the number of days to retain files in the recovery bin, and choose **Save**\.
**Note**  
The default retention period is 60 days\. You can use a period of 0–365 days\.

Administrators can restore user files from the recovery bin before Amazon WorkDocs deletes them permanently\.

**To restore a user's file**

1. Under **My Account**, choose **Open admin control panel**\.

1. Under **Manage Users**, choose the user's folder icon\.

1. Under **Recovery bin**, select the file\(s\) to restore, then choose the **Recover** icon\.

1. For **Restore file**, choose the location to which to restore the file, then choose **Restore**\.

## Manage user settings<a name="manage-users-settings"></a>

You can manage settings for users, including changing user roles and inviting, enabling, or disabling users\. For more information, see [Inviting and managing Amazon WorkDocs users](users.md)\.