# Permissions<a name="permissions"></a>

Amazon WorkDocs uses permissions to control access to folders and files\. Permissions are applied based on user roles\.

**Topics**
+ [Roles](#roles)
+ [Shared folder permissions](#folder_perms)
+ [File permissions](#doc_perms)
+ [Shared file permissions](#shared_document_perms)

## Roles<a name="roles"></a>

Folder and file permissions are granted based on user roles\. Amazon WorkDocs defines the following roles for folders:
+ Folder owner – The owner of a folder or file\.
+ Folder co\-owner – A user or group that the owner designates as the co\-owner of a folder or file\.
+ Folder contributor – Someone with unlimited access to a folder\.
+ Folder viewer – Someone with limited access \(read\-only permissions\) to a folder\.

The following roles apply to files:
+ Owner – The owner of a file\.
+ Co\-Owner – A user or group that the owner designates as the co\-owner of the file\.
+ Contributor – Someone allowed to give feedback on file\.
+ Viewer – Someone with limited access \(read\-only permissions\) to the file\.
+ Anonymous viewer – A non\-registered user outside of the organization who can view a file that has been shared using an external viewing link\. Unless otherwise indicated, an anonymous viewer has the same permissions as a viewer\.

## Shared folder permissions<a name="folder_perms"></a>

Amazon WorkDocs provides the following permissions for shared folders\. As a reminder, permissions applied to a folder also apply to the files in that folder\.
+ View – View the contents of a shared folder\.
+ View sub\-folder – View a sub\-folder\.
+ View shares – View the other users a folder is shared with\.
+ Download folder – Download a folder\.
+ Add sub\-folder – Add a sub\-folder\.
+ Share – Share the top\-level folder with other users\.
+ Revoke share – Revoke the sharing of the top\-level folder\.
+ Delete sub\-folder – Delete a sub\-folder\.
+ Delete top\-level folder – Delete the top\-level shared folder\.


**Permissions for shared folders**  

| Permission | Folder owner | Folder co\-owner | Folder contributor | Folder viewer | 
| --- | --- | --- | --- | --- | 
| View | X | X | X | X | 
| View Sub\-folders | X | X | X | X | 
| View Shares | X | X | X | X | 
| Download | X | X | X | X | 
| Add Sub\-folder | X | X | X |  | 
| Share | X | X |  |  | 
| Revoke Sharing | X | X |  |  | 
| Delete Sub\-folder | X | X |  |  | 
| Delete Top\-level folder | X | X |  |  | 

## File permissions<a name="doc_perms"></a>

Amazon WorkDocs provides the following permissions for files that do not reside in a shared folder:
+ View – View a file\.
+ Delete – Delete a file\.
+ Annotate – Add feedback to a file\.
+ View Shares – View the other users that a file is shared with\.
+ View Annotations – View feedback from other users\.
+ View Activity – View the activity history of a file\.
+ View Versions – View previous versions of a file\.
+ Download – Download a file\. This is the default permission\. You can use file properties to allow or deny the ability to download shared files\. 
+ Prevent Download – Prevent a file from being downloaded\.
+ Upload – Upload new versions of a file\.
+ Share – Share a file with other users\.
+ Revoke Sharing – Revoke the sharing of a file\.


**Permissions for a file not in a shared folder**  

| Permission | Owner/Co\-Owner | Contributor | Viewer | Anonymous Viewer | 
| --- | --- | --- | --- | --- | 
| View | X | X | X | X | 
| View Shares | X | X | X | X | 
| Download | X | X | X |  | 
| Annotate | X | X |  |  | 
| View Annotations | X | X |  |  | 
| View Activity | X | X |  |  | 
| View Versions | X | X |  |  | 
| Upload | X | X |  |  | 
| Delete | X |  |  |  | 
| Prevent Download | X |  |  |  | 
| Share | X |  |  |  | 
| Revoke Sharing | X |  |  |  | 

## Shared file permissions<a name="shared_document_perms"></a>

Amazon WorkDocs provides the following permissions for files in a shared folder:
+ View – View a file in a shared folder\.
+ View Shares – View the other users that a file is shared with\.
+ Download – Download a file\.
+ Annotate – Add feedback to a file\.
+ View Annotations – View feedback from other users\.
+ View Activity – View the activity history of a file\.
+ View Versions – View previous versions of a file\.
+ Upload – Upload new versions of a file\.
+ Delete – Delete a file in a shared folder\.
+ Prevent Download – Prevent a file from being downloaded\. This is the default permission for files in the folder\. 
+ Share – Share a file with other users\.
+ Revoke Sharing – Revoke the sharing of a file\.
+ Private Comments – Owner/co\-owner can see all private comments for a document, even if they are not replies to their comment\.


**Permissions for a file in a shared folder**  

| Permission | Folder Owner/Co\-Owner | File Owner\* | Folder Contributor | Folder Viewer | Anonymous Viewer | 
| --- | --- | --- | --- | --- | --- | 
| View | X | X | X | X | X | 
| View Shares | X | X | X | X | X | 
| Download | X | X | X | X |  | 
| Annotate | X | X | X |  |  | 
| View Annotations | X | X | X |  |  | 
| View Activity | X | X | X |  |  | 
| View Versions | X | X | X |  |  | 
| Upload | X | X | X |  |  | 
| Delete | X | X |  |  |  | 
| Rename | X | X |  |  |  | 
| Prevent Download | X | X |  |  |  | 
| Share | X | X |  |  |  | 
| Revoke Sharing | X | X |  |  |  | 
| See All Private Comments\*\* | X | X |  |  |  | 

\* The file owner, in this case, is the person who uploaded the original version of a file to a shared folder\. The permissions for this role apply only to the owned file, not all files in the shared folder\.

\*\* File owner/co\-owner can see all private comments\. Contributors can only see private comments that are replies to their comments\.