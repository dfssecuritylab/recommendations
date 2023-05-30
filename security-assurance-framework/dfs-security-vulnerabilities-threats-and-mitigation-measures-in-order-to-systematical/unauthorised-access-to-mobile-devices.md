# Unauthorised Access to Mobile Devices

Threats is characterized as specific attacks against mobile devices from adversaries.

## Affected entity: Mobile User

**Risk:** impersonation and data loss/fraudulent transactions

* **Vulnerability:** Inadequate user authentication on the device (SD: Data Confidentiality)
  * [ ] **Control 16.1:** Mobile devices should automatically lock after a period of inactivity, forcing device authentication to be performed to unlock the device before it is used for DFS transactions.
  * [ ] \*\*Control 16.2:\*\*Use Strong PINs, remote data wipe, PIN lock, use biometric authentication (e.g., fingerprint, iris) when such device features are available.
  * [ ] **Control 16.3:** Device manufacturers must ensure that critical updates are available for consumers to directly acquire or are made available to the network provides to be pushed to users.

## Affected entity: DFS Provider

**Risk:** DFS user account takeover

* **Vulnerability:** Overly permissive access to the DFS infrastructure (SD: Authentication)
  * [ ] \*\*Control 16.4:\*\*Before authenticating DFS users, when possible, validate the IMSI, device, and location, and IP address of the user to establish their identity and to prevent unauthorized access to the network infrastructure.

**Risk:** Failed transaction executon

## Affected entity: DFS Provider, Third-Party Provider

* **Vulnerability:** Inadequate transaction verification (SD: Non-Repudiation)
  * [ ] \*\*Control 16.5:\*\*Payment service providers should ensure that companion general-purpose reloadable cards linked to DFS accounts require the use of EMV chips with cardholder verification methods, such as PINs or biometrics, when practical, and that all transactions result in an alert to customers.
