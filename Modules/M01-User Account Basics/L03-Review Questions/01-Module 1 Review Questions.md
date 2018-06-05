## Multiple Choice  
<<display_name:Question 1; max_attempts:2; showanswer:never; weight:1.0>>
Which PowerShell command can be used to create a new user? 
( ) Enable-ADAccount  
( ) New-ADAccount  
(x) New-ADUser  
( ) Set-ADUser  
or New-ADAccount  

[explanation]  
<b>New-ADUser</b>. The New-ADUser command can be used to create a new user. For example, New-ADUser -Name "Ed Meadows".   
[explanation]  

---

## Multiple Choice
  
Which setting ensures users do not reuse the same password too often?  
( ) Complexity requirements  
(x) Enforce password history  
( ) Maximum password age  
( ) Minimum password age  

[explanation]  
<b>Enforce password history</b>. The Enforce password history setting determines the number of unique, new passwords that must be associated with a user account before an old password can be reused.   
[explanation]  

---

## Multiple Choice
  
Which setting can be used to set the number of failed logon tries that are allowed before a user account is locked out?  
( ) Account lockout duration  
(x) Account lockout threshold  
( ) Complexity requirements  
( ) Reset account lockout counter  

[explanation]  
<b>Account lockout threshold</b>. The Account lockout threshold setting determines the number of failed logon tries that are allowed before a user account is locked out. Set this value high enough to allow for mistyped passwords, but low enough to minimize the chances of a successful brute force attack on a password.  
[explanation]  

---

## Multiple Choice

Your organization’s administrators need to use more stringent passwords. Which of the following should you implement?  
( ) Complexity requirements  
(x) Fine-grained password policies  
( ) Password permissions  
( ) User profile redirection  

[explanation]  
<b>Fine-grained password policies</b>. You can use fine-grained password policies to specify multiple password policies, and to apply different password restrictions and account lockout policies to different sets of users in a single domain. For example, administrators may have different password requirements that are stricter than the policies for a user.   
[explanation]  

---

## Multiple Choice

What of the following AD DS attributes represents a user’s logon name?  
( ) cn  
( ) DisplayName  
( ) Name  
(x) sAMAccountName  

[explanation]  
<b>sAMAccountName</b>. When users sign in, they use their sAMAccountName. In some cases, the value of sAMAccountName can match the value of other attributes.  
[explanation]  

---

## Multiple Choice

Your company has experienced several accounts being locked out. You suspect that a denial of service (DoS) attack is responsible.  Which of the following settings should you use to temporarily halt the attack?  
( ) Set the account lockout duration to 0.  
(x) Set the account lockout threshold to 0.  
( ) Set the account lockout duration to 999.  
( ) Set the account lockout threshold to 999.  

[explanation]  
<b>Set the account lockout threshold to 0</b>. Setting the account lockout threshold to 0 will prevent accounts from being locked out which temporarily halts the attack.  
[explanation]  

---

## Multiple Choice

You are setting up a new branch office with 25 user accounts. Much of the user account information is the same, so you have created a user template. When you run the New-ADUser command which parameter should you use to pass the template?  
(x) -Instance  
(  ) -Template  
(  ) -Path  
(  ) -Settings  

[explanation]  
<b>-Instance</b>. The Instance parameter can be used to create a new user from a template.   
[explanation]  

---

## Multiple Choice

Brad is a member of several groups. Which of following can be used to view his overall password permissions?  
(  ) Additive group permissions  
(  ) Administrator account permissions  
(  ) Fine-grained password settings  
(x) Resultant password permissions  

[explanation]  
<b>Resultant password permissions</b>. You can use the ADAC to view a user’s resultant password permissions and ensure they have the correct permissions.   
[explanation]   

---

## Multiple Choice

You are creating a new user using Windows PowerShell. You have used New-ADUser and Set-ADAccountPassword. Which command should you use next?  
(x) Enable-ADAccount  
( ) Enable-ADObject  
( ) Set-ADAccount  
( ) Set-ADUser  

[explanation]  
<b>Enable-ADAccount</b>. Without this command the user account will be disabled.  
[explanation]  

---

## Multiple Choice

You are creating a new user but the password (Password) keeps throwing an error. What is likely the problem?  
( ) You have to create the user before assigning the password.  
(x) The password does not meet complexity requirements.  
( ) You do not have permission to create a user.   
( ) The user already has a password.   

[explanation]  
<b>The password does not meet complexity requirements</b>. Even when you are creating a new user where the password will be changed, the password must meet complexity requirements.  
[explanation]  