# Permissions<a name="permissions"></a>

Amazon WorkDocs uses permissions to control access to folders and files\. Permissions are applied based on user roles\.

**Topics**
+ [User roles](#roles)
+ [Permissions for shared folders](#folder_perms)
+ [Permissions for files in shared folders](#shared_document_perms)
+ [Permissions for files not in shared folders](#doc_perms)

## User roles<a name="roles"></a>

User roles control folder and file permissions\. You can apply the following user roles at the folder level:
+ **Folder owner** – The owner of a folder or file\.
+ **Folder co\-owner** – A user or group that the owner designates as the co\-owner of a folder or file\.
+ **Folder contributor** – Someone with unlimited access to a folder\.
+ **Folder viewer** – Someone with limited access \(read\-only permissions\) to a folder\.

You can apply the following user roles at the individual file level:
+ **Owner** – The owner of a file\.
+ **Co\-owner** – A user or group that the owner designates as the co\-owner of the file\.
+ **Contributor** – Someone allowed to give feedback on file\.
+ **Viewer** – Someone with limited access \(read\-only permissions\) to the file\.
+ **Anonymous viewer** – A non\-registered user outside of the organization who can view a file that has been shared using an external viewing link\. Unless otherwise indicated, an anonymous viewer has the same permissions as a viewer\.

## Permissions for shared folders<a name="folder_perms"></a>

The following permissions apply to user roles for shared folders:

**Note**  
Permissions applied for a folder also apply to the sub\-bolders and files in that folder\.
+ **View** – View the contents of a shared folder\.
+ **View sub\-folders** – View a sub\-folder\.
+ **View shares** – View the other users a folder is shared with\.
+ **Download folder** – Download a folder\.
+ **Add sub\-folder** – Add a sub\-folder\.
+ **Share** – Share the top\-level folder with other users\.
+ **Revoke share** – Revoke the sharing of the top\-level folder\.
+ **Delete sub\-folder** – Delete a sub\-folder\.
+ **Delete top\-level folder** – Delete the top\-level shared folder\.


|   | View | View sub\-folders | View shares | Download folder | Add sub\-folder | Share | Revoke share | Delete sub\-folder | Delete top\-level folder | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| Folder owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Folder co\-owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Folder contributor | ✓ | ✓ | ✓ | ✓ | ✓ |  |  |  |  | 
| Folder viewer | ✓ | ✓ | ✓ | ✓ |  |  |  |  |  | 

## Permissions for files in shared folders<a name="shared_document_perms"></a>

The following permissions apply to user roles for files in a shared folder:
+ **Annotate** – Add feedback to a file\.
+ **Delete** – Delete a file in a shared folder\.
+ **Rename** – Rename files\.
+ **Upload** – Upload new versions of a file\.
+ **Download** – Download a file\.
+ **Prevent download** – Prevent a file from being downloaded\. This is the default permission for files in the folder\. 
+ **Share** – Share a file with other users\.
+ **Revoke sharing** – Revoke the sharing of a file\.
+ **View** – View a file in a shared folder\.
+ **View shares** – View the other users that a file is shared with\.
+ **View annotations** – View feedback from other users\.
+ **View activity** – View the activity history of a file\.
+ **View versions** – View previous versions of a file\.
+ **Delete versions** – Delete one or more versions of a file\.
+ **Recover versions** – Recover one or more deleted versions of a file\.
+ **View all private comments** – Owner/co\-owner can see all private comments for a document, even if they are not replies to their comment\.


|   | Annotate  | Delete | Rename | Upload | Download | Prevent download | Share | Revoke share | View | View shares | View annotations | View activity | View versions | Delete versions | Recover versions | View all private comments\*\* | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| File owner\* | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Folder owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Folder co\-owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Folder contributor | ✓ |   |   | ✓ | ✓ |   |   |   | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   | 
| Folder viewer |   |   |   |   | ✓ |   |   |   | ✓ | ✓ |   |   |   |   |   |   | 
| Anonymous viewer |   |   |   |   |   |   |   |   | ✓ | ✓ |   |   |   |   |   |   | 

\* The file owner, in this case, is the person who uploaded the original version of a file to a shared folder\. The permissions for this role apply only to the owned file, not all files in the shared folder\.

\*\* File owner/co\-owner can see all private comments\. Contributors can only see private comments that are replies to their comments\.

## Permissions for files not in shared folders<a name="doc_perms"></a>

The following permissions apply to user roles for files that do not reside in a shared folder:
+ **Annotate** – Add feedback to a file\.
+ **Delete** – Delete a file\.
+ **Rename** – Rename files\.
+ **Upload** – Upload new versions of a file\.
+ **Download** – Download a file\. This is the default permission\. You can use file properties to allow or deny the ability to download shared files\. 
+ **Prevent download** – Prevent a file from being downloaded\.
+ **Share** – Share a file with other users\.
+ **Revoke share** – Revoke the sharing of a file\.
+ **View** – View a file\.
+ **View shares** – View the other users that a file is shared with\.
+ **View annotations** – View feedback from other users\.
+ **View activity** – View the activity history of a file\.
+ **View versions** – View previous versions of a file\.
+ **Delete versions** – Delete one or more versions of a file\.
+ **Recover versions** – Recover one or more deleted versions of a file\.


|   | Annotate  | Delete | Rename | Upload | Download | Prevent download | Share | Revoke share | View | View shares | View annotations | View activity | View versions | Delete versions | Recover versions | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| Owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Co\-owner | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Contributor | ✓ |   |   | ✓ | ✓ |   |   |   | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | 
| Viewer |   |   |   |   | ✓ |   |   |   | ✓ | ✓ |   |   |   |   |   | 
| Anonymous viewer |   |   |   |   |   |   |   |   | ✓ | ✓ |   |   |   |   |   | 