# 1999 - NASA Attack 👨‍💻

From August to October 1999 (Rohit Sharma, 2017), Jonathan James, a 15-year-old boy, under the pseudonym of Comrade repeatedly penetrated into the computers of NASA to and a US Defence Department agency. 

## Who was attacked and when?

The attacks were carried out in 1999 by Jonathan James, a 15-year-old hacker from Florida, USA. He went by the online pseudonym “c0mrade” (abc News, 2000). In June 1999 he stole a piece of software from NASA which controlled the international space station’s physical environment including humidity and temperature. The attacker was found and charged with six months in prison, making him the first young hacker to be incarcerated for computer crimes.

## Negative impact of the attack

James was able to download “$1.7 million in NASA propriety software used to support the International Space Station’s physical environment […] within the living quarters” (Cohen, 2021). If used, this software could have the potential to put NASA astronauts in immediate danger. Because of this, NASA had to shut down the systems in the space station for 21 days to recover. This cost NASA $41,000 in contractor labour and replaced equipment.

## Attack Agent

James found an unknown vulnerability on a government server in Virginia which allowed him to intercept thousands of messages between DTRA employees. Using this collected credential data, he carried out privilege escalation attacks to access many government computers, including ones operated by NASA at the Marshall Space Flight Center in Alabama. From there, he downloaded the software used to control the physical environment within the International Space Station.

## Categorisation in the STRIDE model

#### Spoofing
* James collected credentials by intercepting messages between employees.
* The enabling vulnerability was the use of unencrypted messaging between employees.

#### Tampering
* N/A

#### Repudiation
* N/A

#### Information Disclosure
* He intercepted private messages that he was not authorised to read
* The enabling vulnerability again was the use of unencrypted messaging between employees.

#### Denial of Service
* N/A

#### Escalation of Privilege
* Once James had access to a government server he was able to put in a back door which enabled him to bypass levels of authentication to other government servers including ones owned by NASA.
* The enabling vulnerability has not been disclosed.

## What measures have been put in place as a result of the attack?

Any measures taken after this attack have not been made clear to the public. However, we can hopefully assume that message encryption has been implemented.

## Bibliography
abc News. (2000, September 21). 15-Year-Old Admits Hacking NASA Computers. Retrieved from abc News: https://abcnews.go.com/Technology/story?id=119423&page=1

Cohen, G. (2021). Florida teen hacks the Department of Defense and NASA. Industrial Cybersecrutiy Pulse.

Empist. (2021, October 15). Cybersecurity Scary Stories: Infiltrating NASA. Retrieved from Empist: https://empist.com/cybersecurity-scary-stories-infiltrating-nasa/

Rohit Sharma, D. M. (2017). Cyber Attacks That Shook the World. IJSRD - International Journal for Scientific Research and Development, 2.

## Credit

* Lizzie Hamer
* Anthony Clermont
