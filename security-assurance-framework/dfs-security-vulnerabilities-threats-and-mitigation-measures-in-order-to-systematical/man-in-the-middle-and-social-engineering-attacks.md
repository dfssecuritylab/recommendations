# Man-in-the-middle and social engineering attacks

We group these two types of attacks because they both involve an adversary actively interposing themselves into communication or interaction (e.g., between a user and device or MNO, or a communication interposition between parties)

### Affected entity: Mobile User

#### **Risk:** Data exposure and modification

* **Vulnerability:** Use of unverified and unsigned applications (SD: privacy, data integrity)
  * [ ] **Control 8.1:** _Critical focus should be on guiding the customer to access and download DFS applications through official application release channels to mitigate the risk of running malware-infected apps._
* **Vulnerability:** Spamming such as unsolicited SMS messages, in-app advertisements, or e-mails (SD: data integrity)
  * [ ] **Control 8.2:** _MNOs and DFS providers should undertake active customer awareness campaigns to educate consumers and internal staff about malicious messages, phishing attacks, and spoofing._
* **Vulnerability:** Insufficiently protected credentials (SD: access control)
  * [ ] **Control 8.3:** _Mask user passwords and PINs, actively educate customers on shoulder surfing and safe PIN/password usage to avoid shoulder surfing and writing down of passwords._

### Affected entity: MNO

#### **Risk:** Unauthorized access to user data

* **Vulnerability:** Weak over-the-air encryption (SD: communication security)
  * [ ] **Control 8.4:** _Discontinue the use of A5/0, A5/1 GSM encryption ciphers. Closely monitor results from the security and cryptographic community regarding the feasibility and ease of compromising A5/3 and A5/4 and begin considering stronger ciphers. Have a deployment strategy ready for these newer ciphers._

**Risk:** User impersonation

* **Vulnerability:** Failure to force Calling Line Identification & filtering (SD: communication security)
  * [ ] **Control 8.5:** _MNOs should do CLI analysis for calls/SMS to detect calls and SMS that may be spoofed to appear like DFS provider calls._

**Risk:** User account takeover

* **Vulnerability:** Inadequate account configuration and authorisation controls (SD: authentication)
  * [ ] **Control 8.6:** _Require user authentication and authorization for high-risk account changes and transaction, and deny performing of transactions even when the device is logged in until knowledge of PIN or password has been demonstrated_

### Affected entity: Third-Party Providers

#### **Risk:** Third party exposure of sensitive information

* **Vulnerability:** Weak encryption algorithms used on data stored in the device and data transmitted (SD: privacy)
  * [ ] **Control 8.7:** _Sufficiently secure encryption should be employed for both data protection within the mobile application and communication with backend DFS systems and whenever possible, mask, truncate or redact customer confidential information._
* **Vulnerability:** Lack of encryption of communications (SD: communication security
  * [ ] **Control 8.8:** Use digital signatures to identify third parties connected to the DFS system when transactions are being performed.
* **Vulnerability:** Handling & management of certificate or key materials (SD: access control)
  * [ ] **Control 8.9:** _Only trusted keys and certificates should be accepted to allow data exchange between DFS providers and third parties, and they should be protected from disclosure._

#### **Risk:** Identity theft

* **Vulnerability:** DFS Provider or MNO system failure leading to agents/third parties reverting to offline processes (SD: availability)
  * [ ] **Control 8.9:** Set procedural and technical controls for effective management during system downtime with related service providers. For example, set controls to manage offline transactions (e.g., SIM swaps) when access to the DFS system is intermittent. Have additional checks for remittances and third-party payments when DFS system or 3rd party system access is intermittent.
