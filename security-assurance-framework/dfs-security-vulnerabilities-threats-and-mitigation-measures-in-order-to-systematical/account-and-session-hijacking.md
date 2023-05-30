# Account and Session Hijacking

The general threat is the ability of an attacker to take control of an account or communication session. The vulnerabilities are manifested in different ways at the DFS provider and the MNO.

### Affected Entity: DFS Provider

#### **Risk:** Data exposure and modification

* **Vulnerability:** Inadequate controls on dormant accounts
  * [ ] **Control 1.1:** _Set timeouts and auto logouts user sessions on DFS applications (logical sessions). Within the application, ensure support for password complexity (enforced by the server), set maximum unsuccessful login attempts, password history and reuse periods, account lock-out periods to a reasonably minimal value to minimize the potential for offline attack_

#### **Risk:** Unauthorized account takeover

* **Vulnerability:** Inadequate controls on dormant accounts
  * [ ] **Control 1.2:** _Require user identity validation for dormant DFS accounts users before re-activating accounts_

#### **Risk:** User impersonation

* **Vulnerability** Failure to perform geographical location validation (SD: Communication security)
  * [ ] **Control 1.3:** _Limit access to DFS services based on user locations (for example disable access to DFS USSD codes while roaming, STK and SMS for merchants and agents) where possible restrict access by region for DFS agents, where possible check that agent and number performing a deposit or withdrawals are within the same serving area_
* **Vulnerability:** Inadequate user verification of preferred user communication channels for DFS services (SD: Communication security)
  * [ ] **Control 1.4:** _Restrict DFS services by communication channels (during registration customers should optionally choose service access channel, USSD only, STK only, app only, or a combination) attempted DFS access through channels other than opted should be blocked and red-flagged_

#### **Risk:** Unauthorised access to user data and credentials

* **Vulnerability:** Replay session based on tokens intercepted (SD: communication security)
  * [ ] **Control 1.5:** _The DFS system should not trust any client-side authentication or authorization tokens; validation of access tokens must be performed at the server-side_
* **Vulnerability:** Weak encryption algorithms for password storage (SD: data confidentiality)
  * [ ] **Control 1.6:** _Store DFS passwords using strong salted cryptographic hashing algorithms._

### Affected Entity: MNO

#### **Risk:** Impersonation of authorised users occurs because of the following vulnerability

* **Vulnerability:** Session timeouts not specified for DFS services
  * [ ] **Control 1.7:** _Add session timeouts for USSD, SMS, application, and web access to DFS services._

#### **Risk:** Unauthorized access to user data and credentials

* **Vulnerability:** User credentials for DFS application are sent in inherently insecure ways like SMS or through agents (SD: data confidentiality)
  * [ ] **Control 1.8:** _Where possible, DFS users should set their own passwords at registration and they should be encrypted throughout the transmission to the DFS system. Where first-time credentials are sent to the users, ensure DFS application credentials are sent to users directly without third parties/agents. Users should then be required to set new passwords after the first-time login._
