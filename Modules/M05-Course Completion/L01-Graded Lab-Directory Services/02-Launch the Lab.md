## Lab: Directory Services

These are the tasks in your graded lab. Be sure you can complete the tasks in the time allotted and that you ready to be tested. The tasks will be repeated in the testing environment.

**TASK 1**: Create a new top level Organization Unit (OU) named Merger in the <g>ADATUM</g> domain. In the Merger OU, create a security group with a Global scope named Auditors.

**TASK 2**: Create a new user account for Jim Healy with the following properties.

*    User logon name: **<g>jimh</g>**
*   Password: **Pa55w.rd**
*   Job Title: **Auditor**
*   Group: **Auditors**

**TASK 3**: Create a fine-grained password policy and apply it to the Auditors group.

*    Name: **Auditors**
*   Precedence: **10**
*   Minimum password length: **10**
*   **Enforce lockout policy with 10 failed logon attempts allowed**

**TASK 4**: Add a DHCP reservation to the London Office DHCP scope for LON-CL1.

*   Name: **LON-CL1**
*   IP Address: **172.16.0.201**
*   MAC Address: **00-15-5D-A3-97-61**
*   Support Types: **DHCP**

**TASK 5**: Create a new organizational unit named MyComputers in the root of the <g>ADATUM</g> domain so that computer accounts are by default created in the MyComputers OU when computers are joined to the domain.

**TASK 6**: Edit the <g>these User Configuration</g> Personalization settings.

*   Enable Screen Saver Timeout to 600 seconds.
*   Password protect the screen saver.



---
## LTI component
### lti_consumer:

###### Enter the LTI ID for the external LTI provider. This value must be the same LTI ID that you entered in the LTI Passports setting on the Advanced Settings page. 
```
LTI ID:xtreme
```

###### Enter the URL of the external tool that this component launches. This setting is only used when Hide External Tool is set to False.
```
LTI URL: https://labs.microsoftlabsonline.com/mslconnection/authlti 
```
###### Add the key/value pair for any custom parameters, such as the page your e-book should open to or the background color for this component.
######  Ex. ["page=1", "color=white"]
```
Custom Parameters:["content_title=AZURE202x-MPP"]
```

###### Enter the text on the button used to launch the third party application. 
###### This setting is only used when Hide External Tool is set to False and LTI Launch Target is set to Modal or New Window. 
```
Button Text:Launch the Graded Lab Environment
```

###### Enter 'inline' if you want the LTI content to open in an IFrame in the current page. 
###### Enter 'modal' if you want the LTI content to open in a modal window in the current page. 
###### Enter 'new_window' if you want the LTI content to open in a new browser window. This setting is only used when Hide External Tool is set to False. 

```
LTI Launch Target:new_window 
```

###### Enter the name that students see for this component. 
###### Analytics reports may also use the display name to identify this component.
```
Display Name:Launch Lab 
```

###### Enter 'true' if this component will receive a numerical score from the external LTI system. 
```
Scored:true 
```
###### Enter the number of points possible for this component.
###### The default value is 1.0. This setting is only used when Scored is set to True. 
```
Weight:1.0 
```
###### Enter 'true' to request the user's email address, otherwise enter 'false'
```
Request user's email:true 
```
###### Enter 'true' to request the user's username address, otherwise enter 'false'
```
Request user's username:true 
```
###### Enter a description of the third party application. 
###### If requesting username and/or email, use this text box to inform users why their username and/or email will be forwarded to a third party application.
```
LTI Application Information:
```
###### Enter the desired pixel height of the iframe which will contain the LTI tool. 
###### This setting is only used when Hide External Tool is set to False and LTI Launch Target is set to Inline.
```
Inline Height:800
```
###### Enter the desired viewport percentage height of the modal overlay which will contain the LTI tool. 
###### This setting is only used when Hide External Tool is set to False and LTI Launch Target is set to Modal. 
```
Modal Height:80
```
###### Enter the desired viewport percentage width of the modal overlay which will contain the LTI tool. 
###### This setting is only used when Hide External Tool is set to False and LTI Launch Target is set to Modal. 
```
Modal Width:80
```
###### Enter 'true' if you want to use this component as a placeholder for syncing with an external grading system rather than launch an external tool.
###### This setting hides the Launch button and any IFrames for this component. 
```
Hide External Tool:false
```
###### Enter 'true' to allow third party systems to post grades past the deadline; otherwise enter 'false'
```
Accept grades past deadline:True
```