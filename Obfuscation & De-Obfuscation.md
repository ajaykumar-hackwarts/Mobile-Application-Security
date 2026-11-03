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

- JADX(Java to Dex Decompiler) : Open source command line GUI tool that converts android DEX and APK files into readable Java files.

- 
