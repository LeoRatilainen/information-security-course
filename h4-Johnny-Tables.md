# x)
## OWASP: OWASP 10 2021.
  ### A01:2021 - Broken Access Control
#### Common vulnerabilities are:
  - Bypassing access control checks by modifying the URL.
  - Accessing APi with missing access controls.
  - Elevation of priviledge.
  - Metadata manipulation.
#### How to prevent:
  - Deny by defult.
  - Should enforce record ownership.
  - Log access control failures alert admins.
  - Rate limit API and controller access to minimize the harm from automated attacks.
  - Disable web server directory listing.
  ### A05:2021 – Security Misconfiguration
#### Application might be vulnerable if:
  - Unnecessary features are enabled or installed.
  - Default accounts and passwords are enebled and unchaged.
  - On upgraded systems, the latest security features are disabled.
  - The software is out of date or vulnerable.
#### How to prevent:
  - Minimal platform without any unnecessary features, components, documentation samples.
  - Sending security directives to clients.
  - An automated process to verify the effectiveness of the settings.
  ### A06:2021 – Vulnerable and Outdated Components
#### Common vulnerabilities 
  - You don't know the versions of all components being used.
  - The software is vulnerable, unsupported or out of date.
  - You don't scan for vulnerabilities regularly.
  - You don't secure the components' configurations.
#### how to prevent
  - Remove everything unnecessary.
  - only get components form official sources.
  ### A03:2021 – Injection
  - Some of the more common injections are SQL, NoSQL, OS command, Object Relational Mapping, LDAP.
#### Common vulnerabilities
  - User-supplied data is not validated.
  - Dynamic queries or non-parameterized calls are used directly in the interpreter.
  - Hostile data is used within object-relational mapping.
  - Hostile data is diractly used or concatenated.
#### How to prevent
  - Preferred option is to use a safe API that doesn't use interpreters at all.
  - Use positive server-side input validation.
# a)

- I wasn't able to get java 17 downloaded with the commands given so i manually downloaded java 21 from the web, this seemed to work just as well
- After this i downloaded webgoat with the command 'wget https://github.com/WebGoat/WebGoat/releases/download/v2023.4/webgoat-2023.4.jar'
  
<img width="827" height="519" alt="Webgoat_download" src="https://github.com/user-attachments/assets/cf44cf8e-5ec2-4b0e-af81-d88d2968b593" />

# b)
- I then disabled my networking and ran webgoat with localhost in port8888 with the command 'java -Dfile.encoding=UTF-8 -Dwebgoat.port=8888 -Dwebwolf.port=9090 -jar webgoat-2023.4.jar'

<img width="819" height="489" alt="Webgoat_startup" src="https://github.com/user-attachments/assets/2b37265c-873a-4899-8504-333966b49267" />

- Solving the first part was done with the command 'webgoat.customjs.phoneHome()' typed into the console.
- you can then look at the response and that'll give you the answer which in this case was "-1196949528", althought this is randomized everytime the request is made.
  
<img width="1273" height="682" alt="webgoat-part1" src="https://github.com/user-attachments/assets/172c49e0-499e-4831-b7c5-29e3bd6eb409" />

- Solving the second part was done by finding the correct network activity and checking the request tab for the code.
- this then displays the code needed to complete the assingment which in this case was '12.922941108655783' but once again this is randomized everytime the request is made.

<img width="1278" height="726" alt="webgoat_part2" src="https://github.com/user-attachments/assets/f0a75ff9-b738-49db-9851-93b7ca0e7d89" />

# c)
The update was quite Large so i can't get everything to fit here but here's a small exmaple

<img width="937" height="519" alt="Screenshot_2025-09-16" src="https://github.com/user-attachments/assets/3ac5fdae-f933-4454-ae42-54280a348a62" />

After this i restarted my PC
# d)
### 0 SELECT from basics
<img width="1088" height="917" alt="Screenshot 2025-09-16 120819" src="https://github.com/user-attachments/assets/df1756d8-1ecc-4552-a807-dd712092bcb9" />

### 2 SELECT from world
<img width="1088" height="917" alt="Screenshot 2025-09-16 120819" src="https://github.com/user-attachments/assets/646fa848-0491-4e6f-9051-862ba2ece78c" />

# e)
The lab is solved but writing '+OR+1=1-- in the URL after category,
you use a single quote to close the previous querie and then writing OR 1=1 which is a new condition that always evaluates the true and then you use two dashes to say everything after this is a comment.

<img width="949" height="648" alt="Screenshot 2025-09-16 121235" src="https://github.com/user-attachments/assets/a542c598-09d9-47db-8919-9308541fe5ae" />

# Sources

https://terokarvinen.com/information-security/

https://owasp.org/Top10/A01_2021-Broken_Access_Control/

https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

https://owasp.org/Top10/A03_2021-Injection/

https://portswigger.net/

# Updated on 28/09/2025
deleted wrong picture.
# Updated on 06/10/2025
took another crack at webgoat and was able to get it working and solved this time around.
