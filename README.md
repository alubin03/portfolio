# Malware Analysis Lab

Malware is a significant threat to computer systems, making malware analysis a crucial function of cybersecurity. To better understand malware and protect against it, I am creating a malware analysis lab using VirtualBox, Windows 10, and Flare VM. The purpose of this lab is to analyze malware in a safe and controlled environment. Using these tools, I will be able to identify and dissect malware in-depth, catalog any malicious activity, and formulate effective methods of detection and removal. This documentation outlines my process of creating and using the malware analysis lab, as well as the tools and techniques used.

### Goals🏆
- The main goal of this lab is be to gain practical experience in analyzing different types of malware. I can achieve this by testing and analyzing various malware samples, including viruses, trojans, ransomware, and others.
- To understand the behavior of malware, how it works and how to prevent it from causing damage.
- To be able to develop practical and effective techniques for detecting and removing malware.
- Staying up-to-date with the latest malware threats
  
### Tools Used🔨

- VirtualBox Installer
- Windows 10 ISO file
- Flare-VM

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
Then went to the powershell as admin mode  
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
After it completly installed the flare. reboots on its own then prompt me to click enter. Then I created another snapshot after installing the flare becouse I dont want to lose eveything I just did.
<p align="center">
<img src=https://github.com/alubin03/Malware_Anaysis_Lab/assets/141780397/97923b84-e2a0-4bbb-9727-6148d8f711b6/>
</p>
   
  
### Completion thoughts: 


Resources:

https://letsdefend.io
