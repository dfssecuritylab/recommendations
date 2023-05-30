# Attacks against credentials

We broadly characterize these threats as those designed to steal or tamper with the credentials for users of DFS systems and mobile devices

## Affected entities: Mobile User

**Risk:** Unauthorized access and takeover

* **Vulnerability:** Use of weak passwords/PINs at the application level, making these credentials susceptible to brute-force attacks (SD: authentication)
  * [ ] **Control 2.1**: _Require the use of longer and not easily guessed PINs/passwords in mobile money applications. Caution should be exercised before mandating the use of complex PINs; ensure that any such adoption goes hand-in-hand with user education, as overly complex PINs are likely to be written down or entered by others, thus degrading their security._
* **Vulnerability:** Use of simple PINs for accessing the mobile device (SD: authentication)
  * [ ] **Control 2.2:** _Use robust authentication mechanisms to demonstrate ownership of the device. Because the keyspace of PINs makes them susceptible to a brute-force attack, consider the use of longer PINs or alphanumeric PINs, such as easily remembered passphrases._

**Risk:** Credential-stealing through Man in the Middle attacks

* **vulnerability:** Server misconfiguration (SD: authentication)
  * [ ] **Control 2.3:** _DFS applications should be designed to verify the server name they are connecting to._

**Risk:** DFS system compromise

* **Vulnerability** Failure to perform login monitoring, leaving systems susceptible to brute force attacks (SD: access control)
  * [ ] **Control 2.4:** _Enforce a maximum number of login attempts to DFS accounts for back-end users, merchants, agents and DFS customers on DFS systems (database, OS, application)_
