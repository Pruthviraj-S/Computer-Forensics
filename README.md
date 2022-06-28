<p align="left">
<a href="#"><img title="Made in INDIA" src="https://img.shields.io/badge/MADE%20IN-INDIA-green?colorA=%23ff9933&colorB=%23017e40&style=for-the-badge"></a>
</p>

<p align="center">
<a href="#"><img title="dfis" src="https://e-discovery.ng/wp-content/uploads/2021/07/Digital-Forensics-styled.png" width='256'></a> 
<p align='center' style="font-size:48px; font-family: cursive; "> Computer Forensics </p>
</p>

<p align="center">
<a href="https://github.com/Pruthviraj-S"><img title="Author" src="https://img.shields.io/badge/Author-Pruthviraj--S-red.svg?style=for-the-badge&logo=github"></a>
<a href="#"><img title="Open Source" src="https://img.shields.io/badge/Open%20Source-%E2%9D%A4-green?style=for-the-badge"></a>
<a href="#"><img title="Language" src="https://img.shields.io/github/license/Pruthviraj-S/Computer-Forensics?style=for-the-badge"></a>
</p>

# Computer Forensic Reference Data Sets (CFReDS)

## HACKING CASE 
### Scenario:
> On 09/20/04 , a Dell CPi notebook computer, serial # VLQLW, was found     abandoned along with a wireless PCMCIA card and an external homemade 802.11b antennae. It is suspected that this computer was used for hacking purposes, although cannot be tied to a hacking suspect, G=r=e=g S=c=h=a=r=d=t. (The equal signs are just to prevent web crawlers from indexing this name; there are no equal signs in the image files.) 
    
> Schardt also goes by the online nickname of “Mr. Evil” and some of his associates have said that he would park his vehicle within range of Wireless Access Points (like Starbucks and other T-Mobile Hotspots) where he would then intercept internet traffic, attempting to get credit card numbers, usernames & passwords.

> Find any hacking software, evidence of their use, and any data that might have been generated. Attempt to tie the computer to the suspect, G=r=e=g S=c=h=a=r=d=t.

**Any names in the forensic image are fictional and do no refer to real people.**
### Evidences:
* **What is the image hash? Does the acquisition and verification hash match?**
    ```
    Ans: aee4fcd9301c03b3b054623ca261959a, no acquistion hash found.
    ```
* **What operating system was used on the computer?**
    ```
    Ans: Windows XP Professsional
    ```
    ![Que2](/HackerCase%20imgs/que2.png)
    ![Que2_2](/HackerCase%20imgs/que2_2.png)
* **When was the install date?**
    ```
    Ans: Thursday, August 19, 2004 10:48:27 PM UTC
    ```
    * FTK
    ![Que3](/HackerCase%20imgs/que3.png)
    * Autopsy
    ![Que3a](/HackerCase%20imgs/que3_a.png)
* **What is the timezone settings?**
    ```
    Ans: Central Daylight Time
    ```
    * FTK
    ![Que4](/HackerCase%20imgs/que4.png)
    * Autopsy
    ![Que4a](/HackerCase%20imgs/que4_a.png)
* **Who is the registered owner?**
    ```
    Ans: Greg schardt
    ```
    ![Que5](/HackerCase%20imgs/que5.png)
    * Autopsy
    `Refer Que 3 autopsy img`
* **What is the computer account name?**
    ```
    Ans: Mr.Evil w.r.t autopsy, FTK shows N-1A9ODN6ZXK4LQ as computer name.
    ```
    ![Que6](/HackerCase%20imgs/que6.png)
* **What is the primary domain name?**
    ```
    Ans: N-1A9ODN6ZXK4LQ w.r.t autopsy, FTK show Mr.Evil
    ```
* **When was the last recorded computer shutdown date/time?**
    ```
    Ans: Reg Key:- ShutdownTime	REG_BIN	C4 FC 00 07 4D 8C C4 01 , TIME:- 2004-08-27 15:46:33.1092164 Z UTC
    ```
    `Converter: https://www.digital-detective.net/dcode/`
* **How many accounts are recorded (total number)?**
    ```
    Ans: 5, Administrator,Guest,HelpAssistant,Mr.Evil,SUPPORT_388945a0
    ```

* **What is the account name of the user who mostly uses the computer?**
    ```
    Ans: Mr.Evil, 15 logins
    ```
* **Who was the last user to logon to the computer?**

* **A search for the name of “G=r=e=g S=c=h=a=r=d=t” reveals multiple hits. One of these proves that G=r=e=g S=c=h=a=r=d=t is Mr. Evil and is also the administrator of this computer. What file is it? What software program does this file relate to?**

* **List the network cards used by this computer**

* **This same file reports the IP address and MAC address of the computer. What are they?**

* **An internet search for vendor name/model of NIC cards by MAC address can be used to find out which network interface was used. In the above answer, the first 3 hex characters of the MAC address report the vendor of the card. Which NIC card was used during the installation and set-up for LOOK@LAN?**

* **Find 6 installed programs that may be used for hacking.**

* **What is the SMTP email address for Mr. Evil?**

* ***What are the NNTP (news server) settings for Mr. Evil?***

* **What two installed programs show this information?**

* **List 5 newsgroups that Mr. Evil has subscribed to?**

* **A popular IRC (Internet Relay Chat) program called MIRC was installed.  What are the user settings that was shown when the user was online and in a chat channel?**

* **This IRC program has the capability to log chat sessions. List 3 IRC channels that the user of this computer accessed.**

* **Ethereal, a popular “sniffing” program that can be used to intercept wired and wireless internet packets was also found to be installed. When TCP packets are collected and re-assembled, the default save directory is that users \My Documents directory. What is the name of the file that contains the intercepted data?**
* **Viewing the file in a text format reveals much information about who and what was intercepted. What type of wireless computer was the victim (person who had his internet surfing recorded) using?**

* **What websites was the victim accessing?**

* **Search for the main users web based email address. What is it?**

* **Yahoo mail, a popular web based email service, saves copies of the email under what file name?**

* **How many executable files are in the recycle bin?**

* **Are these files really deleted?**

* **How many files are actually reported to be deleted by the file system?**

* **Perform a Anti-Virus check. Are there any viruses on the computer?**

### Refrences

* **CFREDS ARCHIVE FOR DFIS CASES**
    - https://cfreds-archive.nist.gov/

<!-- * **Guide (ONLY SEEE WHEN NEEDED)**
    - https://medium.com/@sshekhar01/cfreds-project-hacking-case-challenge-writeup-6a52883eac0b -->
## Disclaimer
Contents of this repository are only meant for learning the aspects of computer forensics. Only use for educational purposes
## Contact
<p align='left'><a href='https://discord.com/channels/@me/495023063486824467'><img alt="Discord" src="https://img.shields.io/badge/Discord%20-%237289DA.svg?&style=for-the-badge&logo=discord&logoColor=white"/></a></p>

<!-- https://gist.github.com/joncardasis/e6494afd538a400722545163eb2e1fa5 -->