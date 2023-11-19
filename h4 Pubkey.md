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

# a) Pubkey today

# b) Messaging

# c) Other tool 

# d) Eve and Mallory

# f) Password Management 

## References
Karvinen, 2023. PGP - Send Encrypted and Signed Message - gpg. URL:https://terokarvinen.com/2023/pgp-encrypt-sign-verify/

Rosenbaum, 2019: Grokking Bitcoin. Chapter 2. Cryptographic hash functions and digital signatures. URL: https://www.oreilly.com/library/view/grokking-bitcoin/9781617294648/OEBPS/Text/kindle_split_011.html#ch02lev1sec1

Schneier, 2015: Applied Cryptography: CHAPTER 2. Protocol Building Blocks. URL: https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003 


