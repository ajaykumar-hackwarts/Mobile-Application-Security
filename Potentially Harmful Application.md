Potentially Harmful Application is an Android app which can harm an user or device if it is installed. 

## 1. Ransomware : 

- Code that takes partial or complete control of the device or encrypt the data and lock out the user and demanding ransome to get the device's or data's full access.

- It will either encrypt the user's file write that in some where hidden and delete the original file or lock the device by creating an overlay by hiding the home and back button and will ask for ransom to give the access. 

Permission needed : 
- BIND_DEVICE_ADMIN : To lock the device and reset password.
- WRITE_EXTERNAL_STORAGE : To gain access to the users file and encrypt them. 
- SYSTEM_ALERT_WINDOW : To display an overlay like "your screen is locked like that and give ransom to get back the access.
- RECEIVE_BOOT_COMPLETED : To start the background activity when it is restarted.


## 2. Backdoor : 

- Code that executes the unwanted, remotely controlled code in the device and to malicious activity inside that at the install time.

RAT(Remote Access Trojan) Backdoor : 

- Install itself on the device and opens a hidden backdoor and allows an attacker to remotely control the system.

- After Installing it can perform any PHA like spyware like it can access the datas and can exfiltrate it or privilege_escalation block the device and ask for ransom etc...


DCL(Dynamic Code Loading) Backdoor : 

- It's a technique where it doesn't contain all the malicious code at the install time instead it download and executes malicious code when running dynamically. 

Remote execution code is the code which allows command or instruction sent from one system and executed on the other system over the internet.

These remote execution connection are of four types 
- Socket Connection()     : Direct network connection that sends command to other system in real time. 
- C2(Command and Control) : Server has the direct connect with the system and demands a work and system will do it. 
- FMS(Firebase messaging service)/GCM(Google cloud messaging service)  : A push notification service where a server sends a message to a system without them running or opening. 
- Receiver           : An event based mechanism which is triggered when an event is happened. 


## 3. Trojan :     

Application which pretends to be a legitimate application but it secretly perform harmful activity after installation.

Red falgs : 

- Application is asking for an unwanted permission which is not at all related to the application behaviour example : Flash light application asking for device admin permission.
- Application hiding its icons using the setComponentEnabledSetting by using this it can disable or enable any component without uninstalling the application.

## 4. Riskware : 

The application masks themselves as the legitimate application and uses techniques such as obfuscation, dynamic code loading or cloaking to reveal malicious content. 

Cloaking : Based on the specific condition the application change it's beheviour

Server Side Cloaking : The server hides it's real content or functionality and only reveals to a specific user by a conditions. 

- IP-Based/Location-Based Cloaking : Shows different content on the application depending on the vistor's IP address and the physical location.
- Time-Based Cloaking : Shows different content based on the different time example : dark mode in instagram.
  
MMP : Third party analytics platform used by the mobile apps to track, measure and attribute installs. It tells the developer from which ad or campaign the user has installs the app and after installing what did he do first. Popular MMPs are Appsflyer, Adjust, Branch, Singular and Kochava. 

MMP cloaking :  App behaves differently for MMP tracking and it behaves differently for the real users.


## 5. Spyware : 

- Malicious Code which collects and exfiltrates user's PII(personal identifiable information) to the third party url
- It can collect contacts, sms, call logs, calender, documents, camera and clipboard data.


## 6. Privilege_escalation : 

- Code which gain the unortherised access and takes over the full control of the device. 

To do Privilege_escalation app should have these permissions. 

BIND_DEVICE_ADMIN
SYSTEM_ALERT_WINDOW  
WRITE_EXTERNAL_STORAGE
BIND_ACCESSIBILITY_SERVICE

It will have the admin permission and tried to lock the user and reset the password and perform some malicious action like take over the complete device. 


## 7. Toll fraud : 

- Code which subscribes to the paid services or purchases without the users permission. 

READ_SMS
RECEIVE_SMS
BIND_NOTIFICATION_LISTENER
CHANGE_WIFI_STATE 

Using READ_SMS reads all the sms stored like otp, carrier & subsrciption related messages and using RECEIVE_SMS it can see all the sms before users sees it and BIND_NOTIFICATION_LISTENER can read and hide the notification and using the CHANGE_WIFI_STATE it will change the network settting to mobile instead of WIFI as to subscribe to premium calls it should have the mobile network. 


## 8. Rooting : Use to gain access to the root system of the Operating system. 

Legitimate purpose : Remove Bloatware (pre-installed apps that can't be uninstalled easily), Personalisation, Installing custom ROM. 

Threat : App gets the admin power so they can take the full control of the system. 