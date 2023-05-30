# Compromise of DFS Services

The ability of an attacker to breach a financial service without being detected.

### Affected entity: DFS provider

#### **Risk:** Service failure and compromise of DFS services

* **Vulnerability:** Unauthorized changes to system configuration and log files and data (SD: Data Integrity)
  *   [ ] **Control 11.1:** _Protect against tampering and limit offline DFS transactions_

      _a) Protect and monitor DFS application files from tampering and changes using file integrity monitors, e.g., by calculating checksums or validating digital signatures._

      _b) By policy, the DFS provider or merchant should limit use of mobile payment solution to authorize transactions offline or store transactions for later transmission._
* **Vulnerability:** Insufficient user access validation or user input validation (SD: Authentication)
  * [ ] **Control 11.1:** _Use strong multi-factor authentication for user and 3rd party provider access to DFS systems, e.g., token or biometrics, the use of multi-factor authentication to verify system users increases non-repudiation of origin_
* **Vulnerability:** Inadequate user access validation or user input validation (SD: Authentication)
  * [ ] **Control 11.2:** _Check incoming data against expected values in API related data schema, for USSD, perform XML validation of XML over HTTP requests_
  * [ ] **Control 11.3:** _Use analytics systems to check user velocity between transactions, transaction time of day access tracking for additional authorization validation checks._
  * [ ] **Control 11.4:** _Regardless of the method used for producing receipts (e.g., e-mail, SMS, or attached printer), the method should mask the Primary Account Number (PAN) in support of applicable laws, regulations, and payment-card policies. By policy and practice, the DFS Provider/merchant should not permit the use of non-secure channels such as e-mail and SMS to send PAN or Sensitive authentication data (SAD)_
