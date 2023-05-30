# Denial of Service Attacks

We characterize these attacks as being designed to prevent services within the DFS ecosystem from being offered.

### Affected entity: MNO

#### **Risk:** Inability to perform a transaction as a result of service outage and transaction failure, high transaction delays.

* **Vulnerability:** Network failure due to insufficient network capacity or to maintenance or design (SD: availability)
  * [ ] **Control 6.1:** _The mobile network operator should take steps to ensure network high network availability to allow access to DFS services through USSD, SMS, and the Internet._
* **Vulnerability:** Network failure due to insufficient network capacity or to maintenance or design (SD: availability)
  * [ ] **Control 6.2:** _The MNO should perform technical capacity tests simulating different transactions based on customer numbers, expected growth, expected number of transactions, and expected peak periods to ensure continued system performance._

### Affected entity: DFS Provider

* **Vulnerability:** Inadequate monitoring of network traffic and packets (SD: availability, communication security)
  * [ ] **Control 6.3:** _The DFS provider should protect against network attacks by the use of firewalls and traffic filters, and protect against DFS infrastructure threats by challenging suspicious traffic through network admission techniques and mechanisms such as CAPTCHAs._
* **Vulnerability:** Enabling unnecessary services (SD: data confidentiality)
  * [ ] **Control 6.4:** _Inbound internet traffic should be limited and continuously monitored._
* **Vulnerability:** Enabling unnecessary services (SD: data confidentiality)
  * [ ] **Control 6.5:** _Set restrictive firewall rules by default, use ports whitelisting, use packet filters, and continuously monitor access to whitelisted/permitted ports and IP's._
