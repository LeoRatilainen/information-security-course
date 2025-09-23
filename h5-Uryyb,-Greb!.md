# x)

## Applied Cryptography
- In the first chapter of the book the terminology of encryption is explained.
- It talks about plaintext and ciphertext which are the normal decrypted message and the encrypted message respectively.
- It also talks about the practitioners of cryptography called cryptoanalysts and cryptologists.

## PGP - Send Encrypted and Signed Message - gpg
- This article talks about how to use PGP encryption to send secret, secure messages over the untrusted internet.
- If you want to send messages in both directions between two participants a total of 4 keys is required you need a private key and a public key for both.
- The private key is what encrypts the message as is always kept secure by the holder.
- The public key is what is sent to the recipient of the message so that they can then decrypt the encrypted message.
- Both parties need to know each others public keys for trust to be established.

# a)
I installed OpenSSH with 'sudo apt-get install ssh', 'then used sudo systemctl start ssh' to start the program, then used 'ssh leor@localhost' with my password to connect to my local host. You can use 'exit' whenever you wish to stop using that localhost
<img width="827" height="519" alt="SSH-connection" src="https://github.com/user-attachments/assets/f0ad634b-927f-48ba-bd91-4810a3a93ceb" />
# b)
I used 'ssh keygen' to generate a key and then used 'ssh-copy-id leor@localhost' to connect the generated key to my localhost this will automate the signing in process and a password is no longer need to login.
<img width="827" height="519" alt="ssh-connection-automated" src="https://github.com/user-attachments/assets/041fab2d-42df-4469-861b-8ae8e00b35b5" />

# c)
For this exercise i chose keePass based on absolutely nothing as i don't know much about password managers but from a google search i saw it was cloudless, free and open-source. the software was quite hard for a first time user to understand but after playing with it for a bit i used the following method. you add New entry from file in the top left corner then go choose your settings and setup a master password. You can then add a new entry by right clicking the app, In there you can setup a username and the URL for that password to automate logins.
<img width="489" height="504" alt="Screenshot 2025-09-23 125152" src="https://github.com/user-attachments/assets/5a78f448-facb-45b8-9574-5fd852b955b9" />

the threat that password managers protect from are reusing old bad passwords it will automate creating a strong encrypted password that is near impossible for threat actors to crack they also sometimes include 2FA or two-factor authentication and a password breach monitoring to see if your password is compromised.

# s) 
The answer is "That's it. You're now officially a codebreaker! As you see, simple substitution ciphers can be broken with frequency analysis. See you at http://terokarvinen.com". The short version of how i figured it out is firstly DHHP:// which looks alot like the HTTP at the start of a URL which then would give you the presumption that it also ends with a .com, then the first word HDMH'B becomes ThMt'B which looks a lot like that's. I then checked for the most common word in the english language which are "you", "see" and "the" and at this point KWU wich is repeated multiple times had an o in the middle making it a likely candidate for "you" which then would give you the assumption the KWU'YI is you're. i then sort of brute forced the rest of it with the context clues from the course that the URL which at this point turned into teroLarCTAeA was likely terokarvinen. at this point most of the text is solved and with some thinking and a little more brute forcing you can guess the rest of the words.

 <img width="885" height="521" alt="codebreaker" src="https://github.com/user-attachments/assets/35db2d26-9509-4e4e-9484-0244350936bc" />

# Sources

https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec006

https://terokarvinen.com/2023/pgp-encrypt-sign-verify/

https://terokarvinen.com/information-security/

https://keepass.info/
