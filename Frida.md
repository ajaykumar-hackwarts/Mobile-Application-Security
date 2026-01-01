Frida is a open source dynamic instrumentation toolkit used to watch and change that how an app behaves when it is running without the source code. 

For installing Frida you should install python. 

Steps to run the Frida server. 

- adb(Android debug bridge) root : Gives the root permission.
- adb push ("files") /data/anywhere : Copies files from PC and writes it to Android mobile with our desired locations. 
- adb shell : This opens a android device terminal from the pc.
- su : switch users from normal to admin (Does not work on non-rooted device).
- chmod 777 (file name) : (change mode-permission) (read, write and execute with owner, group and others).
- ./file name  : It will run this file.
