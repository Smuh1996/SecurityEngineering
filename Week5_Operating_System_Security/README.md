# Week 5

### Task1: Bring your own devices

Following link containing NIST:s [security recommendations for workplace bring your own device](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1800-22.pdf). On the page 12 is listed following 9 threat events, and your job is to make one A4 sized poster or otherwise shortly summarize what each listed threat event means based on the document or your own research.

Answer:Intrusive application practices: Applications that request more privileges on the phone than it's needed, It may in turn spy on users or harvest unnecessary information.

2. Account credential theft through phishing: The attacker deceive the users into giving their log-in details by  emails, messages inbox or even fake web links.

3. Outdated phones: Devices that are using old OS or software versions and have no protection against different  attacks as they do not have the necessary updates.

4.Sensitive data transmissions: Data being shared  across the network are in unencrypted or inappropriately protected form which can be easily taken by attackers.

5. Brute-force attacks to unlock a phone: It means that unauthorized use through tries of the telephone’s passcode or PIN, and gaining access after several tries.

6.Application credential storage vulnerability: Application credentials such as passwords which are either weak or poorly secured that attackers can easily harvest for illegitimate use.


7:Unmanaged device protection: Devices that are not controlled by a company’s IT security policies are more disposey to being compromised and improper usage.

8. Lost or stolen data protection: That information on a lost/stolen device is secured, usually through encryption or facility to delete data stored on the device.

9.Protecting enterprise data from being inadvertently backed up to a cloud service: Disabling such applications from synchronizing to an individual’s own personal clouds, which may be a threat to the company


### Task2: attacks on CPU execution
spectre and meltdown are two original side channel attacks discovered in 2017 that target cpu, and over the years more have been discovered. [This wikipedia article](https://en.wikipedia.org/wiki/Transient_execution_CPU_vulnerability) list some of them. Pick 3 of them to research about how exactly each exploits the system,their differences, which systems they targeted and how they can be mitigated. 

Answer in max 300 words. You are free to use tables or otherwise make to comparison easier to read if you wish.


### Task3: Securing OS
Following is a list of some of the more common vulnerabilities and attack vectors existing in operating systems.  

Malware and Viruses
Harm: Malware can spy  and steal personal information, delete files, have a impact on computer’s performance, and even enslavement complete control of your computer.
Windows Mitigation: The best method of detecting and removing the malware is by using the Windows Defender tool. The user must ensure that the Operating systems are up to date current security patches.

2. Realizing Software Vulnerabilities
Harm: They can use the open loophole to perform unauthorized code or code that will probe the system of the owner of the software.
Windows Mitigation: Windows Update can resolve them by offering latest updates periodically. Utilize Application Guard in order to start applications in a safe container.

3. Other two threats of the organism are phishing and social engineering.
Harm: Attacker is likely to deceive the users into providing their account details such as passwords or credit card details.
Windows Mitigation: SmartScreen Filter offers protection against malicious Web sites and phishing. Training users is also very important as well.

4. Drive-by Downloads
Harm: Keep installing unwanted programs in your system without your consent while you are browsing.
Windows Mitigation: Microsoft Edge provides safety against links to dangerous websites, and Windows Defender helps to search for dangerous files.

5. Zero-Day Exploits 
Harm: It takes advantage of the still unexplored weaknesses within the software before the release of updates,that can give the hackers access to your control or data.
Windows Mitigation: Organizations are exposed to such attacks; Windows Defender Exploit Guard advances such an attack and everyday upgrade to the system erases the previously found loophole.

6. USB/Removable Media Attacks
Harm: computer viruses can be spread from infected USB drives that may cause harm to the system, or enable to access the data.
Windows Mitigation: Windows defender performs a scan on the external devices without the user having to do anything. It can protect data on a USB drive by encrypting it thus discouraging any form of intrusion.

7. Password Cracking
Harm: The passwords are open for guess or other attacks such as brute force hacking of system or a sensitive account.
Windows Mitigation:You should ensure that there is strict password is applied and make sure that Windows Hello, which uses fingerprint recognition is utilized for signing in.


These all steps together with safe practices will reduce by a greater magnitude some of the risks that come with these attack vectors.

---

### Task4: Logging
Log files are records of events or actions that occur in a system, application, or program. Logs are essential for troubleshooting, debugging, and analyzing the behavior of software or hardware.

Find answers to following questions:
1. What kind of information would be saved into following types of log files
- Application logs
- Event logs
- Service logs
- System logs

2. Where in each of the common Operating Systems those logs would be stored (Windows, Mac, Linux(changes per distro so provide in answer which you are using)
3. What kind of threats could you notice by monitoring each log file?
4. How would you go about monitoring logs on your personal computer?

Answer:Types of Log Files and What They Store

Application Logs: It describes events that occur in applications, such as mistakes or a user input.
Event Logs: It captures the key events that happen around the system such as logins and crashes, and even updates if any.
Service Logs: They monitor what background services, for example web sites or databases, are doing.
System Logs:It records any difficulties with the computer, for instance with the hardware, or times the computer has locked.


Log File Locations in Operating Systems

Windows: Event logs are stored in C:\Windows\System32>winevt>Logs>. 
See them using the tool known as the Event Viewer.
Logs are in /var/log/ for system info, and in ~/Library/Logs/ for app logs. Use the Console app to check them.

Logs are in /var/log/. For example, system logs are in /var/log/syslog on Ubuntu.



Threats we Can Spot in Logs

Application Logs: It should show if somebody is trying to crack an application.

Event Logs: It Informs you about attempt failure at login and changes.

Service Logs: Indicate whether a service that an organization offers, for example a website is under an attack or not working well.

System Logs: It is great for finding things that are wrong in the program, such as a piece of hardware that has stopped working, or someone who is deliberately

