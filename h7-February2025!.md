# x) Applied Cryptography: Protocols, Algorithms and Source Code in C.

## 2.3 One-way function

- One-way functions are central to public cryptography.
- While they are not protocols themselves they are a fundimental building block for most protocols.
- The way one-way function work is takes a message, encrypts it then hands it to the recipient with no way to decrypt it.
- So this shows how one-way function is not useful by it self you need something more on top of it.
- One way of doing this that's talked about in the book is trapdoor one-way function which essentially means the recipent has some other external information that he can use to decrypt the message.

## 2.4 One-way Hash Function

- One-way hash function is central to modern cryptography.
- A hash function is a function, that takes a variable-length input and converts it to a fixed length output.
- One-way hash function only works in one direction: Computing a hash value from a pre-image is easy, but generating a pre-image that hashes to a given value is hard.
- One-way hash function should also be collision free meaning it's hard to generate two pre-images with the same hash value.
- Hash function is public: The security is in the one-wayness. The output is not dependent on the input.
  
# a) Install Hashcat

- Firstly i did a 'sudo apt-get update' to update the machine
- Then i installed hashcat with 'sudo apt-get -y install hashid hashcat wget'
- I made a new directory with 'mkdir hashed' and then searched that directory with 'cd hashed'
- After this i downloaded a big dictionary with 'wget https://github.com/danielmiessler/SecLists/raw/master/Passwords/Leaked-Databases/rockyou.txt.tar.gz', 'tar xf rockyou.txt.tar.gz', 'rm rockyou.txt.tar.gz
- And then i checked the dictionary with 'head rockyou.txt' and 'wc -l rockyou.txt'

<img width="827" height="519" alt="Hashcat_install" src="https://github.com/user-attachments/assets/5d73a515-9edc-485f-9164-7566a2a2768e" />

# b) Crack this hash

- I cracked the hash with firstly identifying the hash type with 'hashid -m d595b2086532422bbe654bc07ea030df'
- then i used the given mode MD5 since that's very common with 'hashcat -m 0 'd595b2086532422bbe654bc07ea030df' rockyou.txt -o solved'
- This cracked the hash and i could see the cracked hash in clear text with 'cat solved' which was "disobey".

<img width="827" height="519" alt="Hash_cracked" src="https://github.com/user-attachments/assets/ce6166b1-d970-40b0-8552-3eecbe732151" />

# sources 

https://terokarvinen.com/information-security/

https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

https://terokarvinen.com/2022/cracking-passwords-with-hashcat/
