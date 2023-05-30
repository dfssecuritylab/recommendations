---
description: Threats resulting in user data being inadvertently exposed.
---

# Unintended Disclosure of Personal Information

## Affected entity: DFS Provider

**Risk:** The risk of exposure of personally identifiable information occurs because of the following vulnerability

* **Vulnerability:** Inadequate oversight and controls in test environments (SD: privacy)
  * [ ] **Control 17.1:** DFS providers should ensure that customer data in production environments is not used in test environments unless anonymized according to best practices. Conversely, test data should not be migrated to the product.

## Affected entity: Third-Party Provider

**Risk:** Exposure of sensitive information occurs because of the following vulnerabilities: |

* **Vulnerability:** Exposure of customer-sensitive information in transactions or through APIs (SD: privacy)
  * [ ] **Control 17.2:** Third-party providers should restrict the sharing of information with other parties such as payment service providers and DFS providers to the minimum required to assure the integrity of the transaction.
* **Vulnerability:** Insufficient data protection controls (SD: privacy)
* **Control 17.3:** Providers should ensure that customer-sensitive data is removed from environments such as trace logs (for example, cash retrieval voucher codes, bank account numbers, and credentials). Use place holders whenever possible to represent this data in log files.
