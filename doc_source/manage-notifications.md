# Managing notifications<a name="manage-notifications"></a>

**Note**  
For greater security, create federated users instead of IAM users whenever possible\.

Notifications allow IAM users or roles to call the [CreateNotificationSubscription](https://docs.aws.amazon.com/workdocs/latest/APIReference/API_CreateNotificationSubscription.html) API, which you can use to set your own endpoint for processing the SNS messages that WorkDocs sends\. For more information about notifications, see [Setting up notifications for an IAM user or role](https://docs.aws.amazon.com/workdocs/latest/developerguide/manage-notifications.html) in the *Amazon WorkDocs Developer Guide*\.

You can create and delete notifications, and the following steps explain how to do both tasks\.

**To create a notification**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the navigation pane, choose **My sites**\.

   The **Manage your WorkDocs sites** page appears and displays a list of your sites\.

1. Choose the button next to the desired site\.

1. Open the **Actions** list and choose **Manage notifications**\.

   The **Set WorkDocs administrator** dialog box appears\.

1. In the **Username** box, enter the new administrator's name, then choose **Set administrator**\.

**To delete a notification**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. In the navigation pane, choose **My sites**\.

   The **Manage your WorkDocs sites** page appears and displays a list of your sites\.

1. Choose the button next to the site for which you want to set an administrator\.

1. Open the **Actions** list and choose **Set an administrator**\.

   The **Set WorkDocs administrator** dialog box appears\.

1. In the **Username** box, enter the new administrator's name, then choose **Set administrator**\.