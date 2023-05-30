# Compromise of DFS Infrastructure

Attacks as targeting the underlying infrastructure of the DFS ecosystem.

### Affected entity: MNO & DFS Provider

#### **Risk:** Infrastructure and data compromise

* **Vulnerability:** \_Insecure and inadequate access controls on user accounts (SD: access control)
  * [ ] **Control 9.1:** _Use multi-factor or multi-model authentication for access to DFS accounts._

**Risk:** Service outage and inability to transact.

* **Vulnerability:** Untested Service restoration (SD: availability)
  * [ ] **Control 9.1:** _Deactivate and remove default accounts and credentials from databases, applications, operating systems, and other access interfaces that interact with the production DFS system._
  * [ ] **Control 9.2:** _Review installation, vendor, support accounts, and access points to DFS systems and infrastructure. All of these accounts should be deactivated or allocated to appropriate user profiles_

#### **Risk:** Data exfiltration and modification, compromise of transaction integrity, and interruption of service

* **Vulnerability:** Inadequate data controls like inadequate implementation of ACID tests (Atomicity, Consistency, Isolation, Durability) on transactions, allowing them to exist in a partially completed state (SD: data integrity)
  * [ ] **Control 9.3:** _Perform end-to-end tests after any changes to the DFS, MNO, SP, and third party systems, include regression and capacity tests in the acceptance tests. Also, ensure there is a fall-back/blackout plan_
  * [ ] **Control 9.4:** _Schedule regular backups for DFS systems. Regularly test and securely store backups offline and offsite in an encrypted form_
  * [ ] **Control 9.5:** _Use standard ACID functionality of the databases to ensure transaction integrity. DFS operations should either succeed completely or fail completely._

### Affected entity: Third-Party Provider

#### **Risk:** Inability for the user to transact.

* **Vulnerability:** Inadequate mechanisms to assure data integrity and over-reliance on external trust anchors (SD: non-repudiation)
  * [ ] **Control 9.6:** _DFS applications/3rd parties should support the use of digital signatures, a secure digital signature provides irrefutable evidence of the transaction's origin. Digital signatures are only valid as long as the PKI has not been compromised and must be tested with plans for assuring agility. By demonstrating that signing keys are adequately protected up to the root key, the DFS provider can withstand legal challenges about the authenticity of a specific user and desputed transactions._
