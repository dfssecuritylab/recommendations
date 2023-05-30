# Unauthorized access to DFS data

The ability of an attacker to gain unauthorized access to DFS users' DFS data.

**Risk:** Unauthorized access to DFS user mobile data

## Affected entity: MNO

* **Vulnerability:** Inadequate user account access control mechanisms (SD: Access Control)
  * [ ] **Control 12.1:** _DFS users should set their account PIN. Where the first-time PIN is set by the DFS provider system or its agents, the PIN is unique for each user and must require use change at first login_
  * [ ] **Control 12.2:** _DFS users should set strong passwords and avoid easily guessable pins for their devices like date of birth._
  * [ ] **Control 12.3:** _Ensure sensitive DFS information is stored in secure portions of the mobile device._
  * [ ] **Control 12.4:** _App developers should ensure that before application installation on the device, user authentication is required_
  * [ ] **Control 12.5:** _App developers should ensure that access to DFS infrastructure, application, and services should only be authorised after identity authentication. Use multi-factor authentication, Something the user knows (such as a PIN), Something they have (such as a SIMcard), Something they are (such as a fingerprint or other biometric method)_
  * [ ] **Control 12.6:** _App developers should ensure that DFS applications securely manage access credentials_

**Risk:** Interception of DFS data in transit

* **Vulnerability:** Inherent SS7 security weakness\[iii] (SD: Communication Security)
  * [ ] **Control 12.7:** _Ensure all sensitive consumer data such as PINs and passwords are securely stored with strong encryption within the internal network and while at rest to mitigate internal threats against this data_
  * [ ] **Control 12.8:** _Use firewalls to detect and limit attacks based on SS7 security flaws_
* **Vulnerability:** Interception of MO-USSD transactions (SD: Communication Security)
  * [ ] **Control 12.9:** _Check if the IMEI of the device performing the transaction matches the registered IMEI of the account holder’s phone (a MITM system may clone the SIM with a different IMEI)_
* **Vulnerability:** Unprotected sensitive traffic and weak encryption practices (SD: Communication Security)
  * [ ] **Control 12.10:** _Monitor user velocity by comparing the location of the phone used to perform transactions to the last reported location of the phone (last in/out SMS or call)._
  * [ ] **Control 12.11:** _MNO's should enforce the use of the Personal Unlocking Key (PUK) on the SIM card for additional security in case the mobile device is lost or stolen._
  * [ ] **Control 12.13:** _Control and monitor the use of MSC MAP tracing and protocol analysers on USSD, SMS infrastructure to internal limit access to plain text SMS and USSD traffic in transit._
  * [ ] **Control 12.14:** _Use 2-way SecureOTP to the original phone number to verify the legitimacy of the transaction\[iv]_
  * [ ] **Control 12.15:** _Employ strong cryptography practices to assure confidentiality and integrity of data as it enters the DFS provider network and as it is processed and stored within this environment._
  * [ ] **Control 12.16:** _Limit number of DFS sessions per user. Allow a single session per user at a time irrespective of the access channel (STK, USSD, or https); a DFS user account should not be accessible using multiple channels simultaneously_
  * [ ] **Control 12.17:** _The mobile operator should deploy SS7 and diameter signalling security controls specified by the GSMA (FS.11, FS.07, IR.82, and IR.88) to limit threats due to SS7 attacks\[v]_

**Risk:** Exposure of sensitive customer data occurs because of the following vulnerabilities.

## Affected entity: DFS Provider

* **Vulnerability:** Inadequate protection of DFS customer registration data. (SD: Authentication )
  * [ ] **Control 12.18:** _Protect and guard customer data used for DFS registration, where physical forms are used, store, and transmit the data securely._
* \*\*Vulnerability:\*\*Use of weak encryption. (SD: Communication Security)
  * [ ] **Control 12.19:** _Use strong encryption standards like TLS encryption v1.2 and higher for API communication._
* **Vulnerability:** Inadequate DFS user access control and monitoring. (SD: Access Control)
  * [ ] **Control 12.20:** _Extend threat detection to explicitly incorporate threats associated with APIs._
  * [ ] **Control 12.21:** _Limit remote login access and minimize privileges to remote login sessions to backend DFS systems_
* **Vulnerability:** Inadequate DFS user access control monitoring. (SD: Access Control)
  * [ ] **Control 12.22:** _Limit the lifetime of TLS certificates to 825 days._
  * [ ] **Control 12.23:** _Authenticate user IP, device, and login time for all privileged users, agents, and merchants connecting to the DFS system. For example, configure a merchant and agent access to the DFS system to be accessible only during open trading hours._
  * [ ] **Control 12.24:** _Code and changes should be tested in the test environment before moving to the production platform; the test environment should be physically and logically separated from the production environment._
  * [ ] **Control 12.25:** _To improve security, use a trusted tamper-resistant device like a Hardware Security Module (HSM) to Securely manage the process and store cryptographic keys to protect user PINs, transactions, tokens, money vouchers._
  * [ ] **Control 12.26:** _Set user roles to define access rights based on the principle of least privilege._
  * [ ] **Control 12.27:** _After termination of a user, agent, merchant, payment service providers or third parties disable/deactivate respective accounts_
  * [ ] **Control 12.28:** _Set account dormancy period and disable dormant accounts at dormancy maturity._
  * [ ] **Control 12.29:** _Set schedules for logons and session limitations based on DFS roles. (session limitations can include the maximum number of reversals per day based on the role)_
  * [ ] **Control 12.30:** _Limit control, monitor, and periodically review privileged access to DFS systems, including user addition, modification, and deletion._
  * [ ] **Control 12.31:** _Monitor the use of APIs, and encrypt all data shared with third parties, put in place data management procedures and controls like signed non-disclosure agreements with payment service providers to avoid information/data leakage._
  *   [ ] **Control 12.32:** _Protect wireless transmissions per PCI DSS Requirements. Controls should include, but are not limited to, the following:_

      _a) Ensure vendor default encryption keys, passwords, and SNMP community strings are changed._

      _b) Facilitate the use of industry best practices to implement strong encryption for authentication and transmission._

      _c) Ensure that clear-text account data is not stored on a server connected to the Internet._

## Affected entity: Third-party

*   **Vulnerability:** Failure perform data destruction/erasing before disposing of devices (SD: Privacy)

    * [ ] **Control 12.32:** \_DFS Providers/Merchants should consistently dispose of old devices. When the solution provider provides guidance, the merchant should follow it. Some items to consider include:

    _a) Remove all tags and business identifiers._

    _b) Where possible, develop a contract with an authorized vendor who can help securely dispose of electronic materials and components._

    _c) Do not dispose of devices in trash containers or dumpsters associated with your business._
