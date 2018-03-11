# Amazon WorkDocs Sharing<a name="sharing"></a>

There are multiple ways users can share content in Amazon WorkDocs:

+ **Share a Link** allows users to quickly copy and share hyperlinks to content stored in Amazon WorkDocs with coworkers and external partners both inside and outside their organization\. Shareable links can be configured to allow access to site members only or anyone on the internet\. Links with access to site members can be configured for viewing and commenting, while links with access to anyone is restricted to viewing only\. Recipients with viewing permissions can only view a file only, while commenting permissions enables users to comment and perform update or delete operations, such as uploading a new file or deleting an existing file\.

  You can control which users can create links to share their Amazon WorkDocs content with the public\. By default, all managed users can create public links\. To change this setting, choose **Administration**, **Security**, **Change**, and then select one of the following options:

  + **No public sharing**: The ability to create public links is disabled for all site users\.

  + **All managed users can share publicly**: The ability to create public links is enabled for all site users\.

  + **Only power users can share publicly**: The ability to create public links is restricted to powers users only\.

+ **Share by invite** allows users to share files of folders with other users by inviting them using their email address, and set the appropriate permission level for each invited user\. Invited users automatically receive an invite email notifying them that content has been shared with them\. Clicking on the link in the email opens the shared file\. Users can share files and folders with other site members or with external users\. 

+ External sharing allows managed users of an Amazon WorkDocs site to share files and folders and collaborate with external users in a convenient way without incurring extra costs\. Users of a site can share files and folders with external users without requiring recipients to be paid users of the Amazon WorkDocs site\. If external sharing is enabled, users can type the email address of the external user they want to share with and set appropriate viewer sharing permissions\. When external users are added, permissions are limited to viewer only and other permissions are not available\. External users receive an email notification with a link to the shared file or folder\. Choosing the link takes external users to the site, where they enter their credentials to log in to Amazon WorkDocs\. They can see the shared file or folder in the **Shared with me** view\.

  File owners can modify sharing permissions or remove access for the external user from a file or folder at any time\. External sharing for the site must be enabled by the site administrator in order for managed users to share content with external users\. For** Guest users** to become contributors or co\-owners, they must be upgraded to the **User** level by a site administrator\.

  By default, external sharing is turned on and all users can invite external users\. To change this setting, choose **Administration**, **Security**, **Change**, and then select one of the following options:

  + **Only administrators can invite new external users\.**

  + **All managed users can invite new external users\.** \(selected by default\)

  + **Only power users can invite new external users\.**