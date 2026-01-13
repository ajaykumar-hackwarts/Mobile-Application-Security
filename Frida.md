Frida is a open source dynamic instrumentation toolkit used to watch and change that how an app behaves when it is running without the source code. 

For installing Frida you should install python. 

Steps to run the Frida server. 

- adb(Android debug bridge) root : Gives the root permission.
- adb push ("files") /data/anywhere : Copies files from PC and writes it to Android mobile with our desired locations. 
- adb shell : This opens a android device terminal from the pc.
- su : switch users from normal to admin (Does not work on non-rooted device).
- chmod 777 (file name) : (change mode-permission) (read, write and execute with owner, group and others).
- ./file name  : It will run this file.

Hooking : Intercepting a program calls to alter its behaviour or monitor activity.  

Invoking : Calling a method so the method will be executed. 

After running the we can do many things like 

## Info about the apps :

frida-ps -Uai 

frida-ps: Shows you the apps.

-U: Looks at devices connected by USB.
-a: Shows all apps, not just yours.
-i: Gives you more info like the app’s ID and name


## Injecting scripts :

- Frida -U -f app_package_name -l script.js
- Frida -U -n app_package_name -l script.js

Frida - tool
- -U    - USB/emulator
- -f    - start the app and attach
- -n    - attach on the running app
- -l    - load the script

## Printing : 

Java.perform(function() {

 console.log(‘Hello world’);

     // Do your magic here 
});

## Invoking : 

Java.perform(function() {

var classname = Java.use("packagename.classname");

classname.staticmethod();
 
});

## Changing the value of static variable : 

Java.perform(function() {

var classname = Java.use("packagename.classname");

classname.variable.value = (value);
 
});

## Invoking a method on the Non static class : 

Since it is a non-static class we should create an object to use it. 

Java.perform(function() {
    var classname = Java.use("packagename.classname");
    var obj = classname.$new();
    var res = obj.methodname();
    console.log("Flag" + res);
});

obj = object(new instance) 

$new() = keyword to create new object. 


## Invoking Methods on an Existing Instance : 

When an android application starts the system creates an instance of the mainactivity.


Java.performNow(function() {

 Java.choose('packagename.classname', {

   onMatch: function(instance) {

   console.log(instance found);
   
   instance.methodname();
      
  },
  
  onComplete: function() {}
    
  });
  
});

Java.performNow : Used to run the code immediately after the VM is started. 

onMatch: It's callback method that runs each existing instance in the specified class. 

onComplete : It perform as a clean up action after the Java.choose has finished. 


## Passing object as an arguement : 

Java.performNow(function() {
  
   Java.choose('packagename.classname', {
  
  onMatch: function(instance) {
  
  console.log("Instance found");

  var new = Java.use("packagename.newclassname");
  
  var new_obj  = checker.$new();   
  
   new_obj.x.value = 1337; 
   
   new_obj.y.value = 1200; 
   
   instance.methodname(new_obj);  

  },
        
  onComplete: function() {}
  
  });
  
});

newclassname : new class name

new_obj : new object


## Hooking : 

Java.perform(function() {

var.cls = Java.use("packagename.classname");

cls.methodname.implementation = function(){

var value = this.methodname;

console.log("The value" +value);

return value;

};

});

implementation : Keyword used to replace the java code. 

### Native Code : 

It is a C or C++ code which can be used in the Java application. In android we can use the native code by the NDK(Native Development Kit). 

### Why native code ? 

Java source code --> Bytecode(Using Compiler) --> Machince Code(JVM) --> CPU   : Portable, safe, optimized, independent. But not faster than native code. 

C/C++ source code --> Machince Code (Using Compiler) -->  CPU   : faster than java code. 

Native code doesn't need virtual machine to convert source code to machine code hence it is faster that java code and it is very useful in the  low-level access such as video/audio processing, graphics, encryption etc. 




Decryption :

Java.perform(function() {                  
var decrypt = Java.use('PuGMAu.QumH');      
console.log("Decrypted :", decrypt.TUDsyZfyyu("MAVYx7WhNRA9Eg==\n", "eEAKgPDzfVc=\n"));});     


- Java - Works with the java's code 
- .perform -> run the code after all java classes is loaded 
- function () -> keyword to run the function.  
- var -> keyword to create varible 
- decrypt -> variable name 
- Java.use -> get access to the java class so it can hook the method, 
- PuGMAu.QumH -> class name
- console -> outpur screen
- .log -> write
- TUDsyZfyyu -> method name
- "MAVYx7WhNRA9Eg==\n", "eEAKgPDzfVc=\n" -> 2 parameters



 
