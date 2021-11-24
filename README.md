# Ransomware-Locker-Catch-And-Detect-Technique
Keywords— Ransomware, WannaCry, Crypto, Locker, Threat, Security

## Abstract

The ransomware virus has popularly created a unique ecosystem and spread like a cyclone wind amongst cyber-attackers. Ransomware is a type of software virus that encrypts all the system data and locks the system. The victim has to pay ransom to decrypt it. Therefore, this paper aims to provide an in-depth understanding of WannaCry ransomware's working threats and discuss the recent detection techniques used. In terms of detection, machine learning (ML) was the most technique adopted by ransomware researchers. However, none of the researchers has successfully designed a model to protect the system against a ransomware attack. 

## I Introduction

In recent years, Ransomware has captivated great attention from cybersecurity experts because of the fast excrescence of its attacks. Ransomware is one of the most destructive and devastating attacks, which is capable of bypassing anti-malware and anti-viruses [1]. It is a present-day malware, which has received much attention from cybercriminals. Ransomware malware intends to mainly block its victim's system from using its own resources. It targets the encrypting of valuable data or operating systems, such as passwords, presentations, spreadsheets, and images [2]. Basically, ransomware detection has two types of approaches: locker and crypto. Locker was first released in 2016; it is a type of malware that does not encrypt files. Instead, it completely blocks the victim's device, preventing them from using it. Once the device is blocked successfully, the attacker will demand a ransom to unblock the device. However, crypto-ransomware popularly was seen in 2007; it encrypts the valuable user data which cannot be further accessed by the user. It uses encryption technology; this is very difficult to resolve, and once the damage occurs, it may be irreversible to recover compared to the locker ransomware. A third type is scareware ransomware, which has been discussed in the article [3]. This type of Ransomware is used to scare the victim to pay some ransom but does not actually damage the victim's system. 
Until 2005, online exchanges were not easily accessible. As there were not many alternatives, victims were forced to pay the ransom via emailing prepaid cards or using SMS text messages [4]. All of these payment methods were sensitive, as investigators could trace the attacker's path. In 2008, Ransomware came into the role when Bitcoin was introduced. Bitcoin is also known as an electronic currency that is highly secured and extremely difficult to trace, thus helps anonymize the transactions. 
In general, locker ransomware uses a payment voucher system; the victim's computer is locked and, therefore, easier for the attacker to buy a payment voucher manually and enter the payment code. Whereas, the crypto-ransomware approach prefers Bitcoin, where the victim's device is fully functional, so attackers freely use computers to purchase Bitcoin [5]. 
In this work, we have researched on a specific working of ransomware malware. First, our examination is based on the latest studies, from 2016 onwards. Thus, the information provided is recent and authentic. Second, our source compromises only scientific journals, conference papers, newsletters, articles, and websites to ensure the accurate data. Third, we mainly concentrate on our area of interest: Ransomware locker - catch and detect techniques. The purpose of this paper is to review Ransomware's impact on the Operating System, detecting Ransomware, and avoiding such type of attack, to acknowledge valuable user information. 
This report is organized as follows: Section II describes the in-depth explanation of the ransomware virus. Section III and IV describe the effect and detection in the Operating System of ransomware malware. Avoidability and impact of Ransomware are discussed in sections V and VI. The conclusion of the work is presented in section VII. 


## II. EXPLANATION ABOUT THE VIRUS 
Life Cycle of a Ransomware attack 
Ransomware anatomy mainly consists of seven steps, as shown in Fig 1 [6]. The lifecycle reveals the accumulation of the cybercriminal network. 'Creator' and 'Campaigner' have very close relationships. The creator is known as a programmer that produces and develops the ransomware program. The campaigner is the attacking campaign organizer. A combination of both parties improves and sharpens their skills and expertise in their areas of interest with each cycle. Eventually, this produces professional cyber-attackers. 
A. Campaign 
The phishing email is one of the most popular delivery channels. The victim will receive an email from an online retailer, overcharged, or due to a refund. Accidentally, the victim will click on the link without observing the inappropriate URLs, and a ransomware attack will be activated in the system. 
Some common infections vectored are compromised websites, email attachments, email links, and social media. 
B. Infection 
In this stage, the ransomware setup execution may begin. At this point, the operating system has been infected; however, none of the system files is encrypted. 
Encryption requires a high CPU intensive task to reverse mathematical calculation. Therefore, encryption is not processed immediately because it takes time for malware to determine the data's possibility to be encrypted. 
C. Staging 
Once the setup is complete, malicious code ensures connectivity with its command and control server for several reasons. It is also known as the C2 server. Basically, the idea is to acquire the encryption key for the procedure cycle. An additional reason is to download extra files to impulse malware infection. 
At the end of the staging stage, the attacker now 'owns' the victim's system. 
D. Scanning 
Here is a stage where the process slows down a bit. Firstly, malware will scan the local computer to encrypt files. Next, data stored in the cloud is also scanned. This can take minutes to hours, depending on the connectivity. Valuable information, such as passwords, images, documents, will be scanned. 
E. Encryption 
Once the scanning is inventoried, encryption begins. Ransomware commonly uses three major encryption types: asymmetrical encryption, symmetrical encryption, and hybrid encryption. 
F. PayDay 
After the above steps have been completed, your data is gone. The attacker will demand a ransom. The demand will inform the victim about the infection occurring in his system and specify the payment mode. Additionally, demand can also have a restricted payment deadline, after which original files are deleted, and the system will be in recovery mode. 

## III. SURVEY ON RANSOMWARE INFECTION 
According to Sophos Research, from January 2020 to February 2020, 45 percent of ransomware infections 
arose via malicious links or email attachments. Another 21 percent came via a server attack. Another 16 percent came from social media or business application, misconfigured public cloud instances resulted in 18 percent, and nine percent were of a USB stick or unknown origin [7]. 
The ranking of the top 6 countries is shown in Table 1. For most parts, cyberattacks are targeting developed countries. 
1. France 
2. Germany 
3. India 
4. Australia 
5. Brazil 
6. Canada 

## IV. WORKING OF RANSOMWARE MALWARE 
G. Ranomware behaviour in the operating system 
Like most other Ransomware, ransomware scouts the victim's systems searching for file extensions to encrypt [8]. Ransomware usually leaves an AES encryption and opens a window that provides an explanation and details about the infection, as shown in the Fig 2. The windows explain what has happened to the victim's systems and issues a payment method or payment process that demands a ransom for the victim to access their files. 
H. Ransomware infection mechanism 
Ransomware has the capability of attacking all versions of the window operating system [9]. After the victim has opened the phishing email, the Trojan-Downloader, which contains the malicious code, is installed as a windows service using a random file name and usually places itself in the C:/WINDOWS/SYSWOW64 directory of the infected file name. Meanwhile, another service is installed in the: C:/PROGRAMDATA/STEG/ using the filename Steg.exe. When opened, the service creates a file under the directory C/PROGRAMDATA/ name TOR. Another file is simultaneously installed under the name LDR with its execution protocols installed at C:/PROGRAMDATA/RKCL under RKCL.EXE, which activates four services. The loaders then installed and launched an executable file under C:/PROGRAMDATA/RKCL and saved under RKCL.EE. 

## V. HOW TO DETECT RANSOMWARE VIRUS 
The following are the techniques to use to detect and prevent a ransomware attack. 
A. Carefully examine the extension files 

Even though the ransomware list is endless, there is a need to research filename extensions of Ransomware. It is also essential to have file activities monitoring installed in the computer to monitor in real-time and view the historical records of all the applications; this will enable the timely detection of ransomware attacks. 
B. Check for many files rename 

It is not common to have many files with the name in your system or network. Observing an increased number of renames illustrates an attack. Ransomware attacks by massively expanding the file renames before it starts encrypting the data on your computer. So, it is essential to be vigilant and check for file renames so that one can act and prevent the system from being attacked. 
C. Using Software 

Ensuring that one has the right software to detect and prevent Ransomware is critical and essential in the defence line. More established corporations have established software that detects and prevents ransomware attacks [10]—most of these software work by preventing file modification by application in some specific and specified folders. 
The other way anti-ransomware works is by blocking the encryption of files. If the computer has already been infected, the anti-ransomware will disengage and protect the files to prevent further encryption. Some anti-ransomware acts in a way that tricks the Ransomware to believe that the computer has already been attacked, preventing the Ransomware from acting. 
Other Ransomware provides email alerts by scanning through the email and detecting Ransomware before an individual opens their email contents. Updating and ensuring the right anti-ransomware is critical for detecting Ransomware—some of the examples of anti-ransomware include CyberSightRansomStopper, window defender, and Cybereason RansomFree. 

## VI. HOW TO AVOID 
There is no 100% security, but there are several ways to reduce the risk of attack and mitigation strategies to minimize impact in infection cases. Ronny Richardson and Max North explain in their thesis that there are four techniques to prevent an attack: 
• Backing up data 
• Attachments and Email Links 
• Patch and Block 
• Drop-and-Roll 
A. Back up 

Having multiple layers of backup can help a fast and secure recovery. It is recommended to regularly backup data and create numerous sessions daily, weekly, monthly, and yearly. Ensure all backups are placed in different places, servers, and the cloud because in case the backup is infected, it will have a better chance to recover due to a shared architecture. Use the cloud as one more layer of defense and ensure data storage in the cloud is up to date. 
B. Email Links and Attachments 

Attack using attachments or advertising links in emails are the most common way to introduce Ransomware on a computer. Once the malware is introduced in a first computer, it compromises the network in an organization, company, government, or individuals' network [8]. Constant training plays a crucial role in avoiding infection in large network environments. The use of scanners can mitigate the risk of opening malicious files, and blocking ads software can reduce the chance of clicking on malicious advertisements. 
C. Patch and Block 

Attackers are continually looking for breaches to enter and contaminate a network environment in a company, organization, or individual computer [8]. Keeping all computers, networks, and servers up to date with the latest patch can significantly reduce the risk of an attack because software providers are continually working to increase safety measures and vulnerability reductions in their software. The administrator must do all updates to ensure all updates, patches, and plug-ins are tested and checked before implemented in all production environments. End-users must not be allowed to perform any installation or update without an administrator or security team's supervision. 
D. Drop-and-Roll 

During the infection, administrators should immediately turn off the machine infected to avoid more damage. Back up should be disconnected from the network to prevent back up data contamination. If this machine is connected to the network, all the systems should turn off to avoid more contaminations [4]. Each device and server 
should execute anti-virus and malware detection software to ensure the machine and data are not affected. After the first emergency precautions are complete, a disaster recovery protocol should take over, and best practices should be executed to reestablish all environments as fast as possible [12]. 
Several measures should be taken into considerations involving multiple teams to reduce risk and loss to mitigate and attack. 
Incident response team. Scott and Spaniel explained, "Any organization that believes that they can get by without an information security team is doomed to exploitation" (2016, p32, para. 1). This team is responsible for executing disaster recovery plans, inform authorities, backup, and document all information about the incident so law enforcement can take action. 
Software-define networking. Cabaj and Mazurczyk stated that working together with a networking team can stop communication during the infection and even stop data encryption already started leveraging more time for recovery action (2016). 
E. Back up 

During the attack, backups play a crucial role in two critical stages. First, the security team must guarantee that several backup layers should not be affected by the malware code, ensuring that data integrity is safe. Second, after measures are taken to remove malware from the network, data must be appropriately restored to reestablish the environment; those measures can take hours or even days. Suppose a backup plan is not well defined; this means that an organization can lose its data resulting in a significant loss for the organization or even be a hostage of the attacker resulting in payments to get their data decrypted. There is no guarantee that the attacker will give the encryption key, and data will be recovered after payment. 

## VII. IMPACT
We live in a digital era where companies and organizations are measured not only by their physical assets but more about their data. Data is the most critical asset of the global market. However, having access to large amounts of data and correctly using those pieces of information can lead to competitive advantages in several industries, markets, and governments. Storing and securely using this information can make the difference between leading a competitive market or bankrupt. 
Those organizations are frequently under attack from computer gangs looking to steal information or kidnap information and hardware to obtain payment. Other organizations can try to access confidential information to gain more advantages in a competitive market. Therefore, Cybersecurity departments play a crucial role in the organization, ensuring that all measures are taken to prevent a company from losing its most valuable asset. As presented in an article by Malwarebytes CEO Marcin Kleczynski, "a survey was done in 2016 with 5400 high-level employers in U.S., Canada, U.K., and Germany, … 40% of businesses have experienced a ransomware attack in the last year. Of those victims, more than a third lost revenue, and 20% had to stop business completely." [11]. This type of attack can generate a tremendous impact in companies, organizations, governments, and people, affecting not just the organization itself but all society involved, putting at risk companies' reputations, products, patents, business strategies, and even lives. 
Malwarebytes CEO Marcin Kleczynski also mentions that "Over the last four years, ransomware has evolved into one of the biggest cybersecurity threats in the wild, with instances of ransomware in exploit kits increasing 259 percent in the last five months alone" [11]. Especially in crisis periods like a pandemic, where most employers work from home in a non-safe network, the risk of attack is always present in embedded emails, malicious attachments, and pitching links on the web. The Cybersecurity team plays a crucial role in managing risk, detecting vulnerabilities, implementing action from a technological standpoint, and providing security training for employers. There is no 100% security. It will always be a breach in the form of an email or a new device installed with default configurations, especially with the IoT market growing in the business where technology is used everywhere inside an organization. 
Been a victim of Ransomware can generate several problems for an organization; data loss can cause not just revenue loss but several other issues as described by Anthony P. Valach in the Magazine Forefront, "depending on the business, the productivity of the office staff may friend to a halt." Recovering from an attack can take hours, days, and sometimes it may never recover. 
The impact inside a company can be catastrophic to their reputation, resulting in loss of confidence from its customers and sometimes even legal action and penalties due to service unavailability and broken SLA. If "customer pieces of information, personally identifiable information (PII) or personal health information (PHI) of employees or customers are stolen in the attack, a documented record of these findings should be kept by the company in case an investigation by authorities or a private lawsuit." [13] The company is obligated to inform authorities and its customers about the incident. 
IT plays a critical role in company structures; having departments dedicated to improving security within the organization, providing constant training about threats and vulnerabilities, making sure a security plan and disaster recovery adequately implemented can make the difference between taking proper action to prevent an attack or the complete loss of a business. 

## VIII. CONCLUSION 
Ransomware attackers are continually working to find new ways to penetrate individuals and an organization's networks, compromising OS security. Guaranteeing safety within those organizations is not an easy task. It is crucial to invest in a Cyber Security team, employee education, and defense technology to prevent loss in business productivity and sales, employee morale, data loss, downtimes, legal actions, brand reputation, products recall. Ensuring a backup and disaster recovery strategy is continuously up to date in parallel with cyber liability coverages to mitigate possible 
risks in case of an incident. The work of a diverse group of professionals (technology teams, employees, legal teams, insurance agreements coverage, third-party security audit, etc.) can help reduce risk, damage and generate less impact on business. Individuals and organizations will never be 100% safe, but security professionals' constant work can reduce the threat into an acceptable path.  

## Author 
Meet Soni
