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

<img width="610" height="434" alt="Screenshot_2025-09-16_12-52-43" src="https://github.com/user-attachments/assets/31efbec4-25df-40b7-99af-ab8252654ff6" />

# b)
I could not for the life of me get this part working even after multiple redownloads, updates and guides on the opertaing system, java and webgoat and trying different commands it would always just return me with the same line when trying to change the port of webgoat:

bash: java: command not found
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

# n)

<img width="933" height="535" alt="Screenshot 2025-09-16 122633" src="https://github.com/user-attachments/assets/5d5d7c8f-de1c-41ca-80df-3580edec5a41" />


# Sources

https://terokarvinen.com/information-security/

https://owasp.org/Top10/A01_2021-Broken_Access_Control/

https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

https://owasp.org/Top10/A03_2021-Injection/
