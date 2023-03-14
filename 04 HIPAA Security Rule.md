# The HIPAA Security Rule

Outlines national security standards intended to protect health data created, received, maintained, or transmitted electronically.

## 3 Parts to the HIPAA Security Rule

1. Administrative Safeguards
2. Technical Safeguards
3. Physical Safeguards

### Administrative Safeguards

The administrative components are really important when implementing a HIPAA compliance program; you are required to:

+ Assign a privacy officer
+ Complete a risk assessment annually
+ Implement employee training
+ Review policies and procedures
+ Execute Business Associate Agreements (BAAs) with all partners who handle protected health information (PHI)

Companies like [Accountable](http://accountablehq.com) can help with the administrative components of a compliance program.

+ Accountable -- http://accountablehq.com
+ Compliance Helper -- http://www.compliancehelper.com
+ Compliancy Group -- http://compliancy-group.com
 
For more information, see [Administrative Safeguards](https://www.hhs.gov/sites/default/files/ocr/privacy/hipaa/administrative/securityrule/adminsafeguards.pdf?language=es) from the [HIPAA Security Rule Educational Paper Series](https://www.hhs.gov/hipaa/for-professionals/security/guidance/index.html#:~:text=Security%20Rule%20Educational%20Paper%20Series)


### Technical Safeguards

Technical safeguards outline what your application must do while handling PHI. 

While there are both required and addressable elements to these safeguards you should implement them all. Addressable elements (such as automatic logoff) are really just best practices. 

#### Access Control Requirements

+ Unique User Identification (required): Assign a unique name and/or number for identifying and tracking user identity.
+ Emergency Access Procedure (required): Establish (and implement as needed) procedures for obtaining necessary ePHI during an emergency.
+ Automatic Logoff (addressable): Implement electronic procedures that terminate an electronic session after a predetermined time of inactivity.
+ Authentication (required): Implement procedures to verify that a person or entity seeking access to ePHI is the one claimed.
+ Encryption and Decryption (addressable): Implement a mechanism to encrypt and decrypt ePHI.

#### Transmission Security

+ Integrity Controls (addressable): Implement security measures to ensure that electronically transmitted ePHI is not improperly modified without detection until disposed of.
+ Encryption (addressable): Implement a mechanism to encrypt ePHI whenever deemed appropriate.

#### Audit and Integrity 

+ Audit Controls (required): Implement hardware, software, and/or procedural mechanisms that record and examine activity in information systems that contain or use ePHI.
+ Mechanism to Authenticate ePHI (addressable): Implement electronic mechanisms to corroborate that ePHI has not been altered or destroyed in an unauthorized manner.

For more information, see [Technical Safeguards](https://www.hhs.gov/sites/default/files/ocr/privacy/hipaa/administrative/securityrule/techsafeguards.pdf) from the [HIPAA Security Rule Educational Paper Series](https://www.hhs.gov/hipaa/for-professionals/security/guidance/index.html#:~:text=Security%20Rule%20Educational%20Paper%20Series)

### Physical Safeguards

The Physical Safeguards really have to do with who has access to PHI data and how that access is managed. Much of the Physical Safeguard requirements that developers need to worry about are handled by HIPAA compliant hosting companies (such as TrueVault, AWS, Firehost and Rackspace).

Other parts of the Physical Safeguards are handled by your internal rules around who can and can't access PHI. 

#### Facility Access Controls

+ Contingency Operations (addressable): Establish (and implement as needed) procedures that allow facility access in support of data restoration under the disaster recovery and emergency operations plan in the event of an emergency.
+ Facility Security Plan (addressable): Implement policies and procedures to safeguard the facility and the equipment therein from unauthorized physical access, tampering, and theft.
+ Access Control and Validation Procedures (addressable): Implement procedures to control and validate a person’s access to facilities based on their role or function, including visitor control, and control of access to software programs for testing and revision.
+ Maintenance Records (addressable): Implement policies and procedures to document repairs and modifications to the physical components of a facility which are related to security (e.g. hardware, walls, doors, and locks).

#### Device and Media Controls

+ Disposal (required): Implement policies and procedures to address the final disposition of ePHI, and/or the hardware or electronic media on which it is stored.
+ Media Re-Use (required): Implement procedures for removal of ePHI from electronic media before the media are made available for re-use.
+ Accountability (addressable): Maintain a record of the movements of hardware and electronic media and any person responsible therefore.
+ Data Backup and Storage (addressable): Create a retrievable, exact copy of ePHI, when needed, before movement of equipment.

#### Workstation Security

+ Workstation Security (required): Implement physical safeguards for all workstations that access ePHI, to restrict access to authorized users.
+ Workstation Use (required): Implement policies and procedures that specify the proper functions to be performed, the manner in which those functions are to be performed, and the physical attributes of the surroundings of a specific workstation or class of workstation that can access ePHI.

For more information, see [Physical Safeguards](https://www.hhs.gov/sites/default/files/ocr/privacy/hipaa/administrative/securityrule/physsafeguards.pdf) from the [HIPAA Security Rule Educational Paper Series](https://www.hhs.gov/hipaa/for-professionals/security/guidance/index.html#:~:text=Security%20Rule%20Educational%20Paper%20Series)

## Required vs. addressable specifications

Some implementation specifications are “required” and others are “addressable.” Required implementation specifications must be implemented. 

Addressable implementation specifications must be implemented if it is reasonable and appropriate to do so; your choice must be documented.

It is important to remember that an addressable implementation specification is not optional. 

**When in doubt, you should just implement the addressable implementation specifications. Most of them are best practices anyway.**

#### Navigation

[Chapter 3: Do I Need to Be HIPAA Compliant?](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/03%20Do%20I%20Need%20to%20Be%20HIPAA%20Compliant%3F.md) | [Chapter 5: Becoming HIPAA Compliant](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/05%20Becoming%20HIPAA%20Compliant.md)
