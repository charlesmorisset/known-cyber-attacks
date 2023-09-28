# CD Projekt RED Ransomware attack 08/02/21

## General

On the 8th of February 2021, CD Projekt RED suffered a ransomware attack [1].

CD Projekt RED posted about the incident on Twitter [1], stating: 

>“An unidentified actor gained unauthorized access to our internal network, collected certain data belonging to CD PROJEKT capital group, and left a ransom note the content of which we release to the public.” [1].

This article [3] by the BBC covers the attack and the context surrounding CD Projekt RED at that time. 

On the 10th of June 2021, CD Projekt RED posted a further post on Twitter regarding the incident [2]. This post [2] described their actions taken due to this attack and placed a large focus on the data of employees.

## Exploit

The ransomware used against CD Projekt RED was HelloKitty [4]. 

This article [4] describes concisely how the ransomware works, including that:

>“Specific encryption recipes and routines can vary across variants of HelloKitty. Generally speaking, they tend to use a combination of AES-256 and RSA-2048 or even NTRU+AES-128.” [4].

The severity of the ransomware was clarified by CD Projekt RED, who stated: “Although some devices in our network have been encrypted, our backups remain intact.” [1].

## STRIDE Model

Information Disclosure – Data was taken by the attackers [1, 2]. On the 10th of June 2021, CD Projekt RED stated: 

>“We are not able to confirm the exact contents of the data in question, though we believe it may include current/former employee and contractor details in addition to data related to our games.” [2].

Elevation of privilege – CD Projekt RED describes this in their Twitter post [1], stating: “An unidentified actor gained unauthorised access to our internal network” [1].

## References

[1] @CDPROJEKTRED, “Important Update.” Twitter. Feb. 9, 2021. https://twitter.com/CDPROJEKTRED/status/1359048125403590660 (accessed Sep. 28, 2023).

[2] @CDPROJEKTRED, “IMPORTANT UPDATE.” Twitter. Jun. 10, 2021. https://twitter.com/CDPROJEKTRED/status/1403059158065295361 (accessed Sep. 28, 2023).

[3] C. Criddle. “Cyberpunk 2077 makers CD Projekt hit by ransomware hack.” *BBC News*. Accessed: Sep. 28, 2023. [Online]. Available: https://www.bbc.co.uk/news/technology-55994787

[4] SentinelOne. “Hello Kitty.” *SentinelOne*. Accessed: Sep. 28, 2023. [Online]. Available: https://www.sentinelone.com/anthology/hello-kitty/