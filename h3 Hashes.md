# X)

- The chapter 2, authored by Schneier (2015), defines protocols as agreements between two or more parties. The cryptographic protocols, in particular, is to prevent cheating
where participants cannot do or learn more than the pre-specified in the protocol. To illustrate, these protocols go beyond simple secrecy, such as sharing secrets, joint
computation, identity verfication or contract signing.
In this chapter, it is identified different types of protocols such as arbitrated protocols, adjudicated protocols, and self-enforcing protocols.
The author goes further to state that attacks against protocols may happen when hackers try to involve altering the protocol, pretending to be someone else, or manipulating
messages. Another challenge is the exploration of digital signatures to attack some given system. Thus, it is important to combine those digital signatures with encryption
to enhance security.  

- According to Karvinen (2022), systems store hashes, not original passwords due to the onw-way nature of hashing. In the article, there is a reference to hashcat, a password-cracking tool, to demonstrate hash cracking. The steps to crack the hash include: installing hashcat with commands; creating a new directory; downloading the Rockyou dictionary, extracting it, and removing the compressed file; identification of the hash type; and finally cracking the hash with hashcat. Moreover, for better performance it is recommended to use hashcat with the host OS and real hardware.

- In the article "Command Line Basics Revisited", Karvinen (2020) refers that the command line in Linux and BSD has a long history, predating Google, the web, Linux, Windows, and the internet. It is known for its convenience, speed, expressiveness, and ease of automation. The basic command prompt is represented by '$' and the hash mark is '#' is a comment character. The article shows many hints for moving and looking around such as 'cd' to change directories; for file manipulation e.g. 'mkdir' to create a new directory and 'rmdir' removes an empty directory; etc.

# a) Billion dollar busywork

As shown below in the picture, I was able to create a hash that starts with 0 by writing 'echo -n 'DebianPedroFonte 80'|sha256sum'. It was a trial by error. 

<img width="319" alt="0 hash" src="https://github.com/Student20231/Hello/assets/149126670/b39a8d99-502a-4bd3-9ed1-7e0440dffa48">

# b) Compare hash

First, I created the text file called tero.txt and inside it was written "Small text file" and I used the `cat` command to see this same content. Then, I calculated the initial hash by writing sha256sum tero.txt. With the command nano tero.txt, I opened a text editor and changed the word "Small" to "small". This slight change has influenced completely the hash. The new hash was calculated by inserting again the command sha256sum tero.txt. 

<img width="367" alt="Screenshot 2023-11-15 235853" src="https://github.com/Student20231/Hello/assets/149126670/0898a3ee-84b8-4d80-848b-4988714cb7eb">





## References
Karvinen, 2022. Cracking Passwords with Hashcat. URL: https://terokarvinen.com/2022/cracking-passwords-with-hashcat/

Karvinen, 2020. Command Line Basics Revisited. URL: https://terokarvinen.com/2020/command-line-basics-revisited/

Schneier, 2015: Applied Cryptography: CHAPTER 2. Protocol Building Blocks. 
URL: https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

