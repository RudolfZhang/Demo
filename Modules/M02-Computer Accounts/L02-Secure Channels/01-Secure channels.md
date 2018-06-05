## Secure channels

**A secure channel is used for all computer communications.**

The NetLogon service uses the computer credentials to log on to the domain, which establishes the *secure channel* with a domain controller. This secure channel between a computer and a domain controller is used for all communication with the domain.

If the computer is unable to sign in successfully, the secure channel is not established. The effect is similar to when a user enters the wrong user name or password. In both circumstances, the user is not able to authenticate to the domain.

**Know the symptoms of a broken secure channel.**

A *broken* computer account manifests itself with a variety of symptoms, error messages, and event-log entries. The most common signs of computer account problems are **sign-in messages** and **event log messages**.

**Sign-in messages**

![Screenshot of a user login error: The trust relationship between this workstation and the primary domain failed. ](/Modules/Linked_Image_Files/3.2.1.png)

Messages at sign-in indicate that a domain controller cannot be contacted, that the computer account might be missing, that the password on the computer account is incorrect, or that the trust relationship (also called *the secure relationship*) between the computer and the domain has been lost.

**Event log messages**

**![Screenshot of NetLogon Event ID 5722: The session setup from the computer failed to authenticate. Access denied. ](/Modules/Linked_Image_Files/3.2.1-2.png)**

Error messages or events in the event log indicate similar problems or suggest that passwords, trusts, secure channels, or relationships with the domain or a domain controller have failed.
