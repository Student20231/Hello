# X) Summaries 

- According to Schneier (2015), the cryptography protocol basics encompass addresses secrecy and trust issues. Thus, protocols show the necessary steps that involve
multiple parties to achieve a task. The characteristics must include the need for prior knowledge and agreement by all parties.
Security challenges: Cryptographic protocols aim to prevent cheating and eavesdropping. Therefore, it is important to formalize protocols for online interactions to
ensure fairness and security in digital interactions.
Role of arbitrators: Even though they help in completing protocols between distrusting parties and ensure fairness and trust, they also introduce vulnerabilities,
costs, delays, and potential bottleneck issues in large-scale implementations.

- Encoded Passwords and Hashcat: passwords are held as unidirectional hashes which cannot be reversed. Hashcat is a tool to decrypt such ashes using dictionary-based
 attacks; there`s a demonstration of the process that employs Hashcat through a dictionary attack sourced from the RockYou word list; the article also shows methods
 recognizing hash types and breaking down the cracking command`s elements, displaying the rate of decryption and proposing improvements such as using the host OS and
 real hardware for better performance (Torvinen, 2022).

- The command line navigation provides essential commands for file management, directory navigation and secure remote operations via SSH. The file manipulation and
system administration covers crucial file handling commands. While software management demonstrates apt-get usage for secure package installation and system updates,
ensuring software security (Torvinen, 2020).

- Frow the videos about Hacking user credentials (Santos et al 2017), I splitted the summary in 4 main components:
 •	storage security measures: OS systems by themselves can represent a robust barrier against hackers. However, it is recommended that organizations restrict access
to accounts to specific authorized personnel and conduct constant audits to fortify the system. Moreover, there should be an implementation of encryption for stored data
to prevent password hacking attempts. Use one-way hashing as a method to protect passwords, albeit not as encryption, it offers a quick computation and should always
incorporate 'salting' for enhanced security.
 •	transmission security measures: the transmitted data should be encrypted to prevent hackers from intercepting passwords. It should guard against various MITM attacks,
including those on clear text ciphered protocols as well as relay attacks. Understanding cracking tools such as medusa, thc-hydra, john ripper, or hashcat may help preventing
brute force attacks.
 •  organizations may improve password security by implementing hashing algorithms and salting techniques for stored passwords, and by encouraging the use of stronger and
complex passwords for added security.
 •  individuals may improve password security by enabling two-factor authentication for an additional layer of security, employ certificate-based authentication for more
secure access; and there is also the emphasis of use of strong, random passwords for personal accounts. 



## References 

Santos et al 2017. Security Penetration Testing - The Art of Hacking Series LiveLessons: Lesson 6: Hacking User Credentials. 
URL: https://learning.oreilly.com/videos/security-penetration-testing/9780134833989/9780134833989-sptt_00_06_00_00/

Schneier, B., 2015. Applied cryptography protocols, algorithms and source code in C, 20th Anniversary Edition. 
URL: https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

Torvinen 2022. Cracking passwords with Hashcat. URL: https://terokarvinen.com/2022/cracking-passwords-with-hashcat/

Torvinen 2020. Command Line Basics Revisited. URL: https://terokarvinen.com/2020/command-line-basics-revisited/

