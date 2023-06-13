# MNO controls to address DFS vulnerabilities due to SS7

1. **Secure GSM ciphers for radio network traffic**: The mobile operator should ensure the use of secure radio encryption between users' devices and base stations.
2. **Session time out:** use session timeout for USSD and STK to reduce success man in the middle attacks.
3. **USSD PIN masking:** Deploy USSD PIN masking whenever possible.
4. **Secure and monitor core network traffic**: Use a TLS v1.2 or higher to secure the connection between the SMSC GW, USSD GW, and the DFS application server.
5. **Limit access to traces and logs**: Ensure there is an auditable process in place to review access to traces and logs on interfaces that use inherently insecure protocols. USSD PINs should not be logged in the event data records.
6. **SMS filtering**: Remote attackers rely on mobile networks to deliver binary SMS to and from victim phones. Mobile operators should implement blocking the ability to send and receive binary messages like OTA SMS. Such SMS should only be allowed from whitelisted sources.
7. **SMS home routing:** This is the barring of all outgoing and incoming SMS except those routed through the home network hosts. OTA messages with STK coding from home subscribers should be restricted to only be sent to/by the MNO platform—and not to other subscribers.
