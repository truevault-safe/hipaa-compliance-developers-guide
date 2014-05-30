# HIPAA Fines

HIPAA violations are expensive. The penalties for noncompliance are based on the level of negligence and can range from $100 to $50,000 per violation (or per record), with a maximum penalty of $1.5 million per year for violations of an identical provision. Violations can also carry criminal charges that can result in jail time.

Fines will increase with the number of patients and the amount of neglect. Starting with a breach where you didn’t know and, by exercising reasonable diligence, would not have known that you violated a provision. To the other end of the spectrum where a breach is due to negligence and not corrected in 30 days. In legalese, this is known as mens rea (state of mind). So fines increase in severity from no mens rea (didn’t know) to assumed mens rea (willful neglect).

The fines and charges are broken down into 2 major categories: “Reasonable Cause” and “Willful Neglect”. Reasonable Cause ranges from $100 to $50,000 per incident and does not involve any jail time. Willful Neglect ranges from $10,000 to $50,000 for each incident and can result in criminal charges.

**HIPAA violation categories and their respective penalty amounts are outlined in the chart below:**

![hipaa violations summary](https://dg80atg7s3qsy.cloudfront.net/blog/img/hipaa-violations.png)

Source: HHS, Federal Register.gov

## Unencrypted Data
While encryption is an addressable (rather than required) specification, it does not mean optional. The vast majority of data breaches are due to stolen or lost data that was unencrypted. When in doubt, you should implement the [addressable implementation specifications](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/04%20HIPAA%20Security%20Rule.md#required-vs-addressable-specifications) of the Security Rule. Most of them are best practices.

## Employee Error
Breaches can occur when employees lose unencrypted portable devices, mistakenly send PHI to vendors who post that information online, and disclose personally identifiable, sensitive information on social networks. 

These are all examples from actual cases. Employee training and adherence to security policies and procedures is extremely important.

## Data Stored on Devices
Almost half of all data breaches are the result of theft. When laptops, smartphones, etc. are unencrypted the risk of a breach increases considerably. With TrueVault, your data is safely stored off-premise; so that stolen laptop just has a token on it, and no PHI is compromised.

## Business Associates
Almost two-thirds of data breaches involved a business associate. Meaning that you delegated a covered function or activity to someone, and that someone messed up. So pick your partners carefully. 

Some of the largest breaches reported to HHS have involved business associates. As a result, the final omnibus rule expanded many of the requirements to business associates and greatly enhanced the government’s ability to enforce the law.

**What sort of penalties are we talking about? Check out this chart with fines levied in years past:**

![hipaa fines table](https://dg80atg7s3qsy.cloudfront.net/blog/img/hipaa-fines.png)

Source: HHS, Case Examples and Resolution Agreements

Looking at this chart we can conclude that HHS does not like people storing unencrypted PHI on mobile devices. What we don’t see yet are fines levied against business associates. 

2014 is the first year where business associates will be audited and fined. Smart money says that the first fines levied against business associates will be passed down toward the end of this year.

If these fines make you nervous, then this might be a good time to revisit your decision about whether your application needs to be HIPAA compliant or not.

The good news is that not every PHI breach ends in a fine. If you can show that you have made a reasonable effort to comply with HIPAA then you may not be dinged.

#### Navigation

[Chapter 6: Who Certifies HIPAA Compliance](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/06%20Who%20Certifies%20HIPAA%20Compliance%3F.md) | [Chapter 8: Developer Considerations](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/08%20Developer%20Considerations.md)