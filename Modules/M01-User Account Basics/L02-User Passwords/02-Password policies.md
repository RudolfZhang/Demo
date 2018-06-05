## Password policies

![Screenshot of the GPMC with the Password Policies node highlighted. GPOs discussed in the text (such as Enforce password history) are shown. ](../..\Linked_Image_Files\1.2.2.png)

When www securing your user accounts use the [Password Policy](https://technet.microsoft.com/en-us/library/cc757692(v=ws.10).aspx#w2k3tr_sepol_accou_set_kuwh) settings. You should configure the properties of the passwords that users might select. Use these settings to make sure users don’t select simple <g>passwords,</g> or passwords that have been recently used. You can only have one standard password policy in a domain.

<table>
<tbody>
<tr>
<td width="229" valign="top">


**Setting**

</td>
<td width="271" valign="top">


**Description**

</td>
<td width="236" valign="top">


**Values**

</td>
</tr>
<tr>
<td width="229" valign="top">


**Enforce password history**

</td>
<td width="271" valign="top">


The number of unique, new passwords that must be associated with a user account before an old password can be reused.

</td>
<td width="236" valign="top">


Default setting: 24 passwords 


</td>
</tr>
<tr>
<td width="229" valign="top">


**Maximum password age**

</td>
<td width="271" valign="top">


Number of days that a password can be used before the user must change it. 

</td>
<td width="236" valign="top">


Recommended setting: 42 days 

</td>
</tr>
<tr>
<td width="229" valign="top">


**Minimum password age**

</td>
<td width="271" valign="top">


Number of days that a password must be used before the user can change it.

</td>
<td width="236" valign="top">


Default setting: 1 day

</td>
</tr>
<tr>
<td width="229" valign="top">


**Minimum password length**

</td>
<td width="271" valign="top">


Minimum number of characters that a user’s password must contain.

</td>
<td width="236" valign="top">


Default setting: 7 characters 

High security: 15 characters 

</td>
</tr>
<tr>
<td width="229" valign="top">


**Complexity requirements**

</td>
<td width="271" valign="top">


Required password characteristics. Don't disable. 

</td>
<td width="236" valign="top">


Does not contain your name or user name. Has at least six characters. Contains characters from different charsets **<sup>[1]</sup>** 

</td>
</tr>
</tbody>
</table>


<sup>[1]</sup>Contains characters from 3 of these 4 for charsets: Uppercase letters [A–Z]; Lowercase letters [a–z]; Numerals [0–9]; Special, non-alphanumeric characters, such as !@#)(*&^% .
