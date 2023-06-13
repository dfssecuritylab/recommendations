# Security recommendations to protect against DFS SIM risks and SIM swap fraud

## SIM vulnerabilities

Financial institutions have adopted digital means and are continuing to avail financial products on mobile based application like Unstructured Supplementary Services (USSD) and STK banking, which makes financial services available anywhere, anytime through strings of interactions via Unstructured Supplementary Service Data (USSD), Short Messaging Service (SMS), internet. The interactions between the mobile user and the network are authenticated with the SIM card. However, there has been increased fraud risks on SIMs due to threats arising from notably SIM swaps, SIM jacker attacks and SIM recycling and number porting.

### SIM swap fraud

SIM swap fraud has become a common tactic used to takeover accounts. In a SIM swap fraud, a telecom provider is tricked into issuing a replacement of a victim's SIM to a fraudster allowing them to take over a DFS accounts that relies on the SMS one time password (OTP) or USSD for authentication.

### SIM recycling risks

SIM recycling risks is related to reliance on the phone numbers, Mobile Station Integrated Services Digital Network (MSISDN) as the primary DFS account numbers. Telco providers reassign phone numbers that are dormant or deemed to have churned (not used within specific period). The reassignment of the phone number may effectively lead to an account takeover of the DFS wallet associated with the number if the DFS provider is not aware of the change of ownership.

### Binary Over the Air attack (SIM jacker)

The SIM jacker attack exploits a vulnerability in a SIM Card library called the S@T browser. A specially formatted binary text message is sent to the victim handset, which contains a set of commands to be executed by the S@T Browser environment in the SIM card. The commands can instruct the handset to exfiltrate this information, force the mobile device to initiate a USSD request, make a phone call, or send a message.
