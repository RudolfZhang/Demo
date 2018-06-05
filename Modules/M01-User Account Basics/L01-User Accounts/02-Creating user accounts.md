## Creating user accounts

Update on 6.27

As an IT Administrator, you have several  [managing users tasks](https://technet.microsoft.com/en-us/library/cc754661.aspx). One of those tasks is to create new user accounts. When you create a new user account, you must provide the Full Name, User Name, and Password options. The following screenshots are from the User and Computers tool.

![Screenshot of the New Object - User wizard. The first image highlights the Name and Logon information. The second image highlights the password information. ](../..\Linked_Image_Files\1.1.2.png)

1.  **Full Name**. The First name and Last name attributes combine to create the Full name attribute. Full name is used as the Common Name (CN) and it must be unique within the container or OU.
2.  **User Logon Name**. The User Logon follow the format *user logon name*@*domain suffix*. The Domain Name System name of your domain is always available as a suffix. However, you can add other suffixes if they are needed.
3.  **Password**. Several password options are available. As a best practice, you should always select **User must change password at next logon**. This property enables you to force users to reset their password the next time that they log on. This is typically something that you might enable after you reset a user’s password.
