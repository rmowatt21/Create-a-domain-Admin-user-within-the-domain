CREATING USER NAMES IN ACTIVE DIRECTORY

Go into your DC-1 VM. Your user name and password should have the "MYDOMAIN.COM\LABUSER" as the user
and the password. After you're log in, go to start menu box and type in "active directory domain users"
<img width="614" alt="image" src="https://github.com/user-attachments/assets/7d21c3ea-8aa4-43dd-a779-d78d7defa249">

In active dirctory domain services(ADUC)we're going to create a new organization unit(OU) and we're going to 
name it "_EMPLOYEES". Right click inside the ADUC box were it say's mydomain.com. Go to new and toggle over to
Oganizational Unit. Click inside
![image](https://github.com/user-attachments/assets/d41e8422-1532-4375-af04-8e9dadbb4580)
![image](https://github.com/user-attachments/assets/e6313205-9571-4ede-bcbe-965547fa91f2)

We going to create a new user name in the "_ADMINS" named "Jane Doe" with the username of 
"Jane_admin"/ password:Password1. Right click on "_ADMINS" scroll to new and toggle over to "User".
In the new object box type in "Jane Doe" for first and last name. The user logon name: "Jane_admin"
![image](https://github.com/user-attachments/assets/926b4adf-1624-46ca-abad-cef0ccb9080b)
<img width="328" alt="image" src="https://github.com/user-attachments/assets/a65a640e-cea7-452f-8729-55d196e0235f">

The "jane Doe" has been accepted as a domain user just yet. We have to add the name in the secruity group first to 
complete the process. Do do that we right click on the user name "Jane Doe" go to properties. Go to the "Member of" tab,
click add next to remove
![image](https://github.com/user-attachments/assets/aa76f892-94bd-4c3c-9fbe-438edd7b5f4c)
![image](https://github.com/user-attachments/assets/4f827337-360b-45e4-9c0b-ca8895c15338)

In the select groups box at the bottom enter "domain" and click "check names" on the right of the box. Go to
"Domain Admins" and double click that box.
![image](https://github.com/user-attachments/assets/eab7e0e9-fd90-4d12-b3f4-37b0493c66f1)

to see if it works. Log out and log back in as Jane_admin user with the password. 

Login to Client-1 as the original local admin (labuser) and join it to the domain (computer will restart).
First go to start > settings > systems > About > Rename this PC (advanced) 
> system properties, change > Comptuter Name/Domain changes >
> Member of (mydomain.com) 
![image](https://github.com/user-attachments/assets/fbaa979d-deed-45f4-abd9-0558d7e320ef)


















