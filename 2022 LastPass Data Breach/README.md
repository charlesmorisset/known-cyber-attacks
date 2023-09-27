# 2022 LastPass Breach
---
## Overview
Lastpass suffered two breaches in 2022<sup>[1]</sup>, this page focuses on the one with greater impact, the second breach.

By targeting a DevOps engineer, unauthorized access was gained to cloud backups. These backups contained a wide range of data, including customer data (encyrpted and unencrypted)

## Details of attack
A DevOps engineers personal computer was targeted via their installation of Plex Media Server. The installation was many versions behind the most recent version at the time, and was missing security updates.<sup>[3]</sup>

The specific vulnerability targeted was [CVE-2020-5741](https://nvd.nist.gov/vuln/detail/CVE-2020-5741), which allowed arbitrary python code to be executed on the local system, from the current system user.<sup>[3]</sup>

To exploit this vulnerability, valid credentials for a Plex account are required by the attacker, these were leveraged in some way from the engineer<sup>[2][3]</sup>

The python code exeution was used to install keylogger software, which was used to capture the engineer's master password for their LastPass Vault. This vault contained secure notes describing how to access critical information for LastPass, and necessary decryption keys.<sup>[3]</sup>

LastPass became aware of the breach after warnings from Amazon of anomalous behaviour<sup>[4]</sup>

*Attacker Unknown*

## Categorisation

This is an attack with many steps, so can fall into multiple STRIDE catagories

- A **spoofing** attack was made on the DevOps engineer's Plex installation, and multiple other times, using the credentials extracted from the engineer's vault
- There was an attempt at **Tampering** when the attacker tried to access Cloud Identity and Access Management roles<sup>[4]</sup>
- There is a risk of **Information disclosure** as the information extracted during the breach could be made public, or sold. There's even a risk of some password being brute force decypted<sup>[6]</sup>


## Negative Impact
The data taken includes (but is not limited to):<sup>[5]</sup>

- **Encrypted** customer vaults
- Customer account secrets
	+ API keys
	+ One time pads
	+ Seeds for one time pads
- Customer information
	+ Including billing address, names and ip address
	+ Also including Information about Vault encryption configurations
	
LastPass operated with a breach-assumption policy<sup>[6]</sup>, meaning that all vault data is secure under the event of a breach. The vault is secured via 256 bit AES encryption using a hashed version of the master password as a key<sup>[7]</sup> and therefore the vault is only susceptible to a brute force attack. So long as a user uses a secure master password, and keeps their password secret, their vault data should be safe.

However, much of the other data extracted is still valuable for a malicious party

The key impact for LastPass will be the substantial reputation hit that they have taken, a password manager such as LastPass, that stores data on the cloud is dependent on customer trust, especially considering this is one of two data breaches that took place, so close together.
See [this](https://www.wired.com/story/lastpass-breach-vaults-password-managers/) article from WIRED, titled "It's Time to Ditch This Password Manager" (sorry about the paywall)


## Measures Implemented
Below is a list of measures that have been implemented as a result of this breach, from the LastPass incident report:<sup>[2]</sup>

<blockquote>

- With the assistance of Mandiant, we forensically imaged devices to investigate corporate and personal resources and gather evidence detailing potential threat actor activity.
- We assisted the DevOps Engineer with hardening the security of their home network and personal resources.
- We enabled Microsoft’s conditional access PIN-matching multifactor authentication using an upgrade to the Microsoft Authenticator application which became generally available during the incident.
- We rotated critical and high privilege credentials that were known to be available to the threat actor; we continue to rotate the remaining lower priority items that pose no risk to LastPass or our customers.
- We began revoking and re-issuing certificates obtained by the threat actor.
- We analyzed LastPass AWS S3 cloud-based storage resources and applied or started to apply additional S3 hardening measures:

	- We put in place additional logging and alerting across the Cloud Storage environment with tighter IAM policies enforced.
	- We deactivated prior development IAM users.
	- We enabled a policy that prevents the creation and use of long-lived development IAM users in the new development environment.
	- We rotated existing production service IAM user keys, applied tighter IP restrictions, and reconfigured policies to adhere to least privilege.
	- We deleted obsolete service IAM users from the development and production environments.
	- We are enabling IAM resource tagging enforcement on accounts for both users and roles with periodic reporting on non-compliant resources.

- We rotated critical SAML certificates used for internal and external services.
- We deleted obsolete/unused SAML certificates used for development, services, or third parties.
- We revised our 24x7 threat detection and response coverage, with additional managed and automated services enabled to facilitate appropriate escalation.
- We developed and enabled custom analytics that can detect ongoing abuse of AWS resources.
</blockquote>

## References

[1][Security incident update - LastPass](https://blog.lastpass.com/2023/03/security-incident-update-recommended-actions/)

[2][Incident additional details - LastPass](https://support.lastpass.com/s/document-item?bundleId=lastpass&topicId=LastPass/incident-2-details.html&_LANG=enus)

[3][LastPass Hack: Engineer's Failure to Update Plex Software Led to Massive Data Breach - Ravie Lakshmanan](https://support.lastpass.com/s/document-item?bundleId=lastpass&topicId=LastPass/incident-2-details.html&_LANG=enus)

[4][LastPass says employee’s home computer was hacked and corporate vault taken](https://arstechnica.com/information-technology/2023/02/lastpass-hackers-infected-employees-home-computer-and-stole-corporate-vault/)

[5][What data was accessed? - LastPass](https://support.lastpass.com/s/document-item?language=en_US&bundleId=lastpass&topicId=LastPass/incident-data.html&_LANG=enus)

[5][LastPass data breach - University of Washington](https://ciso.uw.edu/2022/12/23/lastpass-data-breach/)

[6][LastPass technical whitepaper - LastPass](https://support.lastpass.com/s/document-item?bundleId=lastpass&topicId=LastPass/lastpass_technical_whitepaper.html&_LANG=enus)


