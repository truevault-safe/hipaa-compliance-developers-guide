# Mobile Applications and HIPAA Compliance

Pundits estimate that there are more than 40,000 health-related applications in AppStores everywhere. That's a lot of apps for an industry that by all accounts is just starting to get its bearings when it comes to consumer technology.

That number is sure to grow, particularly if Apple goes full on ahead with its rumored Healthbook—which is a health-related version of its integrated Passbook application.

For sure, mobile makes a ton of sense to be the platform of choice for the next generation of patient health management tools. Tablet sales are skyrocketing past PCs, more smartphones are being sold to more people, and the very notion of health management lends itself to a device that you have with you all the time.

Building a health-related mobile application does have some challenges of its own, particularly as it relates to HIPAA compliance. These special cases are why we've added this section just about mobile application development and HIPAA compliance.

## Use cases

As we mentioned under [Developer Considerations](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/08%20Developer%20Considerations.md) a thorough understanding of your application use cases is essential. We won't rehash it all here, but definitely read up on it in the link above.

Needless to say, it’s important to consider whether or not your app will be used to store or transmit protected health information, regardless of how you’ve designed it or anticipate it being used.

Even if you’ve designed your app to collect or use anonymous data that doesn’t fall under HIPAA by itself, if a user chooses to use your app to transmit PHI to a doctor then you are subject to HIPAA compliance requirements. Edge case or not, as soon as PHI is involved your app falls under HIPAA.

If your application has the chance to be used to store and transmit PHI it’s a safer bet to be HIPAA compliant to protect yourself from inadvertently violating HIPAA guidelines.

## PHI in the application

PHI is information that could be used to identify an individual and that relates to their physical or mental health, any healthcare services they have received and any information regarding the payment for such services.

The fact that an individual has received services from a covered entity is itself PHI. Likewise, the name or address of an individual, although publicly available, is also PHI when it’s on a covered entity’s computer simply because its presence suggests that the individual is or was a patient.

PHI can also include what would otherwise be anonymous information. This includes a date of service i.e. anything more specific than a year.

If you store, collect, manage, or transmit any protected health information to covered entities then your app needs to be HIPAA compliant.

## User communication

This is another area where developers can get tripped up when it comes to HIPAA compliance. We're so used to building in email and app notifications that questioning whether they can be used at all, or in a compliant manner, is a foreign concept.

The very premise of the HIPAA is to protect sensitive information, so it is paramount that you consider how you will communicate with subscribers once they are using your app.

### Email
Consider email. Emails are usually not compliant with HIPAA as they often lack the ability to encrypt their contents. Therefore sending information that may contain PHI via email is a HIPAA violation.

Because many applications use email as a communication source with users, it’s important to understand what can and can’t be included in those communications.

If you are sending email communications that include or might include protected health information from your mobile app you should send those emails via a HIPAA compliant email service provider.

### Database/API calls
If your application is relying on data from any covered entity (such as a doctor's office) it will have to be compliant. Same goes for any integration you need to do with a business associate of a covered entity.

If your app is not compliant these covered entities will not be able to grant your app access to make API or database calls, nor can you search and read anything within their database.

Captain obvious says "This greatly limits the functionality of your application."

## Push notifications

As we have said before, mobile phones are particularly insecure devices and the native push notifications that are used by many applications to notify users of updates and changes run the risk of violating the privacy regulations outlined in HIPAA.

If you’re using notifications in your mobile app, it’s critical that you do not include any PHI in any push notifications from your app as they can appear and be publicly visible even when a phone is locked.

This goes beyond just mobile push notifications. Any time you’re making an automated, outbound push message (whether it be mobile, email, or automated calling) the same rules apply. Make sure you evaluate all communication touch points for potential PHI/HIPAA issues.

## Physical phone security

Phones are prone to being stolen, left in the back of cabs, on the table at restaurants, and pretty much everywhere else. Because of the natural lack of security of the phone itself you need to ensure that PHI isn't easily accessible to unauthorized users.

Unfortunately, as a mobile app developer, most of this is out of your hands. However you can take a few small steps to help users ensure their PHI is protected if they should lose their phone.

### Using the lock screen

In order to secure data on an iPhone (for example), users must use a passcode to lock the handset when not in use. You can’t control whether a user enables this functionality, but you can recommend that users who install your app enable the feature.

An easy way to do this is suggest that the user turns on the passcode lock setting in your welcome email to new account holders.

### Enabling remote wiping of lost phones

Again, not something you can control yourself, but as in the example above you can help users make their phones more secure by taking advantage of some of the built-in functionality of their device.

#### Navigation

[Chapter 8: Developer Considerations](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/08%20Developer%20Considerations.md) | [Chapter 10: Wearable Applications](https://github.com/truevault/hipaa-compliance-developers-guide/blob/master/10%20Wearable%20Applications.md)
