# 2021 Florida Water Supply Attack

--------------------------------

### Overview
On 5th February 2021, security at the water treatment plant in Oldsmar, Florida was breached when an unknown actor gained access to the supervisory control and data acquisition (SCADA) system.[1]

Two incidents were reported on the day of the attack. Around 8am, the cursor of one operator’s computer began moving unexpectedly. Around 1:30pm, this happened again, but the actor used the cursor to navigate to the SCADA system and attempted to increase the concentration of lye (sodium hydroxide) over one-hundred-fold from 100ppm (parts per million) to 11,100ppm[2], which is well over safe drinking allowances and potentially hazardous to human health.[3]

### Impact
The impact of the attack was minimal. While suspicious activity was noticed earlier in the day, the operator assumed it was the actions of a supervisor and no action was taken. Later, when the sodium hydroxide levels were changed, the activity was noticed by the operator and action was taken within minutes to correct the sodium hydroxide levels. Officials reported that no significant change was ever made to the water supply concentration and the attack presented no danger to the public at any time.[2][4]

### Categorisation
**Spoofing** – The FBI investigation into the attack concluded that the malicious actor probably gained access to the computer system via the TeamViewer remote access software.[1] While specific details of the vulnerability that was exploited are unclear, it is possible that the actor gained access to a legitimate user’s username and password for TeamViewer to gain access to the system.[5]

**Tampering** – The primary target of the attack was changing the SCADA system’s data to change the water supply’s sodium hydroxide concentration to dangerous levels.

**Repudiation** – N/A

**Information Disclosure** – If the TeamViewer access was obtained by using a legitimate user’s login credentials, it is possible that this information was not kept sufficiently secure to prevent access by malicious actors.[5]

**Denial of Service** – Had the attack not been noticed and corrected as quickly as it was, the result would likely have been that areas served by the Oldsmar water treatment plant would have their water supply reduced or disabled for some time while excess sodium hydroxide was dealt with.

**Elevation of Privilege** – N/A

### Resulting Measures
On 11th February 2021, just under a week after the attack, a Joint Cybersecurity Advisory was released by the FBI, the Cybersecurity & Infrastructure Security Agency, the Environmental Protection Agency, and the Multi-State Information Sharing and Analysis Center.[1] It summarised the incident as well as related potential security vulnerabilities, including the threat posed by using outdated operating systems such as Windows 7 which often no longer receive security updates, as well as techniques used by malicious actors with desktop sharing software like TeamViewer. As part of the report, the authors published a list of general security recommendations, as well as recommendations specific to water treatment facilities and users of TeamViewer software.

Many state-level advisories were also sent to water treatment plants around the United States.[6]

### References
[1] ‘Compromise of U.S. Water Treatment Facility’ report by the Cybersecurity and Infrastructure Security Agency: https://www.cisa.gov/uscert/sites/default/files/publications/AA21-042A_Joint%20Cybersecurity%20Advisory_Compromise%20of%20U.S.%20Water%20Treatment%20Facility.pdf

[2] Tampa Bay Times: https://www.tampabay.com/news/pinellas/2021/02/08/someone-tried-to-poison-oldsmars-water-supply-during-hack-sheriff-says/

[3] Chemistry World: https://www.chemistryworld.com/news/florida-drinking-water-plant-hack-briefly-raised-sodium-hydroxide-levels-100-fold/4013236.article

[4] BitDefender: https://www.bitdefender.com/blog/hotforsecurity/attacker-tries-to-poison-water-supply-near-tampa-florida

[5] BitDefender: https://www.bitdefender.co.uk/blog/hotforsecurity/fbi-issues-private-industry-notification-in-light-of-florida-water-plant-hack

[6] Pew Trusts: https://www.pewtrusts.org/en/research-and-analysis/blogs/stateline/2021/03/10/florida-hack-exposes-danger-to-water-systems
