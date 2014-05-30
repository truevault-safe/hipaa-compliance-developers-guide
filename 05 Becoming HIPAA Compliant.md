# Becoming HIPAA compliant

The HIPAA Security Rule requires having the appropriate Administrative, Physical, and Technical Safeguards in place to ensure the confidentiality, integrity, and security of protected health information (PHI).

In other words, you need to cover all three bases in order to be  compliant per the HIPAA guidelines. 

## What does HIPAA require?

HIPAA as a law requires that you do the following four things.

1) Put safeguards in place to protect patient health information.

2) Reasonably limit use and sharing to the minimum necessary to accomplish your intended purpose.

3) Have agreements in place with service providers that perform covered functions. These Business Associate Agreements (BAAs) ensure that service providers (Business Associates) use, safeguard and disclose patient information properly.

4) Procedures to limit who can access patient health information, and training programs about how to protect patient health information.

## What it means for developers

If you are collecting, storing or transmitting PHI to a covered entity then you definitely should be HIPAA compliant.

If you're building an application that has any reasonable likelihood of collecting, storing or transmitting PHI you should probably be HIPAA compliant.  

Your non-technical team or (co-founder, depending on your size) should worry about the administrative compliance issues. As the developer you should focus both on the physical and technical aspects of the law.

**You can really go about it in one of three ways:**

1. Decide that you're not going to have PHI in your system and don't need to worry about HIPAA compliance. This is the easiest choice, but remember, there's no safe harbor with HIPAA. 
2. Decide that you'll build out the compliance requirements yourself. Many of the safeguards are standard parts of today's apps, login, auto-logout, etc. You can build many of these as part of your core infrastructure. Others are not so easy to build and maintain.
3. You outsource your HIPAA compliance. Using a service like TrueVault you are guaranteed compliance with the technical and physical safeguard requirements by storing any PHI in the cloud in TrueVault's secure data store. [Learn more](https://truevault.com)

## If we're being honest

It's not worth taking the risk of HIPAA compliance audits and penalties if you have even a small chance of managing PHI within your application. 

#### Navigation

[Chapter 4: HIPAA Security Rule](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/04%20HIPAA%20Security%20Rule.md) | [Chapter 6: Who Certifies HIPAA Compliance](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/06%20Who%20Certifies%20HIPAA%20Compliance%3F.md)