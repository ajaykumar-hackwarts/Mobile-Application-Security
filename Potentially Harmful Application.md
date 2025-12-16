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

- It's a technique It doesn't contain all the malicious code at the install time instead it download and executes malicious code when running dynamically. 




3. Trojan/Riskware
4. Spyware
5. Privilege_escalation
6. Toll fraud
7. Rooting


1. Ransomware : 
