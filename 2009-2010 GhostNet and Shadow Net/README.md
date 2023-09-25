## Introduction
**Type:** Cyber Espionage \
**Description:** "The Shadow Net attack used internet services such as social networking and cloud computing platforms, including Twitter (now X), Google Groups, and Yahoo Mail, which were used to host and infect computers with malware." [1]

## Who Attacked and When
The Shadow Network cyber attack, also known as GhostNet, was attributed to hackers with ties to China. The attack was first uncovered in 2009, and there is no definitive proof of the exact individuals or entities responsible. However, "there was suspicion, but no confirmation, that one of the hackers had a connection to the University of Electronic Science and Technology in Chengdu. The account of another hacker was linked to a Chengdu resident who claimed to know little about the hacking." [1]

GhostNet was discovered in March 2009 and was followed by Shadow Net, which researchers "said was more sophisticated and difficult to detect." [1] Shadow Net was discovered on April 6, 2010, after eight months of research by individuals in Canada and the United States.

## Negative Impact of the Attack
The attack majorly impacted countries just beyond India. The data stolen from the compromised agencies "includes about 1,500 letters sent from the Dalai Lama's office between January and November 2009, reports on missile systems in India, and documents related to NATO force movements in Afghanistan." [2] This confidential information being potentially leaked to the Chinese government could have catastrophic impacts on any future conflict between the already hostile India and China. Access to important missile documentation could detrimentally effect the missiles effectiveness. Potentially compromising both the location and functionality of the missiles. The details regarding troop movement also could be catastrophic as the information could be passed on to opposing forces which could cost the lives of the NATO soldiers operating in Afghanistan.

## Vulnerability Exploited
The attackers behind the Shadow Network cyber attack leveraged several vulnerabilities and techniques, including:

1. Spear Phishing: The attack began with targeted spear-phishing emails sent to specific individuals within the Indian government and other organizations. These emails contained malicious attachments or links designed to compromise the recipient's system. [2]
2. Malware: Once a victim opened the malicious attachment or clicked on the link, malware was delivered and executed on their computer. This malware was responsible for establishing a backdoor connection to the attacker's command and control servers. They used exploits in Adobe PDFs and Microsoft Word 2003.
3. Command and Control (C&C) Servers: The attackers maintained C&C servers to communicate with compromised systems, allowing them to exfiltrate data, install additional malware, and maintain control over the infected systems.

## CVS Vulnerabilites
"The people behind the Shadow attacks used a variety of exploits and file types to compromise their victims. We observed the group using PDF, PPT, and DOC file formats to exploit Adobe Acrobat and Acrobat Reader, Microsoft Word 2003, and Microsoft PowerPoint 2003." [2]
1. [CVE-2009-0927](https://www.cvedetails.com/cve/CVE-2009-0927/) [3]
2. [CVE-2009-2990](https://www.cvedetails.com/cve/CVE-2009-2990/) [3]
3. [CVE-2009-4324](https://www.cvedetails.com/cve/CVE-2009-4324/) [3]

## STRIDE Model
**Spoofing**: Attackers used social engineering tactics in spear-phishing emails to impersonate trusted entities or individuals. \
**Tampering**: The attackers tampered with compromised systems by installing and executing malware, enabling unauthorised access and data exfiltration. \
**Repudiation**: This aspect is less relevant in cyber espionage cases like the Shadow Network attack. \
**Information Disclosure**: The primary goal of this attack was to steal sensitive information and documents from the Indian government and other organisations, constituting a significant information disclosure threat. \
**Denial of Service (DoS)**: The attack's primary focus was on data exfiltration rather than causing service disruptions. \
**Elevation of Privilege**: The attackers aimed to gain elevated privileges on compromised systems to access sensitive data.

## Measures in Place to Prevent Future Attacks
1. **Update Software:** The Indian government should update all their software to use the latest versions to ensure that all known vulnerabilities are patched. 
2. **Anti-Virus/Phishing Software:** Utilise software to determine if an attachment is potentially dangerous or contains malicious code. 
3. **Hosting Sensitive Information Securely:** All sensitive information should be kept in a safe location or server and should not be shared through email or other social networks.

## References
[1] Wikipedia. (2022). Shadow Network. [online] Available at: https://en.wikipedia.org/wiki/Shadow_Network [Accessed 25 Sep. 2023].
[2] CNET. (n.d.). Report: India targeted by spy network. [online] Available at: https://www.cnet.com/news/privacy/report-india-targeted-by-spy-network/ [Accessed 25 Sep. 2023].
[3] CVE Details (2009). CVE security vulnerability database. Security vulnerabilities, exploits, references and more. [online] Cvedetails.com. Available at: https://www.cvedetails.com/.
