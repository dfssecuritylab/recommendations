# Insider Attacks

Attacks as performed by adversaries within the organization’s perimeter, often who have elevated access and privileges to resources.

### Affected entity: DFS Provider

#### **Risk:** Data exposure and modification

* **Vulnerability:** Insufficient internal controls on critical operations (SD: access control)
  * [ ] **Control 7.1:** _Where possible, limit critical changes using the four-eye principle (maker-checker/two-person rule) for critical actions including (but not limited to) an administrator creating, modifying or deleting another administrator account, changing, attaching and detaching of DFS account from mobile number/user ID, and transaction reversal._

#### **Risk:** Lack of validation of data inputs (SD: data integrity)

* **Control 7.2:** _DFS providers should ensure sufficient separation of duties for maker-approver; for example, an administrator may not have access rights to both create and activate a DFS account_
* **Vulnerability:** Inadequate privilege management & control (SD: access control)
  * [ ] **Control 7.3:** _Limit, control, and monitor physical access to sensitive physical DFS infrastructure. Physically isolate and put in place logical and physical deterrents/barriers to DFS infrastructure from other infrastructure. Employ least privilege techniques such that preventative access is only allowed for authorized persons, supplanted by detection and enforcement (e.g., alarms if forced). Monitor system activity by logging all access (e.g., who accessed, what they accessed, where they accessed from, and when they accessed it)._

#### **Risk:** Data inaccuracy and inconsistency

* **Vulnerability:** Use of test data & configurations in a production environment (SD: data integrity)
  * [ ] **Control 7.4:** _The DFS provider should employ robust input validation routines on external-facing services by checking out-of-range values and unpermitted characters in fields, and by constraining and sanitizing input. Input validation should happen at the earliest possible point and should be done both on the client and server-side, however, the server should not rely solely on client-side validation. Additionally, block, log and review all requests that violate the Web Services Description Language (WSDL) and schemas_
  * [ ] **Control 7.5:** _Use database fingerprinting to detect tampering and modification of data after it has been stored. Techniques such as digital signatures across database columns can be used to detect user data modification_
  * [ ] **Control 7.6:** _Ensure all test data is removed from code before it is migrated to the production environment._
* **Vulnerability:** Insufficient logging, inability to protect logs from alteration. (SD: non-repudiation)
  * [ ] **Control 7.7:** _DFS systems should use logging mechanisms, including capturing the provenance of user actions or logging of critical actions into tamper-proof storage, secure DFS system logs from tampering, editing, deleting, stopping. Use digital signatures attached to actions, particularly those that arrive over a network connection._
* **Vulnerability:** Inaccurate and unsynchronised clocks (SD: data integrity)
  * [ ] **Control 7.8:** _Ensure clock accuracy synchronization on all systems connected to the DFS system. NTP and SNTP are some of the protocols used to sync accurate time; however, these have to be deployed securely._
