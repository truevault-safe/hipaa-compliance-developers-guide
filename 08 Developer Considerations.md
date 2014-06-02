# Developer considerations

As you're evaluating how to best deal with HIPAA you'll probably have some of these questions pop-up in your deliberations. We'll continue to add more here, but these are ones that we've heard from developers tackling HIPAA in their development process.

## Build vs. Buy

Scanning the list of safeguards required by HIPAA it's not unreasonable to think first of building out the safeguards yourself. Functionality such as unique identifiers for users and automatic logoff are part of any application anyway, so building those is going to happen one way or another. 

Couple that with HIPAA compliant hosting providers, and it's easy to draw the conclusion that a combination of an AWS instance and some best practice application security wouldn't do the trick.

Unfortunately, the other pieces of the security rule safeguards aren't as easy to address or maintain and can take a ton of people-power and time to build out not just the features but the audit and logging functionality as well. 

We think this comment from Hacker News sums up the technical debt required to roll your own HIPAA compliant infrastructure quite accurately. This was completely unsolicited and is not from a TrueVault customer. 

> 	“[Building our own HIPAA compliant infrastructure] took upwards of 1,000 person-hours to figure out HIPAA-compliance issues. This will continue to be an ongoing cost for us, because HIPAA is an ongoing law 	and it changes sometimes. It takes substantial auditing time and money." — jph

Looking at it as a 1,000 hour project is one way to evaluate the true cost of rolling your own compliance infrastructure, not to mention the ongoing audit and maintenance costs associated with your in-house solution.

## Unintended use cases

As we've mentioned before, HIPAA isn't like the DMCA, there is no safe harbor clause for unintended transmission, storage or disclosure of PHI. Regardless of how you planned it, scoped it, envisioned it or dissuaded users from including it—if PHI is in your app or on your servers you could face HIPAA fines if you're not in compliance.

It's not as big of an edge case as you might think. Here's a few examples of how easily PHI can enter into your application.

+ Your app to get doctor's advice based on anonymous symptoms could easily have PHI as soon as the patient shares an email address, lab report, or last doctor visit.
+ Your diabetes management app which tracks your blood sugar and prescription information has a note added by the user of their doctor's dosing instructions and pharmacy Rx number.

You get the idea. Regardless of how you intend for the user to use your application, there is a pretty decent chance that if the application is related to personal health in any way, PHI will ultimately end up in the system.

## HIPAA Hosting and compliance

HIPAA hosting refers to website, application or data storage and hosting services that comply with the physical safeguard requirements of the HIPAA security rule. 

HIPAA hosting is an important part of the requirements needed for application developers to ensure HIPAA compliance of their solutions. 

### Does Using HIPAA Hosting Make My Application HIPAA Compliant?

**The short answer is no. HIPAA hosting alone does not make you HIPAA compliant.**

Compliance is determined by the adherence to the privacy and security rules outlined by HIPAA. HIPAA Hosting only addresses one aspect of those requirements. 

Hosting your application in a HIPAA compliant hosting environment such as Amazon AWS or Firehost does not make your application HIPAA compliant as they only address the physical safeguard requirements of the HIPAA security rule.

You are still required to meet the administrative and technical specifications of the HIPAA Security Rule in order to be compliant. 

### What Data Should Be Stored in HIPAA Compliant Hosting Environments? 

Not all of your application data needs to exist in a HIPAA hosting environment. But any PHI must be in a HIPAA compliant environment. 

[Examples of PHI](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/02%20What%20is%20HIPAA%3F.md#protected-health-information-phi)

### What Makes a Hosting Environment HIPAA Compliant?

HIPAA compliant hosting providers typically provide two main aspects of HIPAA compliance:

They sign a Business Associate Agreement with you, which is required by service providers managing and handling HIPAA protected information. [Learn more about Business Associate Agreements](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/02%20What%20is%20HIPAA%3F.md#business-associate).

They address many of the Physical Safeguard requirements of the HIPAA Security rule. [See a complete list of physical safeguards](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/04%20HIPAA%20Security%20Rule.md#physical-safeguards).

### Network and application security

Ensuring your hosting environment is HIPAA compliant is only the first step. You must also implement network and application security best practices to protect your hosting environment.

Health information is a popular commodity for hackers. According to a recent [Information Week article](http://www.informationweek.com/healthcare/security-and-privacy/healthcare-it-security-worse-than-retail-study-says/d/d-id/1269207), each health record could be worth as much as $20 on the black market. 

It's easy to imagine hackers trying to breach your servers when your application becomes popular. You need to be sure your HIPAA  hosting environment is locked down and secure from unauthorized access attempts.

### High-Availability and Redundancy

A good infrastructure design eliminates all single-point-of-failures. While running one web server and one database server may save you money in the short run, how much would it cost your business if that one web server goes offline causing the entire hosting environment to crumble? 

It's best to design your hosting environment with at least 2 web servers behind a load balancer and 2 database servers on a active/passive failover setup. 

Clearly most environments are more complicated than just a 2-tier setup, so you must implement an infrastructure design best suited for your business. But the point remains, high-availability and redundancy are crucial parts of your HIPAA compliant infrastructure.

### Required vs. Addressable HIPAA Implementation Specifications

We've talked about the [difference between required and addressable specifications](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/04%20HIPAA%20Security%20Rule.md#required-vs-addressable-specifications) already, but most HIPAA hosting companies should implement the addressable specifications as they are best practice data security features any way.

#### Navigation

[Chapter 7: HIPAA Fines](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/07%20HIPAA%20Fines.md) | [Chapter 9: Mobile Applications](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/09%20Mobile%20Applications.md)
