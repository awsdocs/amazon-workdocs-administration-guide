# Deploying Amazon WorkDocs Companion on Apple devices<a name="deploy-on-apple"></a>

You can can run a pre\-installation script to plant installation settings\. WorkDocs supports these settings:
+ **SiteId ** – Indicates the organization to which you're deploying Amazon WorkDocs Companion\. This setting allows Companion to start without user interaction\.
+ **BlockAutoUpdate** – If set to true, this setting blocks automatic updates unless you need to deploy a critical update\.

 To plant this setting, run:

```
defaults write /Library/Preferences/com.Amazon.WorkDocs.WorkDocsClient.plist "SiteId" "amazon"
```

To delete the values, run:

```
defaults delete /Library/Preferences/com.Amazon.WorkDocs.WorkDocsClient.plist "SiteId"
```

To read the values, run:

```
defaults read /Library/Preferences/com.Amazon.WorkDocs.WorkDocsClient.plist 
"SiteId" plutil -p /Library/Preferences/com.Amazon.WorkDocs.WorkDocsClient.plist
```