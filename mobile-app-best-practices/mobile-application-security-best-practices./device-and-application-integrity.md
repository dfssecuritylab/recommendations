# Device and Application Integrity

1. The safest devices for performing financial transactions on are ones that have not been "jailbroken" or "rooted", as it can be difficult or impossible to assess the security of the underlying operating system when it has been replaced or exploited. Applications should thus use the mobile platform services to determine that they and the underlying platform have not been modified.
2. Remove any extraneous code that might have been added to the application during development, such as features that are not designed for the device platforms that the app is to be deployed upon or developer/debug features to reduce the attack surface of the deployed production code.
3. On the server-side, determine whether the app is running in a high integrity state through signature validation or hashing over the app or certain program function blocks.
