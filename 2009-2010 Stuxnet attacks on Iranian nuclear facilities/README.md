## 2009-2010 Stuxnet attacks on Iranian nuclear facilities
<br>

### What is Stuxnet 
Stuxnet is a powerful and malicious computer worm, which unlike any other virus or worm, escaped the digital realm to wreak physical destruction on the computers controlled, rather than simply hijacking the targets or stealing information from them. It is also reportedly the largest and costliest of this type of malware because not only it damaged Iran's uranium-enrichment centrifuges, but cyber attackers modified it over time and adapted it to target other establishments such as power plants and gas pipes.

### Who was attacked
The attacks which used the Stuxnet were aimed at Iran, in the hopes of delaying the country's nuclear proliferation without resorting to an airstrike or an attack by special operation forces and targeted Iran's uranium-enrichment programme, particularly IR-1 centrifuges at the Natanz plant [[1](https://www.researchgate.net/publication/323199431_Stuxnet)].

### When the attacks happened
The attacks happened in two waves. The first wave was less visible and more targeted than the second wave. It infected four Iranian organizations in June and July 2009. After that, and before Stuxnet’s public discovery, the malware’s operators tried to attack again in March. They targeted two organizations attacked earlier and a new one in April and May 2010, using updated code, which made the worm spread more aggressively [[2](https://isis-online.org/isis-reports/detail/stuxnet-malware-and-natanz-update-of-isis-december-22-2010-reportsupa-href1/#5)].

### The negative impact of the attacks
The Stuxnet worm reportedly infected more than 200,000 machines in 14 Iranian facilities and may have ruined up to 10% of the 9,000 centrifuges in Natanz, delaying the expected expansion of the plant, and further consuming a limited supply of centrifuges to replace those destroyed [[3](https://www.forenova.com/blog/deep-dive-into-advanced-persistent-threats)]. 

### The attack agent
While no country has officially admitted to creating Stuxnet, it is widely believed that the US and Israel jointly developed this cyberweapon and carried out the attacks [[4](https://en.wikipedia.org/wiki/Stuxnet)]. 

### CVEs
Stuxnet attacks against Iranian nuclear facilities targeted three systemic layers:
-	Windows OS
-	Siemens PCS 7, WinCC, and STEP7 industrial software applications
-	Siemens S7 programmable logic controller

And exploited the following vulnerabilities and exposures:
- ([**CVE-2010-2568**](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2010-2568)) served as the initial attack vector on a flash drive targeting Windows systems by allowing quick execution of a payload from a connected USB device.

- Windows Print spooler vulnerability ([**CVE-2010-2729**](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2010-2729)) which allowed remote attackers to create files in a system directory, and consequently execute arbitrary code, by sending a crafted print request over RPC.

- Siemens Simatic WinCC and PCS 7 SCADA system vulnerability ([**CVE-2010-2772**](https://cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2772)) which was the critical vulnerability that was exploited by the attackers to access the back-end database and gain privileges.

### Categorisation of threats in the STRIDE model
- **Denial of service** – the attackers rendered the centrifuges unusable  
- **Elevation of privilege** – the attackers performed privilege escalation to execute malicious code  
- **Tampering/Spoofing** – the attackers were able to send specially crafted print requests to the vulnerable systems that had print spooler interfaces exposed over RPC and then spoofed sensor signals so that the targeted systems won't shut down due to abnormal behaviour. 

### What measures have been put in place as a result of the attacks
There were several preventive and reactive countermeasures put in place as a result of the attacks.
Preventative countermeasures included effective security policies and procedures, security awareness programs within the organisations, disablement of all unnecessary services, software restriction policies, and the usage of comprehensive patch management programs.
The reactive countermeasures comprised of implementing a more secure IDS, adding passive vulnerability scanners, and implementing SCADA honeypots to help with the detection of potential malicious tampering.

### Other attacks that used the same vulnerabilities

 [CVE-2010-2568](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2010-2568) vulnerability remained extremely popular.
New families of malware such as Chmine, Vobfus, ZeuS and Sality quickly leveraged this flaw in order to propagate and infect systems which then were used to perform other attacks.

- The Vobfus worm was used to distribute a virus called 'Beebone'and in September 2014, attackers used this virus to take control of 100,000 computers in order to steal passwords and download other malicious programs [[5](https://www.bbc.co.uk/news/technology-32218381)]. 

- In February 2022, DDoS attacks were conducted against Ukrainian web forums using a botnet made of computers infected with Sality [[6](https://www.cisa.gov/uscert/ncas/alerts/aa22-110a)].


<br><br>
### References
[1] ResearchGate. (n.d.). (PDF) Stuxnet. [online] Available at: https://www.researchgate.net/publication/323199431_Stuxnet.

[2] David Albright, Paul Brannan, and Christina Walrond (2011). Stuxnet Malware and Natanz: Update of ISIS December 22, 2010 Report. [online] institute for science and international security. Available at: https://isis-online.org/isis-reports/detail/stuxnet-malware-and-natanz-update-of-isis-december-22-2010-reportsupa-href1/#5 [Accessed 4 Oct. 2022].

‌
[3] https://www.forenova.com/blog/deep-dive-into-advanced-persistent-threatswww.forenova.com. (n.d.). A Deep Dive into Advanced Persistent Threats (APT). [online] Available at: https://www.forenova.com/blog/deep-dive-into-advanced-persistent-threats [Accessed 4 Oct. 2022].

‌
[4] https://en.wikipedia.org/wiki/StuxnetWikipedia Contributors (2019). Stuxnet. [online] Wikipedia. Available at: https://en.wikipedia.org/wiki/Stuxnet.

‌
[5] Europol kills off shape-shifting ‘Mystique’ malware. (2015). BBC News. [online] 9 Apr. Available at: https://www.bbc.co.uk/news/technology-32218381 [Accessed 4 Oct. 2022].

‌
[6] www.cisa.gov. (2022). Russian State-Sponsored and Criminal Cyber Threats to Critical Infrastructure | CISA. [online] Available at: https://www.cisa.gov/uscert/ncas/alerts/aa22-110a.

‌

