# Obfuscation : 

**Definition** : The process of modifying source/machine code to make it difficult to humans to understand and reverse-engineer, without altering its original functionality.

**Why Do we Need it** : To protect intellectual property like business logic, prevent modifying and secure sensitive data from reverse engineering. 

**Threats** : Hiding a malicious code and performing some malware without users knowledge and make it tough to reverse engineer.

**Tools** : 

- **Progaurd/R8 :** It is developed by Guardsquare company. It's main purpose is to shrink, optimize, and obfuscate Java and Kotlin bytecode. And it will only do the basic thing a skilled analyst can still read the logic. 

- **Dexgaurd :** It is developed by Guardsquare company too. It provides military level hardening encrypts actual strings and classes so they cannot be read statically at all. Prevents the app from running on rooted devices where tools like Frida can attach.

# De-Obfuscation : 

**Definition** : The process of reversing the obfuscated code. 

**Why Do we Need it** : To read, understand, and analyze compiled apps when the original source code is unavailable and to find the vulnerabilities and rectify it.

**Threats** : It can compromises security controls, leaks hardcoded secrets. 

**Tools** : 

- JADX(Dex to Java Decompiler) : Open source command line GUI tool that converts android DEX and APK files into readable Java files.

- Frida : Dynamic instrumentation app which helps to peek inside the running app and see hidden code when static decompilers fail.

- Ghidra : Open source tool developed by NSA to read/deobfuscate raw C/C++ native code (like .so files) when standard Java decompilers can't reach it.


## Packing  : 

- Wrapping an app's code inside an encrypted shell to completely hide it from view until the app actually runs. Tools like Progaurd/R8, Dexgaurd can be used for this. 

## Unpacking : 

- To process of removing or bypassing an app's protective encryption shell to reveal and extract the hidden original code.

**ApkTool** : Apktool was created by Ryszard Wiśniewski. It is an open-source tool used to unpack app's configuration files and resources into readable text. 
