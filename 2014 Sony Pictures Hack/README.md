# Background

Sony Pictures Entertainment is a subsidiary of the Sony Group Corporation that produces, acquires and distributes movies and TV shows (Sony Pictures Entertainment, 2022). In 2013, the company began production on 'The Interview', a comedy movie about two journalists who are recruited by the CIA to assassinate Kim Jong-Un (Sony Pictures Entertainment, 2014). The movie faced backlash prior to its release, particularly from the North Korean government, and the controversy surrounding it led to a hacker group launching a cyber attack on the film studio.

# The Attack

On the morning of November 24th 2014, employees at Sony Pictures Entertainment's headquarters were greeted by an image of a skull along with a threatening message which appeared on all of the company's computers simultaneously and locked employees out of their devices. The message came from a hacking group known as "Guardians of Peace" and they claimed that they would release the company's "top secrets" if their demands were not met (Robb, 2014). A few days prior to this, the company had received emails demanding "monetary compensation" and threatening that the company would be "bombarded as a whole", but these went ignored (Seal, 2015). 

It quickly became apparent that the threats were serious, as huge amounts of private company data began surfacing online. This data included bosses' salaries, employees' social security information and several confidential emails sent between employees (BBC News, 2014). The leaked data also included several unreleased films, which were uploaded to file sharing websites and downloaded millions of times (Robb, 2014).

It was widely speculated that North Korea was involved with the attack as a form of retaliation against Sony's release of 'The Interview', although the hackers did not make direct reference to the movie in their communications until December 16th, over three weeks after the attack began (Robb, 2014). Additionally, the FBI linked North Korea to the attack during their investigations. North Korea would eventually deny their involvement, however they did describe the movie as an "act of terrorism" and praised the attack as a "righteous deed" (BBC News, 2014).

# The Vulnerabilities and Exploits Used

On December 19th 2014, the US government released their findings on the methods used by the attackers via US-CERT (Cybersecurity & Infrastructure Security Agency (USA), 2014). According to the report, the attackers used a Server Message Block (SMB) Worm Tool to steal Sony Pictures Entertainment's private data.

The worm propagated itself via Windows SMB shares, attempting to guess passwords for SMB connections by using brute force and, once successful, creating a copy of itself and running on the new host. The worm featured a listening implant, a lightweight backdoor, a proxy tool, a destructive hard drive tool and a destructive target cleaning tool.

The lightweight backdoor allowed the attackers to transfer files off the target machine, as well as execute code and commands. The backdoor also featured functionality which allowed it to open ports in firewalls, discover routers and add port mappings, allowing for the use of inbound connections. 

The destructive hard drive tool was able to destroy data on the target machine in such a way that essentially made it unrecoverable, this was used by the attackers to remove data from the machines once it had been stolen. In addition to this, the destructive target cleaning tool was used to overwrite the Master Boot Record, meaning that the target machine became unusable. It is believed that the attackers used the RawDisk driver to achieve their effective data wiping, a tool that was also notably used in the 2012 Shamoon attack (Zetter, 2014).

# STRIDE Model Categorisation

The primary threat in this attack was information disclosure. The attackers were able to steal huge amounts of private data from Sony Pictures Entertainment and subsequently release a significant amount of this data to the general public. This data included sensitive information about employees at the company which should never have been accessible. 

Another large element of the attack involved denial of service. Due to the destructive nature of the attack, employees of the film studio were unable to access their computers, e-mail and voicemail for an extended period of time. This left employees unable to complete their jobs as they normally would. 

Spoofing also played a role in the attack. The worm used in the attack was able to propagate via Windows SMB shares by guessing passwords in order to log in as a user and copy itself onto the target host. 

# The Aftermath

Following the threatening messages from the attackers, Sony Pictures initially cancelled their release of 'The Interview', before later opting for a limited cinema release followed by a video-on-demand release (Shaw, 2014). 

The attack led to Sony Pictures, along with many other entertainment companies, paying more attention to the importance of cyber security and improving their systems. The measures taken by entertainment companies included searching for unusual patterns to detect attacks, encrypting files regardless of where they are stored and carefully monitoring who has access to their files (Boorstin, 2015).

The US government also included some advice for companies in their report on the attack methods. This advice included implementing indicators of compromise, creating daily backups of critical systems, isolating critical systems, enforcing strong password policies, keeping software up to date and implementing two-factor authentication (Cybersecurity & Infrastructure Security Agency (USA), 2014).

# References

- Sony Pictures Entertainment (2022) *DIVISIONS | Sony Pictures Entertainment*. Available at: https://www.sonypictures.com/corp/divisions.html (Accessed: 03/10/2022)
- Sony Pictures Entertainment (2014) *THE INTERVIEW | Sony Pictures Entertainment*. Available at: https://www.sonypictures.com/movies/theinterview (Accessed: 03/10/2022)
- Robb, D. (2014) 'Sony Hack: A Timeline', *Deadline*. Available at: https://deadline.com/2014/12/sony-hack-timeline-any-pascal-the-interview-north-korea-1201325501/ (Accessed: 03/10/2022)
- Seal, M. (2015) 'An Exclusive Look at Sony’s Hacking Saga', *Vanity Fair*. Available at: https://www.vanityfair.com/hollywood/2015/02/sony-hacking-seth-rogen-evan-goldberg (Accessed: 03/10/2022)
- *BBC News* (2014) 'The Interview: A guide to the cyber attack on Hollywood'. Available at: https://www.bbc.co.uk/news/entertainment-arts-30512032 (Accessed: 03/10/2022)
- Cybersecurity & Infrastructure Security Agency (USA) (2014) *Alert (TA14-353A)*. Available at: https://www.cisa.gov/uscert/ncas/alerts/TA14-353A (Accessed: 04/10/2022)
- Zetter, K. (2014) 'Sony Got Hacked Hard: What We Know and Don't Know So Far', *Wired*. Available at: https://www.wired.com/2014/12/sony-hack-what-we-know/ (Accessed: 04/10/2022)
- Shaw, L. (2014) 'Sony to Release ‘The Interview’ in More Than 300 Theaters', *Bloomberg*. Available at: https://www.bloomberg.com/news/articles/2014-12-23/sony-to-release-the-interview-on-dec-25-theaters-say (Accessed: 04/10/2022)
- Boorstin, J. (2015) 'The Sony hack: One year later', *CNBC*. Available at: https://www.cnbc.com/2015/11/24/the-sony-hack-one-year-later.html (Accessed: 04/10/2022)