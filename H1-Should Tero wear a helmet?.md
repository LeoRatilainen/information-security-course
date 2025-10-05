# H1 Should Tero wear a helmet?
## x)
### Threat modeling summarized

- Threat modeling in highlighting concernes about security and privacy.
- The highest level of this is asking four questions.
	1. What are we working on?
	2. What can go wrong?
	3. What are we going to do about it?
	4. Did we do a good enough job?
- Everyone should threat model to some degree.
- The values of threat modeling are
	1. Finding and fixind design issues.
	2. Journey of understanding.
	e. Continuous refinement.

### Infosec scene

I chose episode 40 which talks about a red teamer named Kyle and his adventures trying to legally hack a utility company in the US.
A red teamer is someone who is hired to digitally or physically break into a network or a building respectively for the purposes of the company simulating an actual attack scenario so they can improve their security.
I don't want to talk about too about the episode i think it's really funny, but essentially it goes over how he physically got access to four office buildings of this company and the different security flaws they had.

## a) Security hygiene.
What security practices everyone should follow?
- Keep your device updated
- Use a password manager
- Keep an eye on your anti-virus
- Don't click links if you don't know what they are
- Follow recomendations from experts 
- Use a VPN
- Don't log in to sensitve stuff on public wi-fi
## b) Make-belief boogie-man.
### (1) What are we working on?
I made up company that sells consumer electronics in an online webstore. for this our main security priority or crown jewel is customer databases, which in this case is extra important since it contains customer bank accout details and personal information such
as log in information and addresses. For this we are working on a website that needs to be secure by making sure our passwords are encrypted properly and that our databases are not vulnerable SQL-injections.
### (2) What can go wrong?
For this exercise i used the STRIDE attack model in which i think all six attack vectors are very high risk factors, there are also multiple SQL-injection risks that are too numerous to count and frankly i'm most likley not aware of all of them
### (3) What are we going to do about it?
The main thing we need to keep in mind while building that website is making sure it get's constructed in secure way this means getting consultation from experts, hiring pentesters to break that site as it's being built which they will do and making sure all the databases
are construced with proper encryption methods
### (4) Did we do a good enough job?
A good security is an ever involving process and threat models need to always be kept in mind and updated as the process keeps going this also entails constant testing of security, but i feel like this is a good start to my threat model

## Sources 
Karvinen 2024: Information Security Course, https://terokarvinen.com/information-security/

Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course (12 parts, about 15 min total, audio is enough for all except video 7 "Data flow diagrams"), https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf

OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html

Rhysider, Jack. 08.09.2022, It Shouldn't Be THIS Easy to Break Into a Utility Company🎙Darknet Diaries Ep. 40: No Parking https://www.youtube.com/watch?v=3iAlCImWD2w

# Updated on 05.10.2025 to include a missing section 
