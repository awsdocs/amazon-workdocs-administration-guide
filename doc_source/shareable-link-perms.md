# Managing link sharing<a name="shareable-link-perms"></a>

This topic explains how to manage link sharing\. Amazon WorkDocs users can share their files and folders by sharing links to them\. They can share file links inside and outside your organization, but they can only share folder links internally\. As an administrator, you manage who can share links\.

**To enable link sharing**

1. Choose the profile icon in the upper\-right corner of the WorkDocs client\.

    ![\[The default profile icon in the Amazon WorkDocs web client.\]](http://docs.aws.amazon.com/workdocs/latest/adminguide/images/wd-profile-default.png) 

1. Under **Admin**, choose **Open admin control panel**\.

1. Scroll down to **Security** and choose **Change**\.

   The **Policy Settings** dialog box appears\.

1. Under **Choose your setting for shareable links**, select an option:
   + **Do not allow site\-wide or public shareable links** – Disables link sharing for all users\.
   + **Allow users to create site\-wide shareable links, but do not allow them to create public shareable links** – Limits link sharing to just site members\. Managed users can create this type of link\.
   + **Allow users to create site\-wide shareable links, but only power users can create public shareable links** – Managed users can create site\-wide links, but only power users can create public links\. Public links allow access to anyone on the internet\.
   + **All managed users can create site\-wide & public shareable links** – Managed users can create public links\.

1. Choose **Save Changes**\.