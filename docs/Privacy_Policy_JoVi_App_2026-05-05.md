# Privacy Policy for the JoVi App

Legal version: 2026-05-11.de-en.v1
Approved for app version: 2.1.1+261461412

Version date: 05.05.2026

## 1. Controller

The controller responsible for the processing of personal data within the meaning of the General Data Protection Regulation is:

Johannes Vilsmeier  
Blütenstr. 11  
71384 Weinstadt  
Email: developer.joviapp@gmail.com  
Privacy contact: developer.joviapp@gmail.com

## 2. Subject Matter of the App

The JoVi App is an app for order handling, team coordination, and statistics workflows in gastronomy, event, or club environments. According to the reviewed project status, there are in particular two usage modes:

- local solo mode with storage on the end device
- cloud-supported team mode with sign-in, team management, shared orders, activity logs, statistics, and optional Pro subscriptions

## 3. Processed Data

### 3.1 Locally Stored Data

In local operation, the app stores data especially using local app storage, Hive, and SharedPreferences. This may in particular include:

- menus and menu items
- table orders
- cashier and payment data
- table layout and table names
- app settings, language, UI scaling, and other usage preferences
- local markers, read states, and hidden states within the app
- local history information regarding left teams

As a rule, these data remain on your end device unless you use cloud, export, or sharing functions.

### 3.2 Account and Sign-In Data

When using cloud or Pro features, the app processes authentication and profile data through Firebase Authentication. Depending on the selected login method, the following may in particular be processed:

- user ID (UID)
- display name
- email address
- profile image URL
- information on whether an account is used anonymously

The current code provides logins via Google, Apple, and anonymous login for certain scenarios.

### 3.3 Team and Collaboration Data

In team mode, data are processed in Firebase Firestore. Depending on use, this may in particular include:

- team name
- admin ID
- invitation or join code
- team status and creation and closure timestamps
- member data such as display name, initials, role, membership status, and join or leave timestamps
- join requests with display name and request timestamp
- shared menus
- table orders
- payment records
- table configurations
- activity and system logs with text, timestamp, sender name, sender ID, and metadata
- derived daily snapshots for statistical purposes
- membership entries under the respective user account

If users enter personal data in free-text fields or team names, the app may also process such content.

### 3.4 Subscription and Purchase Data

When using paid Pro features, the app processes subscription-related data. According to the reviewed code, this may in particular include:

- subscription product ID
- purchase platform
- purchase ID or transaction-related identifier
- server-side validation data of the respective store purchase
- validation status and validation timestamp
- subscription expiration date
- assignment of a purchase token to a user ID
- Pro status of the user account

The actual payment processing takes place through the respective app store. According to the recognizable project status, complete payment data such as credit card or bank details are not stored by the app itself.

Independently of this, the app processes its own subscription-related evidence, verification, and status data insofar as this is necessary for the technical validation of a purchase, abuse prevention, assignment of a purchase to a user account, and enabling or restricting Pro features. This may in particular include purchase proofs submitted in Firestore, server-side validation results, token assignments, and Pro subscription status fields.

According to the current technical implementation, these data categories are handled with different retention periods. Short-lived technical error and verification records for submitted purchase proofs are retained for a shorter period than successfully validated purchase proofs. Pure token mappings used to assign later store events to user accounts may be retained longer than the receipt records themselves.

### 3.5 Export, Import, and Sharing Data

The app offers export, import, download, open, and share functions. In this context, the following may in particular be processed or transferred to targets selected by you:

- menu files in `.jovi` format
- CSV, HTML, and PDF exports
- statistics files
- contents from local or cloud-based data sets

If you use a share, open, or save function, data are transferred to the target app, file storage, or system function selected by you. From that point on, their data protection conditions additionally apply.

### 3.6 Camera and Scan Functions

The current code uses a scanner function for QR-based or camera-supported processes. The camera is only used if you actively call the corresponding function.

### 3.7 Technical and Operational Data

To provide the app, technical metadata may also be processed, in particular:

- platform and operating system context
- app version and build number
- timestamps of processes
- error and status information within app and cloud workflows
- permission and security status for access to cloud data

According to the reviewed code, there is no separate use of advertising tracking, advertising SDKs, or classic user profiling.

## 4. Purposes of Processing

We process data in particular for the following purposes:

- providing the app functions
- storing and synchronizing orders, menus, team data, and statistics
- user sign-in and account management
- team management and traceability of team activities
- checking and enforcing permissions and security rules
- processing and validation of Pro subscriptions
- export, import, opening, and sharing of content at the user's request
- error analysis, abuse prevention, and technical stability

## 5. Legal Bases

Where the GDPR applies, we rely in particular on the following legal bases for processing:

- Art. 6(1)(b) GDPR for providing app functions contractually requested or requested as part of pre-contractual measures
- Art. 6(1)(f) GDPR for security, abuse prevention, stability, and administrative purposes
- Art. 6(1)(a) GDPR where you voluntarily use functions such as external sharing, camera usage, or certain login procedures
- Art. 6(1)(c) GDPR where legal retention or evidence obligations exist

If a gastronomy business, club, event organizer, or other organization uses the app with its own employees, temporary staff, or team members, that organization may itself be wholly or partially responsible under data protection law for the specific contents entered.

You may withdraw consent given at any time with effect for the future. The lawfulness of processing carried out until the withdrawal remains unaffected.

## 6. Recipients and Service Providers Used

According to the reviewed code status, the following external services are particularly used or integrated:

- Firebase Authentication for login and user accounts
- Cloud Firestore for team, order, statistics, and profile data
- Firebase Cloud Functions for server-side logic, subscription validation, and data maintenance
- Google Play or Apple App Store for in-app purchases and subscription processing
- Google Sign-In and Sign in with Apple if those login paths are used
- system or third-party apps if export, open, or sharing functions are used

If these providers process personal data in countries outside the European Union or the European Economic Area, transfers to third countries may occur. In such cases, we seek to ensure that appropriate safeguards pursuant to Art. 44 et seq. GDPR exist, in particular adequacy decisions, standard contractual clauses, or other legally recognized transfer mechanisms, insofar as they are provided by the respective provider.

The concrete data processing by these providers is governed by their data protection information and contractual terms.

## 7. Storage Locations and Retention Periods

### 7.1 Local Data

Locally stored data generally remain on your end device until you delete them in the app, uninstall the app, or reset the local storage.

### 7.2 Cloud Data for User Profiles and Team Operation

Cloud data are stored as long as necessary for the respective purpose, in particular for the ongoing provision of team and Pro features.

In addition, the reviewed Functions code reveals the following automatically recognizable periods for team data:

- Teams are checked on the server side and automatically closed 42 days after creation.
- Closed teams are recursively deleted 30 days after the closure timestamp.
- Open join requests are deleted when a team closes.
- Inactive members are limited on the server side; if a threshold is exceeded, older inactive member entries may be removed.

### 7.3 Purchase and Validation Data

Purchase and validation data are not stored uniformly, but according to their technical function:

- failed or technically suspicious receipt records are generally stored for up to 90 days
- successfully validated receipt records are generally stored for up to 180 days
- technical token mappings used to assign later store events to user accounts are generally stored for up to 365 days

These periods serve the technical validation of purchases, abuse prevention, assignment checks, handling of typical support cases, and the reliable processing of delayed store events. The decisive factor in each case is the technical necessity of the specific data type; data are not stored longer merely because the app store handled the payment.

Where statutory retention obligations, ongoing disputes, or other overriding legitimate interests require longer storage, storage may exceed these periods in individual cases. Otherwise, such data should be deleted or, where practicable, anonymized after the relevant period expires.

## 8. Security

The reviewed project status uses the following protection mechanisms in particular:

- authentication via Firebase Authentication
- Firestore Security Rules to limit access to own or team-related data
- server-side validation of subscription receipts
- server-side role and status checks for team access
- partial server-side control of privileged changes

Please note that no electronic data transmission is completely secure. You should treat access data confidentially and use appropriate protective measures on end devices.

## 9. Obligation to Provide Data

Certain data are required in order to use cloud, team, or Pro features. Without login, required profile data, or necessary team and purchase data, individual functions may be wholly or partially unavailable.

## 10. Rights of Data Subjects

Subject to the legal requirements, you have in particular the following rights:

- right of access under Art. 15 GDPR
- right to rectification under Art. 16 GDPR
- right to erasure under Art. 17 GDPR
- right to restriction of processing under Art. 18 GDPR
- right to data portability under Art. 20 GDPR
- right to object under Art. 21 GDPR
- right to withdraw consent with effect for the future
- right to lodge a complaint with a supervisory authority under Art. 77 GDPR

If you wish to exercise your rights, please use the privacy contact address stated above.

## 11. No Automated Decision-Making

According to the currently reviewed project status, no automated decision-making including profiling within the meaning of Art. 22 GDPR takes place that produces legal effects concerning you or similarly significantly affects you.

## 12. Notes for Commercial or Organizational Use

If you use the app in the context of a business, club, or other organization and enter personal data of employees, temporary staff, team members, guests, or other third parties, you may have your own data protection obligations. These may in particular include:

- your own information duties toward affected persons
- verification of a suitable legal basis
- internal deletion and authorization concepts
- contractual or organizational arrangements within the business where necessary

## 13. Changes to This Privacy Policy

We may adapt this Privacy Policy if app functions, services used, legal requirements, or data flows change. The current version should be made available in the app, in the store listing, or on an associated website.

## 14. Contact

Questions about data protection may be sent to:

developer.joviapp@gmail.com
