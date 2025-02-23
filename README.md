# Malware Analysis Lab

Malware is a significant threat to computer systems, making malware analysis a crucial function of cybersecurity. To better understand malware and protect against it, I am creating a malware analysis lab using VirtualBox, Windows 10, and Flare VM. The purpose of this lab is to analyze malware in a safe and controlled environment. Using these tools, I will be able to identify and dissect malware in-depth, catalog any malicious activity, and formulate effective methods of detection and removal. This documentation outlines my process of creating and using the malware analysis lab, as well as the tools and techniques used.

### Goals🏆
- The main goal of this lab is be to gain practical experience in analyzing different types of malware. I can achieve this by testing and analyzing various malware samples, including viruses, trojans, ransomware, and others.
- To understand the behavior of malware, how it works and how to prevent it from causing damage.
- To be able to develop practical and effective techniques for detecting and removing malware.
- Staying up-to-date with the latest malware threats
  

⚠️ I want to clarify that the following documentation is not intended to serve as a comprehensive, step-by-step guide for the lab that I have created. It is rather a record of my personal notes and observations on the lab⚠️


### Tools Used🔨

Oracle VirtualBox: I used VirtualBox to set up isolated virtual machines for malware analysis in a controlled environment. This allows me to run malware without the risk of infecting my host machine or network.

Windows 10 ISO: This tool can be used to create a fresh and up-to-date installation of Windows 10 on a virtual machine, which i configured to use to analyze malware behavior.

FlareVM: FlareVM is a customized virtual machine explicitly designed for malware analysis. It includes various malware analysis tools and utilities pre-installed, such as debuggers, disassemblers, and scripting engines.

PeStudio: I used this to examine executables and identify characteristics commonly associated with malware, such as packers or obfuscation techniques.

Wireshark: I use Wireshark to capture and analyze network traffic to detect suspicious behavior, such as network connections to command-and-control servers or evidence of data exfiltration.

### Program Walk-Thru🚶🏽‍♀️
<p align="center">
Using a disk capacity of at least 80 GB and memory of at least 4 GB😭 (lots of storage)

<p align="center">
After completely installing Windows 10, I went to Devices and clicked "Guest Additions CD image"

<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/cd484b29-fce4-4b83-882c-f4b441333908/>
</p>

<p align="center">
After rebooting the system, I disable Windows Updates, Disable Windows Defender, Disable Tamper Protection and any Anti-Malware solution.

<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/8e52405f-3c21-4aff-9164-4ca3d87dc1c3/>
</p>

<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/a03aba2b-07af-4cec-b130-a20647041b52/>
</p>


<p align="center">
Took a VM snapshot so that I can always revert to a state before FLARE VM installation.

<p align="center">  
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/880a539d-a426-4d7f-8f41-51149574c0a9/>
</p>

<p align="center">
Shut down the machine so that I can change a few of the settings.
<p align="center"> 
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/a3de6de2-7323-4a37-b584-8a09c766e3c6/>
</p>

<p align="center">
  A few settings needed to be ajusted such as display and the processor.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/ec39cf95-f29c-4c2b-a150-3a253a355ced/>
</p>  

<p align="center">
  I get back into the vm and install a power shell script. and put it into a folder named "flare". (I moved it into the folder)
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/6d1b9f64-f415-471b-a4e4-0059a92cca85/>
</p>

<p align="center">
Then went into powershell as an administrator
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/32e0963d-cbc2-4a28-8e10-845facb63103/>
</p>

<p align="center">
This is were I installed flare VM
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/ee588fce-9a2b-4edb-b9b9-be40645e8d2f/>
</p>

<p align="center">
Then we wait for 3 hours...
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/c4dfa280-bfa1-462e-bed1-8282e5cafc29/>
</p>

<p align="center">
3 HOURSSS!!!
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/9ed05e36-a4aa-483a-93c9-30f617b13070/>
</p>

<p align="center">
After flare was completly installed, It rebooted on its own then prompt me to click enter. Then I created another snapshot after installing the flare becouse I dont want to lose eveything I just did.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/97923b84-e2a0-4bbb-9727-6148d8f711b6/>
</p>

<p align="center">
This is were all the fun begins😁 I downloaded a malware file online to put onto the virtual machine.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/e4546bbf-f69f-4ca2-8dda-10e645eef2d0/>
</p>

<p align="center">
Now lets turn the virtual machine network to Host-Only Adapter so I dont destroy my cumputer.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/dbe889a1-7009-4970-b2ea-20d138ade863/>
</p>

<p align="center">
Note: Static analysis examines files for signs of malicious contents, including strings, file names, hashes, domains, IP addresses, and file header data. Static analysis provides a first-step into dissecting and examining malware(in other words looking/identifying malware👀)

<p align="center">
I tried a few different tools to become fimilier with them and what they do when it comes to analyzing static malware. VirusTotal analyzes files and URLs for viruses and other types of malicious content. Used to flag malicious files and programs. 
<p align="center">  
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/6166817f-16bd-466f-8172-baa5b0f1f680/>
 </p> 
<p align="center">  
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/ebed6238-d3f2-411c-aedf-e8fb88a5c9fd/>
  </p>
<p align="center">  
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/1cc359e2-3087-49e8-a7d2-b3b38c069546/>
</p>

<p align="center">
But Pe-Stu-di-o...
 <p align="center"> 
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/fa889688-b080-49f4-8037-58b3ce75b185/>
</p>

<p align="center">
Pestudio is all in one. This tool allows me to  easily spot the functionalities commonly used for malicious activities by attackers(Me🤫).
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/1c5a3d58-6a21-48ca-a021-0f21a5257dff/>
</p> 

<p align="center">
Note: Dynamic analysis provides more detail into how the malware operates. A safe environment, called a sandbox, is used to examine what happens when malware is executed.
<p align="center">
Now I started to do some analyze dynamic malware. Process Monitor or ProcMon allows me to observe, view, and capture Windows file and system activity in real-time. 
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/304d0855-9905-4582-b90c-67caada0724b/>
</p> 

<p align="center">
I used Wireshark to check network activity since malware steals data and sends it to the attacker.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/f949136a-fee3-43f2-bd40-785a3a888fd6/>
</p> 

<p align="center">
Completed!!!😁

### Completion thoughts: 
This lab was fun and interesting to complete. I acquired several techniques and tips to detect signs of malware during my lab session. It was a brief and straightforward exercise, and I plan to add different types of malware, such as ransomware, trojans, bots, and rootkits to expand my knowledge in identifying various malicious threats.

Resources📚

https://github.com/ytisf/theZoo

https://letsdefend.io

https://youtu.be/USNOmFcebcU?si=BU_I8p7mmjN53w39
