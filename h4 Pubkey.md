Due to the requirements of the homework found in Karvinen (2023,b), this is what I could have executed: 

# X) Summaries
### *Schneier 2015 Applied Cryptography: Chapter 2 - Protocol Building Blocks, sections*

- 2.5 Communications Using Public-Key Cryptography:
  1. The public-key cryptography uses a pair of keys - a public for encryption and a private for decryption;
  2. In this system, users establish an encryption protocol. In the example provided, Alice uses the recipient`s public key (Bob) to encrypt a message and then Bob decrypts it using their private key;
  3. Public-key algorithms are used for encrypting and distributing session keys, which combined with faster symmetric algorithms secure communication, presenting as a practical hybrid cryptosystem approach;
  4. In the text, there`s the reference to the 'Merkle`s Puzzles', which is a concept or method that is resistant to brute-force attacks, ensuring the security of the communication between sender and recipient (Schneier, 2015, chapter 2.5).

- 2.6 Digital Signatures:
  1. Schneier (2015, chapter 2.6), refers to the characteristics of handwritten signatures, stating that they are seen as  genuine and convincing, thus proving that the signer intentionally authenticated the document;
  2. Moreover, they resist reuse and relocation, remaining unaltered after signing and so preventing denial of commitment by the signer;
  3. When a certain file is copied or modified, there are potential inefficiencies and security concerns and the solutions to address those challenges are the use of a protocol involving a trusted arbitrator (Trent) and symmetric cryptosystems;
  4. Timestamps and one-way hash functions are techniques that are used to implement efficiency and reduced storage requirements. 

- 2.7 Digital Signatures With Encryption:
  1. Security and authenticity are enhanced when there is a combination of digital signatures with public-key cryptography;
  2. As an example, Alice first signed a message with her provate key and then encrypted it using Bob`s public key, demonstrating a sequence of signing and encrypting;
  3. In order to prevent resend attacks, the protocol suggests to employ distinct operations for encryption and signatures, unique keys, or timestamps to ensure the integrity of messages;
  4. In the text, there is a reference to the trusted Key Certification Authority (KDC) in signing and validating public keys, hence mitigating risks such as key substitution during transmission (Schneier, 2015, chapter 2.7). 

- 2.8 Random And Pseudo-Random-Sequence Generation:
  1. According to Schneier (2015, chapter 2.8), there is a need for robust random sequences in cryptographic application to avoid exploitable patterns;
  2. Pseudo-random sequences aim to mimic randomness. However, they are deployed periodically, thus for cryptographic suitability they must not only pass statistical test but also be computationally unpredictable.


### *Rosenbaum 2019: Grokking Bitcoin*

- Chapter 2. Cryptographic hash functions and digital signatures:
  1. Rosenbaum, (2019, chapter 2) explores the importance of cryptographic hash functions demonstrating how they can ensure the integrity of files over different time points;
  2. The integration of digital signatures into the uncomplicated cookie token system can adress the challenge of fraudulent transactions;
  3. The hashes in Bitcoin act as unique fingerprints that are challenging to replicate, ensuring data integrity;
  4. Functions like SHA256 in Bitcoin transform digital data into fixed-length hash values;
  5. Properties like collision resistance, pre-image resistance, and second pre-image resistance reinforce network security;
  6. Digital signatures tied to private keys, provide a robust approval security in Bitcoin;
  7. Furthermore, digital signatures can enhance the reliability of a cookie token system by preventing fraudulent transactions with key pair generation, signing, and verification.


### *Karvinen 2023* 

-  PGP - Send Encrypted and Signed Message - gpg:
  
  1. PGP is a robust encryption standard that secures messages by encrypting and signing them;
  2. In the example shown in the text, Alice sends an encrypted message to Tero;
  3. The text explains GPG as an encryption tool and assists on its installation;
  4. Also, there is the explanation on how we can generate keys;
  5. It shows how a message can be decrypted and verified using a private key and Alice`s public key (Karvinen, 2023).  

# a) Pubkey today

After finding the article "Basics of cryptography: The practical application and use of cryptography" written by Manikandan, J., (2018), in regards to the use of cryptography in Whatsapp, I thought it was interesting to examine the document since I use the tool on a daily basis. 

1. The system name is called Whatsapp.
2. The key usage is public key encryption (Asymmetric cryptography) in which the sender uses the public key of the recipient to encrypt the message, and the recipient uses their private key to decrypt the message.
3. The implementation steps comprise the installation of the tool on a user`s smartphone in which the public keys of the clients are registered with the Whatsapp server; Public are then retrieved from the servers whenever there is the need for communication; after, an encypted session is created between two clients participating in a conversation; finally, if the sender wants to send a message to the recipient, then public keys of the recipient are retrieved from the server. Next, the sender encrypts the message with the recipient`s public key and sends it. The recipient can now decrypt the message with their private key;
4.  The tool employs end-to-end encryption, ensuring that only a certain recipient can read the message.

# b) Messaging

After reading the article "PGP - Send Encrypted and Signed Message - gpg" (Karvinen, 2023), I was able to use the following commands: 

<img width="370" alt="Messaging1" src="https://github.com/Student20231/Hello/assets/149126670/b5412888-1437-41ad-9d21-8a174b01cb61">
<img width="369" alt="Messaging2" src="https://github.com/Student20231/Hello/assets/149126670/f1e56354-31a2-4b4b-b2c2-1b1c0c112542">
<img width="368" alt="Messaging 3" src="https://github.com/Student20231/Hello/assets/149126670/d1be63a0-9569-4292-a890-87d667cc8e5c">
<img width="366" alt="Messaging 4" src="https://github.com/Student20231/Hello/assets/149126670/6ea7b503-99d1-4b5e-8b91-b8c60a28ed48">
<img width="364" alt="Messaging 5" src="https://github.com/Student20231/Hello/assets/149126670/e47ce1af-d7d3-4503-b148-a6b8e9011ad3">

However, I couldn`t continue after this. I`m not sure why. It only showed a message saying that there was file or directory with that name. 

# c) Other tool 

For this exercise, I used the tool "ccrypt" in order to encrypt and decrypt a file in Debian. This tool, which uses Rijndael cypher (Avishek, 2023), has two main commands: 'ccencrypt' and 'ccdecrypt'. Before proceeding to the exercise, I created manually a file in my desktop and inserted it inside a folder in the desktop. Then, I installed ccrypt, encrypted the intended file which involved the creation of password, and proceeded to its decryption. 

<img width="369" alt="ccrypt1" src="https://github.com/Student20231/Hello/assets/149126670/ca61410b-81ac-4830-b73c-ef1fdf13d106">
<img width="367" alt="ccrypt2" src="https://github.com/Student20231/Hello/assets/149126670/7726f50d-f8f9-4637-bc05-52e1037a1fd7">

The security of this tool doesn`t seem so sophisticated as the gpg. It reminds me of a zip file which basically contains a password protecting the file content. 

# d) Eve and Mallory

PGP defends against passive eavesdropping (Eve) and message tampering (Mallory) by encrypting message content and employing hash algorithms like SHA-1 for integrity verification. It also uses digital signatures to authenticate senders, stopping Mallory`s attempts at covert message change. Therefore, senders sign messages with their private keys, and recipients can use the sender`s public key to verify signatures (Callas, Donnerhacke, Finney, Shaw, Thayer,2007). It is important also to note that PGP leverages a secure Web Key Directory service for locating OpenPGP keys over HTTPS, ensuring the authenticity and integrity of public leys for encryption and signature verification (Koch,2023). In regards to the command flags, '--encrypt' encrypts messages as shown before and '--sign' adds a digital signature (Callas et al.). 

# f) Password Management 
https://www.howtogeek.com/devops/how-to-use-pass-a-command-line-password-manager-for-linux-systems/



# g) Refer to the sources

Done.

## References
Avishek, 2023. 7 Tools to Encrypt/Decrypt and Password Protect Files in Linux. Tecmint. URL:https://www.tecmint.com/linux-password-protect-files-with-encryption/

Callas, Donnerhacke, Finney, Shaw, Thayer,2007. URL: https://www.rfc-editor.org/rfc/rfc4880.html

Karvinen, 2023. PGP - Send Encrypted and Signed Message - gpg. URL:https://terokarvinen.com/2023/pgp-encrypt-sign-verify/

Karvinen, 2023,b. Trust to Blockchain 2023 autumn. URL: https://terokarvinen.com/2023/trust-to-blockchain/

Koch,2023. OpenPGP Web Key Directory. URL: https://www.ietf.org/id/draft-koch-openpgp-webkey-service-16.html

Manikandan, J., 2018. Basics of cryptography: The practical application and use of cryptography. 
URL: https://resources.infosecinstitute.com/topics/cryptography/basics-of-cryptography-the-practical-application-and-use-of-cryptography/

Rosenbaum, 2019: Grokking Bitcoin. Chapter 2. Cryptographic hash functions and digital signatures. URL: https://www.oreilly.com/library/view/grokking-bitcoin/9781617294648/OEBPS/Text/kindle_split_011.html#ch02lev1sec1

Schneier, 2015: Applied Cryptography: CHAPTER 2. Protocol Building Blocks. URL: https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003 






