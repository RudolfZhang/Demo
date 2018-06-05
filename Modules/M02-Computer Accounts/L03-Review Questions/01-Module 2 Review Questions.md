## Multiple Choice

<<display_name:Question 1; max_attempts:3; showanswer:never; weight:1.0>>

You have created OUs for the computers in your organization. Now you would like to automatically redirect all new computers into a NewComputers OU so the IT department will know when new computers have been installed. Which tool should you use?  
( ) Active Directory Sites and Domains	
( ) Active Directory Users and Computers	
( ) ADSIEdit	
( ) dsmod	
(x) redircmp	

[explanation]	
<b>redircmp</b>. You can use redircmp to redirect all new computers to the NewComputers OU. For example, if the OU is in the Adatum.com domain: Redircmp “OU=NewComputers,DC=Adatum,DC=com”	
[explanation]	

---

## Multiple Choice

<<max_attempts:null;>>

Which PowerShell command can be used to create a new computer account?	
( ) Add-ADComputer	
( ) Enable-ADComputer	
(x) New-ADComputer	
( ) New-ADObject	
( ) Set-ADComputer	

[explanation]	
<b>New-ADComputer</b>. The New-ADComputer command can be used to create a new group.	
[explanation]	

---

## Multiple Choice

Aziz has reported he is unable to sign in to the domain. The error message is, “The trust relationship between this workstation and the primary domain failed.” What is likely the problem?		
( ) Bad network connection  
(x) Broken secure channel  
( ) Computer does not have required security updates  
( ) Password policy violations  

[explanation]  
<b>Broken secure channel</b>. This error message indicates the computer cannot establish a secure channel with a domain controller.   
[explanation]  

---

## Checkboxes

Which of the following three things can cause a broken secure channel?   
[x] The computer cannot authenticate because the password is out of sync  
[x] The computer has been inactive for an extended period  
[ ] There is a DNS resolution problem  
[ ] There is a network connection problem  
[x] The operating system was reinstalled  

[explanation]  
The operating system was reinstalled, The computer has not been active for an extended period of time, The computer cannot authenticate because the password is out of sync.  Computer accounts and the secure relationships between computers and their domain are robust. Nevertheless, these scenarios can cause a broken channel.   
[explanation]  

---

## Multiple Choice

To fix a broken secure channel what should you do?  
( ) Disable the computer account and rejoin the computer to the domain.  
( ) Delete the existing computer account and create a new computer account.   
( ) Disjoin the computer account and rejoin the computer to the domain.  
(x) Reset the computer account and rejoin the computer to the domain.   


[explanation]  
<b>Reset the computer account</b>. When the secure channel fails, you should reset the computer account. By default, the netdom reset and Test-ComputerSecureChannel solutions will try to reset the password at the computer and domain level. If successful, a reboot is not required. If not, a reboot is required.  
[explanation]  

---

## Multiple Choice

You are on the domain controller and creating a file for offline domain join. You are using the djoin.exe command. Which parameter will create the computer account in AD DS?  
( ) /localos  
(x) /provision  
( ) /requestodj  
( ) /windowspath  

[explanation]  
<b>provision</b>. The provision parameter will create and configure the computer account for the computer that will be joining the domain.   
[explanation]    

---

## Multiple Choice 

You have identified a problem with a broken channel on LON-CL1. Your first step on the Domain Controller is to right-click LON-CL1 and  
( ) delete the account  
( ) disable the account  
( ) disjoin the account  
(x) reset the account  

[explanation]  
<b>Reset the account</b>. When the secure channel fails, you must reset the computer account.   
[explanation]  

---

## Multiple Choice

Which of the following is not a benefit of pre-staging a computer account?  
( ) Enforces delegated control  
( ) Enforces the group policy settings  
( ) Enforces the OU structure  
(x) Ensures there is not a broken channel  

[explanation]  
<b> Ensures there is not a broken channel </b>. Pre-staging a computer account will not prevent a broken channel.    
[explanation]  

---

## Multiple Choice

A computer changes its password approximately every  
( ) other day  
(x) every 30 days  
( ) every 45 days  
( ) every 60 days  

[explanation]  
<b> every 30 days </b>. A computer changes its password in the domain approximately every 30 days.    
[explanation]  

