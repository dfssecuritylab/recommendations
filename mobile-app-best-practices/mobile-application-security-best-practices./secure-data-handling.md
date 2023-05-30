# Secure Data Handling

1. Mobile devices should securely store confidential information, for example by using the Android KeyStore framework.
2. Trusted hardware should be used for the storage of sensitive information if it is available on client smartphones.
3. Avoid storing information in external storage and if it is done, ensure that strong input validation is performed prior to using this data.
4. Delete confidential data from caches and memory after it is used and avoid general exposure of information (e.g., placing the secret key on the stack). Assure the clean-up of memory prior to the application exiting.
5. Restrict data shared with other applications through fine-grained permissions. Minimized the number of permissions requested by the app and ensure that the permissions correlate to functionality required for the app to work.
6. Do not hard-code sensitive information such as passwords or keys into the application source code.
7. Validate any input coming from the client that is to be stored in databases to avoid SQL injection attacks.
