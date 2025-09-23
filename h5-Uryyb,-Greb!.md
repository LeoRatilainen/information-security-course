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

# Sources

https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec006

https://terokarvinen.com/2023/pgp-encrypt-sign-verify/
