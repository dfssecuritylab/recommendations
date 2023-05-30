# SIM attacks

Ability of an attacker to gain unauthorized access to a DFS user's SIM card.

## Affected entity: MNO

**Risk:** SIM takeover and unauthorized transactions

* **Vulnerability:** Inadequate controls for user identification and verification before SIM swap and SIM recycling (SD: Authentication)
  * [ ] **Control 10.1:** _MNOs should ensure that an identity verification process is in place before SIM swaps is performed._
  * [ ] **Control 10.2:** _User identity should be verified using MFA, a combination of something they are, something they have, or something they know. For example, with the presentation of a valid ID, biometric verification, and knowledge about the DFS account details before a SIM swap/ SIM replacement is performed._
* **Vulnerability:** Inadequate controls for user identification and verification before SIM swap and SIM recycling (SD: Authentication)
  * [ ] **Control 10.3:** _DFS and Payment Service Providers should be able to detect real-time whenever a SIM card with DFS services has swapped or replaced. And perform further verification before any high-value transaction or account changes are authorised with new SIM_
  * [ ] **Control 10.4:** _The mobile operator should safeguard and securely store SIM data like IMSI and SIM secret keys (KI values)_
  * [ ] **Control 10.5:** _A mobile number recycling process should be in place that involves communicating with DFS providers on Mobile Subscriber Identification Numbers (MSIDN) being churned or recycled. (in this context: number recycling is when the MNO reallocates a dormant/inactive Mobile Subscriber Identification Number (MSISDN) to a new customer). When a SIM is recycled, the mobile operator will report a new IMSI of the related account phone number. The DFS provider should block the account until the identity of the new person holding the SIM card is verified as the account holder._

**Risk:** Unauthorized access to user's mobile DFS data o

* **Vulnerability:** Mobile device theft (SD: data confidentiality)
  * [ ] **Control 10.6:** DFS users should remotely delete their data and disable the SIM card in the mobile device in case the device is lost or stolen.

**Risk:** Loss of access to accounts or reputational damage.

* **Vulnerability:** Inadequacies in SIM swap and recycling process\[ii] (SD: data integrity)
  *   [ ] **Control 10.7:** DFS providers should ensure they have procedures in place to detect and avert suspicious SIM swaps and SIM recycle by: a) Check if the IMSI associated with the phone number has changed, this is an indication of SIM swap.

      b) Check if the IMSI associated with the phone number has changed, this is an indication of SIM swap.

      If there is an indication of a SIM swap, check the IMEI of the phone holding the SIM. If the IMEI has also changed, there is a high probability of a SIM swap. In that case, the DFS provider should block the account until performing account verification procedures, for example, via a voice call or an agent."
