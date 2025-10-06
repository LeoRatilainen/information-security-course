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
# b)Crack this hash: d595b2086532422bbe654bc07ea030df
