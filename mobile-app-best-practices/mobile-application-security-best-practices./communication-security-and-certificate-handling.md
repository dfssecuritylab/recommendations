# Communication Security and Certificate Handling

1. Apps should be making use of standardised cryptographic libraries and for communication with back-end services, should use end-to-end encryption with standardized protocols, specifically TLS. The minimum recommended version of TLS that should be used is version 1.2.
2. TLS certificates should not be expired and should present strong cipher suites, specifically AES-128 encryption and SHA-256 for hashing. Authenticated encryption modes of operation such as GCM are encouraged.
3. Limit the lifetime of issued certificates to 825 days in accordance with the CA/Browser Forum best practices.
4. Assure the trustworthiness of the certificate authority and consider a contingency plan for if the CA is no longer trusted.
5. Ensure the configuration of TLS is performed in a secure fashion and avoid misconfiguration issues that could result in failure to authenticate or poor algorithm selection.
6. Certificate pinning is recommended to prevent replacement of certificates.
7. Client devices must ensure that they correctly validate server certificates.
