# Attacks against systems and platforms

We characterize these attacks as those that a remote adversary can carry out to spy on or modify information without insider credentials or other privileged access.

### Affected entity: Mobile user

#### **Risk:** Spying and credentials stealing from user devices

* **Vulnerability:** Unverified malicious binary SMS SIM updates (SD: authentication)
  * [ ] **Control 3.1:** _Provide the mobile user with the ability to trust or distrust individual binary-based SMS messages. Doing so could prevent malicious updates to the SIM card_
* **Vulnerability:** Insecure transfer of customer credentials (SD: access control)
  * [ ] **Control 3.2:** _DFS providers should transmit the user authentication credentials securely over a different channel (out of band)._

#### **Risk:** Account access, compromise and denial of service

* **Vulnerability:** Exposure of internal network to external adversaries (SD: access control)
  * [ ] **Control 3.3:** _Use Network Address Translation to limit external exposure of DFS IP address and routing information._

### Affected entity: DFS Provider

#### **Risk:** Account access, compromise, and denial of service

* **Vulnerability:** Insufficient protection of internal systems against external adversaries (SD: access control
  * [ ] **Control 3.4:** _Avoid direct access by external systems to the DFS backend systems by setting up a DMZ that logically separates the DFS system from all other internal and external systems._
