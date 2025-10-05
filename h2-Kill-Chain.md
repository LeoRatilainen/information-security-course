# h2 Kill Chain

## x)

- The abstract talks about how normal defense tools like anti-virus focuses on the vulnerabilty part of risk which presupposes that the intrusion has already taken place.

- It also talks about a new level of threats that use a more sophisticated forms of intrusion that use multi-year long campaings to access highly sensitive information.

- Then goes on to say how knowledge about these actors can create an intelligence feedback loop to help the defenders.

- In part 3.2, kill chains and their importance is explained.

- The word "chain" is used to emphasize the importance of how every step in the process is integral to the success of the operation.

- Then expanding from this a new kill chain model is presented containing

  1. Reconnaissance - Research into the target often in the form of internet websites, mailing lists for email addresses, social networks and information on techologie
  
  2. Weaponization - Creating a payload containing an exploi
  
  3. Delivery - Transmitting the payload on to the intended subjec
  
  4. Exploitation - Triggering the payloads code to gain access to the victims system

  5. Installation - Installing a remote access trojan to maintain presense in the system

  6. Command and Control - Beaconing outbound to an internet server. Once the channel is established, intruders have access inside the target enviroment
  
  7. Actions on target - Only after all six previous objectives are complited can you take the intended action on the target

Comment - i think the subject is quite hard to understand as someone who doesn't have much prior knowledge of the subject. But i do find them quite fun to learn about
  
## a)

- A tactic represents the why of a techique or sub-technique. The intruders goal. One exmaple of tactic is Initial access which consists of tecniques an attacker might use to gain access

- techiques represent how an attacker might achieve their goals and sub-techniques are more specified versions of an attackers behavior. One example of a technique in initial access can be content injection in which an attacker injects malicious content into the system. And one example of a sub-technique could be
phising in which the attacker sends phising messages to gain access to the victims system. this contains all forms of social engineering in which the attacker tries to trick the victim into accepting harmful malware into their system

- Procedures are the specific implementations of how an attacker uses these techiques and sub-techniques. The techincal implementation of these. One exmaple of a procedure in content injection is MoustachedBouncer in which it injects content into DNS, HTTP and SMB replies to fake windows updates to dowload malware.
And one exmaple of a phishing procedure could be Royal in which a phishing campaing has lured the victim into calling a number provided in an email.

Comment - I find it hard to understand most of the procedures with no prior knowledge of how to do anything on technical side.

## b)

<img width="686" height="404" alt="Screenshot 2025-09-02 005452" src="https://github.com/user-attachments/assets/e50147ed-9c2c-4bc9-883e-06443f492961" />

## Sources
Karvinen 2024: Information Security Course, https://terokarvinen.com/information-security/

Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf read: 02.09.2025

MITRE ATT&CK, https://attack.mitre.org/ read: 02.09.2025

MITRE ATT&CK, Frequently Asked Questions, https://attack.mitre.org/resources/faq/#general-faq read: 02.09.2025

# Updated on 05.10.2025
Fixed some typos
