# Backing up folders with Amazon WorkDocs Backup<a name="admin-backup"></a>

Amazon WorkDocs Backup helps support your data resiliency and backup needs, providing a secure, cloud\-based solution for backing up content stored in user folders\. The app runs in the background, and it's optimized for network bandwidth, device configuration, and content priority\. Amazon WorkDocs Backup provides AES\-256 encryption for data in transit and at rest\.

## Deploying Amazon WorkDocs Backup<a name="deploy-wd-backup"></a>

As an Amazon WorkDocs site administrator, you can deploy Amazon WorkDocs Backup to users in your Amazon WorkDocs organization\. Then you can decide which user folders to back up and how often to back them up\. Amazon WorkDocs Backup automatically backs up the designated folders from your users' Windows or macOS desktop computers to Amazon WorkDocs\. Amazon WorkDocs Backup supports back up from multiple computers for the same user\. Users can recover their backups as needed, and they can update some personal backup settings\. For more information, see [Backing up folders with Amazon WorkDocs Backup](https://docs.aws.amazon.com/workdocs/latest/userguide/user-backup.html) in the *Amazon WorkDocs User Guide*\.

**Deploy Amazon WorkDocs Backup to users in your organization**

1. From the Amazon WorkDocs site, choose **Apps**\.

1. For **Backup**, choose **Launch**\.

1. If prompted, download and install the Amazon WorkDocs Companion app\.

1. Choose **Start**\.

1. For **What type of configuration would you like to set up?**, choose **Group policy**\.

1. Select the folders to back up for your organization, and choose **Next**\.

1. Select a backup frequency, and choose **Next**\.

1. Choose **Finish**\.

Your Amazon WorkDocs site users can access Amazon WorkDocs Backup under **Apps**\. When they start Amazon WorkDocs Backup, they can update their personal app settings and recover their backups as needed\.