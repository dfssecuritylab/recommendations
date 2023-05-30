# DFS provider controls to address DFS vulnerabilities due to SS7

DFS operators should consider adopting the following controls to mitigate SS7 risks**.**

1. **Session time out:** use session timeout for USSD and STK to reduce success man in the middle attacks, OTP messages for DFS should also have a session time out.
2. **Transaction limits for insecure channels:** Set transaction limits for customer withdrawals and transfers through insecure channels like USSD.
3. **User education:** DFS users should be educated on how to engage securely with digital financial services including impacts of using rooted devices, connecting to public Wi-Fi, installing unverified applications etc.
4.  **Bidirectional OTP SMS flow**: The DFS provider should make the authentication flow bidirectional, that is receive the OTP from the user, not send it.

    <figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>Detection and mitigation of SMS interception with bidirectional OTP SMS flow</p></figcaption></figure>
5. **Detecting and mitigating social engineering attacks with MT-USSD and interception of USSD** by verifying using secureOTP, location validation, IMSI and IMEI validation
