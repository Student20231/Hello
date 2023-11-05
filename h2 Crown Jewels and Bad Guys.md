# x) 

- The text written by Hutchins et al (2011) shows that intelligence-driven security focuses on combatting advanced persistent threats by using a structured intrusion kill 
chain model; it also shows the phases of the intrusion kill chain; through the lockheed martin incident response case study, we can understand that even utilizing zero-day 
exploits can help identifying and mitigating attacks; highlights the importance of detecting and analysing early potential instrusions; it shows the significance of campaign 
analysis in order to track recurring patterns; it refers to a strategic defensive methodology that understands tactics and intentions of adversaries.

My perspective: It seems to me that the Kill Chain Model is a framework that helps organizations prevent online attacks. Me, being an absolute rookie, I would look into this 
framework whose steps are easy to understand in order to test the defensive system of some server. I remember having a colleague in the high school who had a hobbie to hack 
computers. I remember him saying that he knew how to create trojan horses and deploy them. Trojan horses are programs disguised as benevolent software that contaminates the 
OS as soon as the user clicks the wrong link (without researching that is my idea of trojan horses). Does it matter having a kill chain model in place if the guy in the 
marketing department "opens the castle gate" to the invader? 

- The text written by Shostack (2014) covers the following aspects: 1.Checking your tests - it highlights the importance of building effective test to detect security issue for
each threat addressed; 2. Threat modeling on your own - there`s a five-step process that independently conducts threat modeling, emphasizing practice and experience to improve
skills; 3. Choosing the threat model next - guides system selection for threat modeling, considering trust boundaries and collaboration aspects; 4. checklists for diving in -
offers checklists for diagramming, examining threats, validating threats, and summarizing the threat modeling process; 5. Summary of threat modeling - it explains the threat
modeling, the STRIDE model, Elevation of privilege game, mitigation strategies, and the importance of addressing threats in software.

My perspective: Security is highly important as it protects the organization's database against potential threats. If I understood well, boundaries and collaboration aspects
are the most critical areas for me, as they pertain to data storage and transition, areas where hackers might target the system. I don`t have any other technical knowledge
about the matter. 

- The Debian installation was very straightforward. I could install everything and apparently successfully. I`m just wondering that the browser in the VM is too slow. From
the browser firefox, I clicked in the wikipedia icon and took roughly 80 seconds to actually enter.

# a) Make-belief boogie-man

Business description: Securecompany Ltd. is a company that enables the data transfer between small businesses.
Technical expertize: The specialist contributes by ensuring that the platform is built on robust encryption methods and effective authentication protocols. 

Theat modeling: 
1. What are we working on?
  Guaranteeing the safe file sharing app and its infrastructure.

2. What can go wrong?
  Data breaches since there might be unauthorized access to sensitive files and network vulnerabilities that exploit communication channels.

3. What are we going to do about it?
  Implementation of robust data encryption methods and limit authentication to database of those small companies to just a few people.

4. Did we do a good enough job?
  Diagram analysis: 
  Data storage - Implement encryption and access controls to mitigate risks.
  Authentication system - Implementation of strong password policies by utilizing an effective authentication protocol. 
  Network infrastructure - Analysis of risks related to network vulnerabilities.

Diagram representation:

<img width="438" alt="Diagram analysis" src="https://github.com/Student20231/Hello/assets/149126670/bae1e9e2-594c-4f89-9d5d-b55313e0d4d8">

# b) Incident case analysis - Canada`s Military and Parliament websites (I`ve done it before)
There is a list online about cyberattacks since 2006 (CSIS, 2023) that I consider credible and detailed enough to proceed to a Cyber Kill Chain analysis (CSIS, 2023).

Procedure:
Reconnaissance: Perhaps the hacktivists identified vulnerabilities in those websites that were susceptible to DDoS attacks;
Weaponization: Then, they developed or obtained the necessary tools or technique to carry out the DDoS attack;
Delivery: Execution of the attack to overwhelm the websites` servers;
Exploitation: Exploitation of vulnerabilities in network resources;
Installation: maybe there was no installation but rather an ongoing attack;
Command and control: The attackers could have monitor the impact and adjust the attack strategy to sustain or amplify the assault;
Actions on objectives: To disrupt the Canadian Military and Parliament websites.

# c) Starting a lab. Installation of Debian on Virtualbox.

I forgot to report the environment  while I was installing it. Therefore I went to the terminal to collect the following information:

- System Information:
  System details - Linux pedro-virtualbox 6.1.0-13-amd64 #1 SMP PRREMPT_DYNAMIC Debian 6.1.55-1 (2023-09-29) x86_64 GNU/Linux
  Debian version - 12.2
  
- History:
  1. sudo apt-get update
            2. sudo apt-get update
            3. sudo apt-get -y dist-upgrade
            4. sudo apt-get -y installv ufw
            5. sudo ufw enable
            6. sudo reboot
            7. cd /media/*/VBox*
            8. ls
            9. sudo bash VBoxLinuxAdditions.run
           10. sudo reboot
           11. uname -a
           12. cat /etc/debian_version
           13. history


## References 

CSIS, 2023. Significant Cyber Incidents. URL: https://www.csis.org/programs/strategic-technologies-program/significant-cyber-incidents.

Hutchins et al, 2011. Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains. 
URL: https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf

Karvinen 2023. Install Debian on Virtualbox - Updated 2023. URL: https://terokarvinen.com/2021/install-debian-on-virtualbox/

Shostack 2014. Chapter 1 Dive In and Threat Model!URL: https://learning.oreilly.com/library/view/threat-modeling-designing/9781118810057/9781118810057c01.xhtml#c01_level1_1


