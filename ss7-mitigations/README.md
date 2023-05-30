---
description: >-
  The SS7 Vulnerabilities and Mitigation Measures for DFS Transactions​ contain
  details on the recommendations for DFS regulators and mobile network operators
  to mitigate SS7 vulnerabilities.
---

# Security controls for regulators to mitigate SS7 vulnerabilities

The USSD and SMS communication channels with which the end-user communicates with the DFS provider rely on the legacy Signaling System 7 protocol which has for long been "broken" and with many published vulnerabilities, some over 20 years old, which enables attackers to commit fraud, compromise DFS and steal funds through account takeovers, DFS interception, denial of service attacks etc.

### DFS provider controls to address DFS vulnerabilities due to SS7

DFS operators should consider adopting the following controls to mitigate SS7 risks**.**

1. **Session time out:** use session timeout for USSD and STK to reduce success man in the middle attacks, OTP messages for DFS should also have a session time out.
2. **Transaction limits for insecure channels:** Set transaction limits for customer withdrawals and transfers through insecure channels like USSD.
3. **User education:** DFS users should be educated on how to engage securely with digital financial services including impacts of using rooted devices, connecting to public Wi-Fi, installing unverified applications etc.
4. **Bidirectional OTP SMS flow** : The DFS provider should make the authentication flow bidirectional, that is receive the OTP from the user, not send it.
5. **Detecting and mitigating social engineering attacks with MT-USSD and interception of USSD** by verifying using secureOTP, location validation, IMSI and IMEI validation
