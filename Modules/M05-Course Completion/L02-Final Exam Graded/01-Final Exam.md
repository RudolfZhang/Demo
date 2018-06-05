## 1. Checkbox  

You need to restrict the days and times that a specific user account can access resources in your domain. What should you do?  
[ ] Modify the account expiration date to expire on the dates that the user should be restricted.  
[ ] Modify the computers that the user is enabled to log on to so that it is empty on the days that the user should be restricted.  
[x] Modify the logon hours for the account so that the user is permitted or restricted on certain days and times.  
[ ] Set the lockoutTime attribute to the dates and times that the user should be restricted.  
[ ] Set the msDS-AllowedToDelegateTo attribute to the dates and times that the user should not be restricted.  

[explanation]  
To restrict the days and times that a specific user account can be used to access resources in your domain, adjust the logon hours (the logonHours attribute). You can choose to permit logons during specific days and times or to deny logons during specific days and times.  
[explanation]  

---

## Multiple Choice

You create a new standard password policy for your organization. You enable the password complexity option. The helpdesk receives a large volume of calls because users are having trouble choosing new passwords that meet the complexity requirements. You need to educate the helpdesk so that they can help guide the users. Which of the following statements about password complexity should you use when explaining password complexity to the helpdesk?  
( ) At a minimum, passwords must have letters and numbers.  
(x) Passwords must have characters from 3 of the 4 character sets:  upper case letters, lower case letters, numbers, and special characters.  
( ) Passwords must have upper case letters, lower case letters, and numbers.  
( ) Passwords must have at least one character from all the character sets:  upper case letters, lower case letters, numbers, and special characters.  
( ) Passwords must have letters, numbers, and be a minimum length of 15 characters.  

[explanation]  
In a password policy, password complexity mandates that a password have at least one character in 3 of the 4 character sets:  upper case letters, lower case letters, numbers, and special characters.  
[explanation]  

---

## Checkbox 

Your IT security team contacts you to report that there is an active denial-of-service attack on user credentials. In the last few minutes, hundreds of accounts have been locked out. The security team reports that the attackers are using a script to try invalid passwords across many user accounts. The script is running continuously and locking user accounts out. You check the account lockout policy and notice that the account lockout threshold is set to 5 attempts. You need to ensure that a denial-of-service attack will not impact users from signing in with their accounts. What should you do?  
[ ] Set the account lockout threshold to 999 attempts.  
[x] Set the account lockout threshold to 0 attempts.  
[ ] Set the account lockout duration to 99999 minutes.  
[ ] Set the account lockout duration to 0 minutes.  

[explanation]  
To ensure that a denial-of-service attack against account passwords does not impact users, you must disable account lockout completely by setting the account lockout threshold to 0 attempts.  
[explanation]  

---

## Multiple Choice

You create a shared folder named Share1 on a server named Server1. You create a new security group named Group1. You edit Share1 by removing all existing access control entries and then grant Group1 full control NTFS and share permissions to Share1. You add a user named Ed Meadows to Group1. From his computer, Ed tries to open the \\Server\Share1 but the server reports that he does not have access. You need to ensure that Ed has access to Share1. What should you do?  
( ) Tell Ed Meadows to wait 60 minutes for the shared folder permissions to update.  
( ) Grant Group1 full control NTFS and share permissions to Share1 again.  
( ) Have Ed Meadows sign off from Server1 and then sign in again.  
(x) Have Ed Meadows sign off from his computer and then sign in again.  
( )  Add Ed Meadows to the local Administrators group on Server1.  

[explanation]  
During the sign in process, a user’s access token is built based on their group membership at the time of the sign in. If a user is added to a group after a sign in, the user must sign off so that the access token can be refreshed with new group memberships.  
[explanation]  

---

## Checkbox

Your company, Tailspin Toys, recently acquired a competitor named Wingtip Toys. Each company has their own single-domain forest. As part of the acquisition, the companies connected their networks and implemented a two-way forest trust between the forests. The IT team from Tailspin Toys needs access to a shared folder in the Wingtip Toys domain. You need to create security groups to enable the required access. Which of the following three actions should you take?  
[ ] Create a domain local group named TT-IT1 for the Tailspin Toys IT team.  
[x] Create a global group named TT-IT2 for the Tailspin Toys IT team.  
[x] Create a domain local group named Share1-Read1 in the Wingtip Toys domain.  
[ ] Create a global group named Share1-Read2 in the Wingtip Toys domain.  
[x] Add the TT-IT2 group to the Share1-Read1 group.  
[ ] Add the TT-IT2 group to the Share1-Read2 group.  

[explanation]  
To nest a group from the Tailspin Toys domain to a group in the Wingtip Toys domain, you need to use a global group in the Tailspin Toys domain and nest it into a domain local group in the Wingtip Toys domain. The domain local group can nest global groups from trusted domains.  
[explanation]  

---

## Checkbox

You delegate administrative rights to the IT security team. One of those rights enables the team to reset user passwords for users in the CorpUsers OU. The CorpUsers OU contains a mix of standard user accounts and administrative user accounts for Active Directory administrators. During testing, the IT security team reports that they are only able to reset some of the user passwords in the CorpUsers OU. You need to update the environment to meet the following requirements:  

+ Ensure that the IT security team can reset passwords for all user accounts in the CorpUsers OU.  
+ Ensure that the solution does not require continuing administrative work.  

What should you do?  
[ ] Enable inheritance for all the user accounts in the CorpUsers OU.  
[ ] Disable inheritance for the CorpUsers OU.  
[ ] Add the IT security team users to the Protected Groups group.  
[ ] Delegate the IT security team the right to unlock user accounts.  
[x] Add the IT security team to the Domain Admins group.  

[explanation]  
The CorpUsers OU contains Active Directory administrative accounts, which are protected by being members of protected groups. To enable the IT security team to reset the passwords for members of protected groups, they need to be in the Domain Admins group.  
[explanation]  

---

## Checkbox 

You manage your organization’s Active Directory Domain Services environment. The environment is currently configured to only allow Domain Admins to join a computer to the domain. You propose enabling users in branch offices to join their own computers to the domain. The centralized IT team will ship the computers to the branch office users and the branch office users will join them to the domain. The IT security team agrees to the idea and institutes the following requirements:  

+ The branch office must only be able to join IT-specified computers to the domain.  
+ The solution must maximize security.  

You need to configure your environment to meet the requirements. What should you do?  
[ ] Grant the “Add workstations to the domain” user rights to the users by using a GPO.  
[x] Pre-stage the user computer objects for each user.  
[] Delegate the branch office the right to create computer objects in the domain.  
[ ] Add the users to the Account Operators group.  
[ ] Add the users to the Domain Admins group.  

[explanation]  
To enable users in a branch office to join their computers to the domain, you can pre-stage the computer accounts. During pre-staging, you choose the user or group who can join the pre-staged computer to the domain to complete the process. This solution maximizes security because it ensures that the users cannot join other computers to the domain.  
[explanation]  

---

## Checkbox

You manage the Active Directory environment for your company. All client computer objects are in the Client Computers OU. A user reports that their client computer does not have the correct local Administrator account name. It is “Administrator” but the user thinks it should be “CorpAdmin”. You check other client computers and find the same thing. You look at the current Group Policy configuration and find the following configuration:  

+ The Security Settings GPO, which is linked to the Client Computers OU, is configured to rename the local Administrator account to “Administrator”.  
+ All client computers have a local security policy to rename the local Administrator to “Administrator”.  
+ A Default Domain Policy GPO, which is linked to the domain, is configured to rename the local Administrator account to “Administrator”.  

You need to ensure that all client computers have the local Administrator account renamed to “CorpAdmin”. What should you do?  
[ ] Move all client computers to the Computer container.  
[ ] Remove the renaming of the Administrator account from the local security policy.  
[ ] Change the link order of the Default Domain Policy GPO so that it has the lowest link order.  
[x] Configure the Security Settings GPO to rename the Administrator account to “CorpAdmin”.  
[ ] Configure the local security policy on client computers to rename the Administrator account to “CorpAdmin”.  
[ ] Configure the Default Domain Policy to rename the Administrator account to “CorpAdmin”.  

[explanation]  
When more than one policy tries to set the same policy setting, the policy that is applied last takes precedence and “wins”. In this scenario, the last GPO to be applied is the Security Settings GPO because it is linked at the OU level, which is lower than the domain level. GPO processing occurs after the local security policy.  
[explanation]  

---

## Checkbox

You manage the Active Directory environment for your company. The company has a network operations team with a support center that is several computers. A GPO is linked to the OU that contains the network operations team computers. The manager reports that one of her workers on the night shift is unable to sign in to some of the computers. However, the user can sign into to other computers. You need to ensure that the user can sign into all the support center computers. What should you do?  
[x] Modify the logonWorkstation attribute on the user’s account.  
[ ] Modify the logonHours attribute on the user’s account.  
[ ] Disable the “Smart card is required for interactive logon” option on the user’s account.  
[ ] Modify the otherLoginWorkstations attribute on the user’s account.  
[ ] Add the user’s account to the “Access this computer from the network” GPO setting.  
[ ] Add the user’s account to the “Allow log on locally” GPO setting.  

[explanation]  
Because the user can sign into some of the computers, you can deduce that the user account is not authorized to sign into all the computers. The only answer choice that supports limiting sign on to specific computers is the answer directing to modify the logonWorkstation attribute. The attribute contains a list of computers that the user can sign into.  
[explanation]  

---

## Checkbox

You are creating new user accounts for a new department at your company. You create a template that has some user account properties populated. You name the template “_Department1”. You need to use PowerShell’s New-ADUser cmdlet to create new users by specifying the template. Which parameter should you use?  
[ ] -Credential  
[ ] -PassThru  
[ ] -Path  
[x] -Instance  
[ ] -ProfilePath  

[explanation]  
To create a new user from an existing template in PowerShell, you should use the New-ADUser cmdlet with the -Instance parameter. The -Instance parameter specifies the existing template account to use as the template.  
[explanation]  

---

## Checkbox  

You manage Active Directory Domain Services for your organization. A user reports that they are unable to change their password. When the user tries to change the password, the computer reports that the password does not meet the password requirements. The user is certain that the password meets the password requirements. You look at the current configuration and find the following information:  

+ The user is a member of a group named “IT Admins” and there is an existing fine-grained password policy named Policy1 that applies to the group. The policy has a precedence of 10.  
+ The user is a member of a group named “Corp Users” and there is an existing fine-grained password policy named Policy2 that applies to the group. The policy has a precedence of 15.  
+ The Default Domain Policy has password policy settings defined.  
+ You find an existing fine-grained password policy named Policy3 that does not apply to any objects. It has a precedence of 12.  

You need to ensure that the password settings from Policy3 apply to the user. Which of the two following solutions should you use? (Each answer represents a complete solution. Choose two.)  
[ ] Set the precedence of Policy3 to 20.  
[ ] Remove the password settings from the Default Domain Policy.  
[x] Apply the Policy3 policy directly to the user.  
[x] Set the precedence of Policy3 to 5.  
[ ] Remove the password settings from Policy1.  

[explanation]  
A fine-grained password policy applied directly to a user takes precedence over a policy applied indirectly (via group membership). A fine-grained password policy with the lowest precedence value takes precedence over fine-grained password policies with higher precedence values when they apply at the group level.  
[explanation]  

---

## Checkbox 

You manage Active Directory Domain Services for your organization. You have a GPO that sets Internet Explorer computer settings for all computers in the CorpComputers OU and its child OU. However, one of the computers, named Computer1, must not have the GPO apply to it. Computer1 is the only computer stored in the child OU. Computer1 must not be moved. You need to ensure that the GPO settings do not apply to Computer1 but still apply to the other computers in the CorpComputers OU. What should you do? (Each answer presents an independent solution. Choose two.)  
[x] Add Computer1 to the advanced delegation and set the permissions to only allow “Apply Group Policy”.  
[x] Add Computer1 to the advanced delegation and set the permissions to deny “Apply Group Policy”.  
[ ] Individually add all the client computers from the CorpComputersOU, except for Computer1.  
[ ] Configure loopback processing on the GPO and use Merge mode.  
[ ] Configure loopback processing on the GPO and use Replace mode.  

[explanation]  
To apply a GPO, a computer or user must have Read and Apply Group Policy permissions. Having just one of those permissions means that the computer or user won’t apply the GPO.  
[explanation]  

---

## Checkbox

You manage Active Directory Domain Services for your organization. You have a GPO that sets security-related settings for all computers in the CorpComputers OU and its child OU. However, you have one computer in the child OU that must not have the GPO applied to it. You check current configuration and find the following configuration:  

+ The GPO is linked to the CorpComputers OU with a standard GPO link.  
+ The GPO is linked to the child OU with an enforced GPO link.  

You need to ensure that the computer does not have the GPO applied to it. What should you do?  
[ ] Configure the child OU to block inheritance.  
[ ] Disable inheritance on the computer object in Active Directory.  
[x] Move the computer outside of the CorpComputers OU structure.  
[ ] Move the computer to the CorpComputers OU.  

[explanation]  
When a GPO link is enforced, it overrides inheritance blocking. To ensure that the computer does not have the GPO applied, it needs to be moved outside of the CorpComputers OU structure. While the GPO link is only enforced for the child OU, the GPO is still applying to the CorpComputes OU.  
[explanation]  

---

## Checkbox

You manage Active Directory Domain Services for your organization. All servers are in an OU structure named Servers and in an Active Directory site named Miami. You are planning to deploy a new GPO named GPO4 to set some security-related settings for servers in the File Servers OU, which is a child OU in the Servers OU. You check current configuration and find the following configuration:  

+ There is an existing GPO named GPO3 that is linked to the Servers OU.  
+ GPO4 has some settings that conflict with GPO3.  

You link GPO4 to the Servers OU but the settings from GPO3 are being applied to servers. You need to ensure that the settings from GPO4 take precedence over the settings from GPO3. You also need to ensure that you minimize the complexity of the configuration to ease the administrative overhead of managing the environment. What should you do?  
[ ] Link GPO4 to the Miami site.  
[ ] Link GPO4 to the domain.  
[x] Set the link order of GPO4 to be one order lower than GPO3.  
[ ] Set the link order of GPO4 to be one order higher than GPO3.  

[explanation]  
Because the GPOs are linked at the OU level, you can’t link GPO4 at a site or domain level because the settings won’t take precedence over GPOs linked at the OU level (due to LSDOU). When two GPOs are both linked to the same OU, the GPO link with the lowest link order takes precedence.  
[explanation]  

---

## Checkbox  

You are preparing to join a computer to the domain using the offline domain join feature. You have a laptop computer in a workgroup. You need to perform all the steps to join the computer to the domain using the offline domain join feature. Which of the following steps should you do first?  
[ ] Create a computer account for laptop computer in Active Directory Users and Computers.  
[ ] Reboot the laptop computer.  
[x] Run the djoin.exe command with the /provision, /domain, /machine, and /savefile parameters.  
[ ] Run the djoin.exe command with the /requestODJ, /loadfile, /windowspath, and /localos parameters  
[ ] Transfer the text file from djoin.exe to the laptop computer.  

[explanation]  
You create a computer account as part of the djoin.exe command. You need to create the computer account and text file, transfer it to the desired computer, use the djoin.exe command to configure the computer on next reboot, and then restart the computer to complete the offline domain join process.  
[explanation]  

---

## Checkbox

You are the systems administrator for Tailspin Toys. A client computer technician, that started at the company 2 weeks ago, reports that he is no longer able to join client computers to the tailspintoys.com domain. He says that he successfully joined some computers to the domain already but that it stopped working yesterday. You need to ensure that the client computer technician can join client computers to the domain. What should you do?  

[ ] Add the client computer technician to the “Add workstations to domain” GPO policy setting.  
[ ] Add the client computer technician to the “Create global objects” GPO policy setting.  
[ ] Change the ms-DS-MachineAccountQuota from 10 to 0.  
[x] Grant the client computer technician Create and Delete rights for computer objects on the Computers container.  

[explanation]  
By default, the Authenticated Users group can join 10 computers to the domain. You can adjust that number by modifying the ms-DS-MachineAccountQuota to a different number (with 0 disabling the ability for the Authenticated Users group to join computers to the domain). Because the Authenticated Users group is, by default, already part of the “Add workstations to domain” GPO setting, adding a user account to the setting won’t change anything. You should delegate rights to create and delete computer objects to the Computers container (or another container that you use to store newly created computer objects).  
[explanation]  

---

## Checkbox

You are the systems administrator for Tailspin Toys. Another administrator accidentally deletes a computer object. Thereafter, he can’t sign into the domain from that server. He rejoins the computer to the domain. He can sign in thereafter. However, he notices some access issues that leads him to believe that the entitlements for the server have been modified. You need to figure out what is causing the change in entitlements for the server and report your findings to the security team. What should you do?  
[x] Report that the computer object security identifier (SID) has changed and is causing the change in entitlements.  
[ ] Report that the computer globally unique identifier (GUID) has changed and is causing the change in entitlements.  
[ ] Report that the computer secure channel is broken and is causing the change in entitlements.  
[ ] Report that the server’s computer object is missing from the domain and is causing the change in entitlements.  

[explanation]  
When a computer account is recreated, it gets a new SID. The old SID, which was associated with entitlements via direct assignment or via group membership, is deleted during the computer object deletion. Because the server has a new SID, it must be granted entitlements from scratch (via direct assignment or via group membership). In a deletion scenario, it is a good practice to try to restore the deleted object prior to recreating it to avoid a loss of computer entitlements.  
[explanation]  
 
---

## Checkbox

You are the systems administrator for Alpine Ski House. An outside consulting company performs a security audit. One finding relates to computer objects. The company found that new domain-joined servers are not receiving any GPOs. You look at the existing configuration and find that there are several GPOs linked to the Servers OU, which is in the root of the alpineskihouse.com domain. Most server-based computer objects are stored in the Servers OU but they are manually moved to the Servers OU during the application deployment. You need to ensure that servers get GPOs applied to them as soon as possible after joining the domain. What should you do?  
[ ] Run the gpupdate /force command after completing the domain join process.  
[ ] Run the Invoke-GPUpdate PowerShell command after completing the domain join process.  
[ ] Run the redircmp “OU=Servers,DC=alpineskihouse.com” command.  
[x] Run the redircmp “OU=Servers,DC=alpineskihouse,DC=com” command.  

[explanation]  
By default, new domain-joined computers have computer objects created in the Computers container. GPOs do not target the Computers container. To ensure that computers get GPOs as soon as possible after a domain join operation, you should change the default location for computer objects. In this scenario, dealing with servers, you should use the redircmp tool to change the default location for servers to the Servers OU.  
[explanation]  

---

## Checkbox

You are the system administrator for Contoso Ltd. Your company merges with a company named Fabrikam Inc. You implement a two-way forest trust. You plan to enable the IT teams to work across both companies’ server environments. You check the current configuration and find the following configuration items:  
 
+ In the Contoso environment, there is an existing domain local group named “Server Admins” that grants administrative access to member servers.  
+ In the Fabrikam environment, there is an existing global group named “IT Admins” that grants administrative access to member servers.  

You need to ensure that the Contoso group can be used to grant administrative access across both environments but limit the Fabrikam group to be limited go granting access in the Fabrikam environment only. Which two actions should you perform? (Choose two.)  
[ ] Convert the domain local group in the Contoso environment to a global group.  
[x] Convert the domain local group in the Contoso environment to a universal group.  
[ ] Convert the global group in the Fabrikam environment to a universal group.  
[x] Convert the global group in the Fabrikam environment to a domain local group.  

[explanation]  
The Contoso group must be able to be granted access across both forests. Thus, it must be a universal group. The Fabrikam group must only have access to the Fabrikam environment so it should be a domain local group. A domain local group can only be granted access within the same domain as the domain of the group.  
[explanation]  

---

## Checkbox

You are the system administrator for Contoso Ltd. A user reports that they are unable to sign in. You reset the password and do not check the option to force a password reset upon next logon. The user immediately signs in. Then, the user attempts to change the password. But the password change fails. You check the current configuration and find the following configuration password policy settings:  

+ The “Enforce password history” setting is set to 1.  
+ The maximum password age is set to 180.  
+ The minimum password age is set to 1.  
+ Password complexity is enabled.  
+ Store passwords using reversible encryption is enabled.  

The user tries several more times, including trying brand new passwords. But he can’t change it. You need to ensure that the user can change their password immediately. What should you do?  
[ ] Disable storing passwords with reversible encryption.  
[x] Set the “Enforce password history” setting to 0.  
[ ] Configure the user account so that the user is forced to change their password at next logon.  
[x] Disable password complexity.  

[explanation]  
When a minimum password age is configured, a user cannot change their password until that minimum password age interval has elapsed. This makes it harder for users to reset their password several times in a row so that they can loop back to their original password (thus avoiding an actual password change). When an administrator resets a password, it is a good practice to force the user to change their password at next logon. This ensures that the minimum password age setting doesn’t impact their password change and it also ensures that the administrator does not know their password.  
[explanation]  

---

## Checkbox

You are the system administrator for Contoso Ltd. You use the New-ADUser -Name “Jay Hamlin” -Path “OU=Contractors,DC=contoso,DC=com” -Department “IT” command to create a new user. However, after running the command, you notice that the user account is disabled. Which parameter should you use with the New-ADUser command to ensure that newly created users are not disabled?  
[ ] -Enabled  
[x] -ChangePasswordAtLogon  
[ ] -AccountPassword  
[x] -Credential  

[explanation]  
When you create a new user account, the account will be disabled unless a password is set. The -Credential parameter is used to specify credentials to perform the new user creation task. You need to use the -AccountPassword parameter to set the password, along with a secure method of specifying the password such as -AccountPassword (Read-Host -AsSecureString “Password?”).  
[explanation]  

---

## Checkbox

You are the server administrator for Woodgrove Bank. The desktop support team requests access to Group Policy. The team presents the following requirements:  

+ They need to be able to create new GPOs.  
+ They need to be able to edit the GPOs that they create.  
+ They need to be able to delete the GPOs that they create.  
+ They must not be able to edit or delete GPOs that they did not create.  

You need to delegate administrative access to the desktop support team to meet the requirements while adhering to the principal of least privilege. What should you do?  
[x] Add the user to the Group Policy Creator Owners group.  
[ ] Modify the domain permissions to that the desktop support team has “Read all properties”, “Write all properties”, and “Delete” permissions for “groupPolicyContainer” objects.  
[ ] Add the user to the Domain Admins group.  
[ ] Add the user to the Server Operators group.  

[explanation]  
The Group Policy Creator Owners group gives the desktop support team the permissions to create, edit, and delete GPOs. However, they will not be able to modify or delete GPOs that they did not create.  
[explanation]  

---

## Checkbox
   
You are troubleshooting a Group Policy issue. A GPO isn’t applying the correct computer setting to a single computer. You decide to use the Process Monitor tool to monitor changes to the registry. You need to filter the results of the captured data to minimize the number of changes you review. Which registry hive should you target for your review?  
[ ] HKEY_CURRENT_CONFIG  
[ ] HKEY_CURRENT_USER  
[x] HKEY_LOCAL_MACHINE  
[ ] HKEY_USERS  
[ ] HKEY_SYSTEM  

[explanation]  
Computer-based settings are stored in the HKEY_LOCAL_MACHINE registry hive. The HKEY_SYSTEM hive does not exist.  
[explanation]  

---

## Checkbox

You have a GPO that create shortcuts to shared folders on the desktop of client computers. The company deploys OneDrive for Business and migrates all data to OneDrive. You remove the GPO link for the GPO. However, users report that the shortcuts are still on their desktop. You look at the current configuration and find the following:  

+ The GPO uses Group Policy preferences to set the shortcuts.  
+ The GPO security filter is set to Authenticated Users.  
+ The GPO has user and computer settings enabled.  

You need to ensure that the shortcuts for the shared folders are removed. What should you do?  
[ ] Remove the Authenticated Users group from the GPO’s security filter.  
[ ] Disable the user settings on the GPO.  
[ ] Disable the computer settings on the GPO.  
[x] Update the GPO by removing the shortcuts from the preferences and then relink the GPO.  
[ ] Delete the GPO.  

[explanation]  
To remove a GPO preference item, you need to configure the desired setting (even if blank/empty) and then link the GPO to the target users or computers. Otherwise, the preference items will remain behind. Optionally, users can individually remove the shortcuts. However, that degrades the user experience and requires many people performing the same task.  
[explanation]  

---

## Checkbox

You are troubleshooting a network issue. You find a fix that you can deploy by using a GPO. You implement the user-based setting in a GPO and link it to the OU with all the users. Now, you need to guide users to get Group Policy refreshed. Which two options should you present to the users? (Choose two. Each answer presents an independent solution.)  
[ ] Disable the background refresh for Group Policy.  
[x] Have the users sign out and sign back in.  
[ ] Have the users wait at least 60 minutes.  
[ ] Have the users wait at least 90 minutes.  
[x] Have the users wait at least 120 minutes.  

[explanation]  
User-based GPOs are applied at sign-in and at the background refresh interval. The background refresh interval, by default, is set to 90 minutes. There is a random offset of up to 30 minutes. Thus, to ensure that all users have a background refresh, the wait should be 120 minutes.  
[explanation]  
