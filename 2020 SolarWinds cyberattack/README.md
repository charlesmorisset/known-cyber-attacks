# SolarWinds cyberattack (2020)

--------------------------------
### Who was attacked and when

SolarWinds is a software company who is most known for creating systems like 'Orion' which helps businesses to manage
their IT infrastructure.The SolarWinds attack was discovered in December of 2020. Unfortunately for SolarWinds, the 
attackers had gained access in September 2019, meaning their actions went undetected for 14 months. Nobelium, a 
potential nation-state hacker group, were identified by microsoft as being responsible.

### The negative impact of the attack

Due to the long duration of time that this hack was left undetected it allowed the previously mentioned attackers known
as Nobelium to steal data for 14 months from more than eighteen thousand organisations. This complete breach of GDPR 
then grew exponentially due to the fact that the attack allowed Nobelium to see the inner workings of Orion's users, 
thus compromising those who used the user's systems.

### Categorisation via the STRIDE model

####Spoofing:
This was one of the main reasons this attack was able to go on for so long. Due to the hackers installing
malicious code into the orion system they were able to create a backdoor. Nobelium were then able to utilise this by
gaining access to the organisations' systems and managed to impersonate users on these systems.

####Tampering:
Although the reason for this attack remains unkown it is EXTREMELY likely that database integrity was
compromised by this attack.

####Repudiation:
It is evident that Nobelium was able to impersonate users within the orion's systems. This is evidence that they were
presumably able to mimic and/or deny transactions within systems, making them hidden.

####Information disclosure:
Due to the large amount of time that the SolarWinds attack went uncovered, it is thought that thousands of customers
from thousands of organisations had there data stolen. The fact this went on for so long means that the attackers would
have been able to get far more data than if they were detected immediately and therefore for each customer there was
most likely months worth of data stolen.

####Denial of service:
Due to the nature of this attack being to remain hidden and avoid suspicion, there is no evidence or reason to think
the attackers were planning to deny service as this would alert SolarWinds to the attack almost immediately.

####Elavation of privillege:
Because of Nobelium's ability to impersonate users, they were able to act as admins to systems without ever revealling
themselves

### What measure have been put in place as a result of the attack. 
After the SolarWinds attack which was actually one of many in 2020, the U.S. CyberSecurity and Infrastructure Security
Agency saw first began by issuing guidance that helped defend against supply chain attacks like this one. It wasn't till
one year later that the biden administration put out an executive order mandating SBOMs which are used to quickly 
determine wherether they are at potential risk of a newly discovered vulnerability

### References
* https://www.techtarget.com/whatis/feature/SolarWinds-hack-explained-Everything-you-need-to-know#:~:text=On%20May%2027%2C%202021%2C%20Microsoft,more%20than%20150%20different%20organizations.
* https://www.businessinsider.com/solarwinds-hack-explained-government-agencies-cyber-security-2020-12?r=US&IR=T
* https://en.wikipedia.org/wiki/2020_United_States_federal_government_data_breach
* https://advisory.kpmg.us/blog/2020/what-are-sboms.html
