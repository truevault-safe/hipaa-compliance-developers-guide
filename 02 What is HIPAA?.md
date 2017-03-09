# What is HIPAA?

HIPAA is short for the **Health Insurance Portability and Accountability Act**.

HIPAA sets the standard for protecting sensitive patient data. The law states that Covered Entities and their Business Associates need to protect the privacy and security of protected health information (PHI).

## Background
 
Developed in 1996 HIPAA was initially created to help the public with insurance portability. Back in the day you couldn't easily switch insurances if you didn't like the coverage or doctors that provided services under that insurance. It was a huge pain getting your medical records from one practitioner to another.

Along with portability came privacy concerns, so the law makers built in a series of privacy tools and requirements to protect healthcare data.

## 2013 Final Omnibus Rule Update 
In September of 2013, the [Final Omnibus Rule Update](http://en.wikipedia.org/wiki/Health_Insurance_Portability_and_Accountability_Act#cite_note-33) was passed that amended HIPAA and greatly expanded the definition of who needed to be HIPAA compliant. Previously, only covered entities (such as doctors, hospitals, and insurers) were required to be HIPAA compliant. 

With the recent rule change however, all entities that store, manage, record or pass Protected Health Information (we'll just call it PHI from now on) to and from covered entities are also required to be HIPAA compliant. 

These entities, called Business Associates, who were previously exempt from HIPAA, now fall under its governance.

## The Four Rules of HIPAA

Like the four horsemen, these are the major pieces that govern what you do and how you do it.

+ HIPAA Privacy Rule
+ HIPAA Security Rule
+ HIPAA Enforcement Rule
+ HIPAA Breach Notification Rule


**Developers need to focus on the Technical and Physical safeguards outlined in the Security Rule.**

## Important terms to know

### Protected Health Information (PHI)

You will hear this term non-stop when dealing with applications that can store health information. It's typically called PHI although some parts of the law refer to digitally-stored PHI as ePHI. We'll stick with PHI for consistency. 

PHI is any information in a medical record that can be used to identify an individual, and that was created, used, or disclosed in the course of providing a health care service, such as a diagnosis or treatment. 

In other words, PHI is information in your medical records, including conversations between your doctors and nurses about your treatment. PHI also includes your billing information and any medical information in your health insurance company's computer system.

Some examples of PHI:

+ Billing information from your doctor
+ Email to your doctor's office about a medication or prescription you need.
+ Appointment scheduling note with your doctor's office
+ An MRI scan
+ Blood test results
+ Phone records

Examples of non-PHI data:

+ Number of steps in a pedometer
+ Number of calories burned
+ Blood sugar readings w/out personally identifiable user information (PII) (such as an account or user name)
+ Heart rate readings w/out PII

### The Difference Between Protected Health Information and Consumer Health Information

So how do you know if you’re dealing with protected health information (PHI) or consumer health information? The test is pretty simple: if your device or application stores, records or transmits the user’s personally-identifiable health data held in the app or device to a covered entity (see below) then you are dealing with protected health information and need to be HIPAA compliant.

If you are building a wearable device or application that collects health information, but does not plan on sharing it with a covered entity at any point in time then you do not need to be HIPAA compliant. 

For example, the Nike Fuel Band is not HIPAA compliant because it does not track data considered protected health information because you can't transmit that data from the device to a covered entity. 

### Covered Entity

A covered entity is anyone who provides treatment, payment and operations in healthcare. 

According to the U.S. Department of Health & Human Services (HHS) Healthcare Providers, Health Plans, and Healthcare Clearinghouses are all Covered Entities. 

This one is pretty straightforward. Healthcare Providers are exactly who you might think: hospitals, doctors, clinics, psychologists, dentists, chiropractors, nursing homes, and pharmacies are considered Healthcare Providers and need to be HIPAA compliant.

Examples of Health Plans include health insurance companies, HMOs, company health plans, Medicare, and Medicaid. In addition, employers and schools that handle PHI in order to enroll their employees and students in health plans fall under the definition of a Health Plan and need to be HIPAA compliant.

Healthcare Clearinghouses are a little more esoteric. A Clearinghouse takes in information from a healthcare entity, puts the data into a standard format, and then spits the information back out to another healthcare entity. They need to be HIPAA compliant too.

Covered Entities Include: 

+ Doctor’s office, dental offices, clinics, psychologists, 
+ Nursing home, pharmacy, hospital or home healthcare agency
+ Health plans, insurance companies, HMOs
+ Government programs that pay for healthcare
+ Health clearing houses

### Business Associate

Simply put, a Business Associate is a vendor or subcontractor who has access to PHI.

A more legalese definition of a Business Associate is any entity that uses or discloses PHI on behalf of a Covered Entity. Furthermore, a Business Associate is any person who, on behalf of a Covered Entity, performs (or assists in the performance of) a function or activity involving the use or disclosure of PHI.

The vendors that we are talking about can be data storage or document storage services (doesn’t matter if they can view the PHI that they maintain), providers of data transmission services, portals or other interfaces created on behalf of Covered Entities that allow patients to share their data with the Covered Entity, and electronic heath information exchanges.

If a Business Associate (vendor) delegates a covered function or activity to someone, then that entity is considered a subcontractor.

Some vendors avoid PHI like the plague; they don’t want this information anywhere near their service. But, avoidance doesn’t necessarily excuse a vendor from becoming compliant. 

If a Covered Entity (customer) sends PHI through a vendor, and the vendor’s servers store this information, then they are considered a Business Associate and subject to the HIPAA Security Rule. 

#### No safe harbor clause

Unlike other laws (DMCA anyone?) there is no "safe harbor" here. Just because you don't want to handle PHI doesn't opt you out of HIPAA compliance requirements. 

Further, just refusing to sign a Business Associate Agreement doesn't absolve you of the provisions of HIPAA compliance should your services handle PHI (intentionally or not) in any way. 

Here are some examples of potential Business Associates:

+ Data processing firms or software companies that may be exposed to or use PHI
+ Medical equipment service companies handling equipment that holds PHI
+ Shredding and/or documentation storage companies
+ Consultants hired to conduct audits, perform coding reviews, etc.
+ Lawyers
+ External auditors or accountants
+ Professional translator services
+ Answering services
+ Accreditation agencies
+ e-prescribing services
+ Medical transcription services

In contrast, these folks are NOT Business Associates:

+ Covered Entity’s Workforce
+ Individuals or companies with very limited and incidental exposure to health information, such as a telephone company, electrician, etc.
+ Companies that act as a conduit for PHI, such as the postal service, UPS, private couriers, etc.

#### Navigation

[Introduction](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/01%20Introduction.md) | [Chapter 3: Do I Need to Be HIPAA Compliant?](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/03%20Do%20I%20Need%20to%20Be%20HIPAA%20Compliant%3F.md)
