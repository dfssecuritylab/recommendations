# Elements of DFS ecosystem

&#x20;In the scope of this report are five categories of mobile payments:

* Mobile money transfer using the MNO’s channels (e.g. SMS, USSD, voice telephony) without a specific payment application downloaded onto the customer’s mobile device which would be a featurephone (e.g. MPESA).
* Mobile payment application on mobile device of user linked to a bank account, debit card or credit card (e.g. Square, Venmo, Facebook messenger)
* Contactless payment technologies: Contactless payment technologies involve use of digital wallets, which can use different types of communications technologies for sending payment data from the user mobile device to the merchant POS. Some of the communications technologies used to transmit the information to the POS include Near Field Communication (NFC), QR code, magnetic secure transmission (MST), Bluetooth, SMS and Internet. The digital wallet could be stored either on the user mobile device or in the cloud.
* Near Sound Data Transfer (NSDT) Payments: NSDT uses the audio channel of the mobile phone to encrypt the data for payment transactions.
* Remote payments: This includes Internet payments (via credit card on an e-commerce website/Card-on-file transactions), direct carrier billing, SMS premium payments and mobile banking.              &#x20;

Digital currency wallets (e.g. Bitcoin) are outside the scope of this report.

In the next sections, the elements of the DFS ecosystem are considered for:

1. Mobile payments using USSD, SMS, IVR and STK
2. Mobile payment applications and digital wallets (e.g. Google Pay, Apple Pay, WeChat Pay).

### Elements of a DFS ecosystem using USSD, SMS, IVR, STK and NSDT <a href="#_toc25774565" id="_toc25774565"></a>

In figure 6 below, the major constituents within the ecosystem are shown. Not every element will be used in every deployment; for example, in cases where there is no Wi-Fi access or smartphone app available for a DFS service, communications from the user would be constrained to interactions through the mobile network, rather than through external Internet gateways or through reliance on a cloud service.

&#x20;

<figure><img src=".gitbook/assets/DFS ecosystem.png" alt=""><figcaption><p>Figure 6 - Major Elements of the DFS Ecosystem</p></figcaption></figure>

&#x20;The stakeholders throughout the ecosystem are comprised of the following:

a)   **User/Customer:** The customer is the target audience for a DFS service, who makes use of a mobile money application to interact with the service. Such interaction can happen either directly, through the mobile network or through the Internet (depending on features of the underlying mobile platform and the mobile money application); alternatively, a DFS agent who interacts with the DFS service on behalf of the customer can mediate such interaction. The agent can either interface directly with the network or use a web gateway to provide such services.

b)     **Mobile device:** The mobile device provides a platform for deploying a mobile money application. It is the main channel through which the customer (or agent interacting on the customer’s behalf; for ease of exposition it is assumed that all further interactions with the service as being through the customer unless there are actions specifically required of the agent) interfaces with the DFS service. Mobile devices can be either feature phones or smartphones. Feature phones often containing limited resources and supporting limited interfaces for applications as well as limited connectivity options (e.g., 2G GSM services). Smartphones on the other hand, can support very powerful services with secure hardware elements and support for advanced networking and Wi-Fi connectivity.  Both feature phones and smartphones contain SIM cards, some of which contain secure elements that can be leveraged by applications. The mobile device has an operating system, whose capabilities will be dependent on the resources available to it. Lightweight operating systems modelled after the Symbian OS are often found on feature phones, while smartphones commonly have the Android versions, IOS, Windows and other operating system installed.

c)      Base Station: The communication link between the base station and the mobile handset is the primary channel for sending information between the user and the DFS provider. Notably, in systems where apps are not delivered to handsets but open networks are instead used (e.g., SMS, STK, IVR and USSD-based communication), this link is the only part of the overall architecture where encryption is in place on data transmitted to and from the consumer – once data is received at the base station, it is sent unencrypted through the provider networks. It is vital to the sustainability and feasibility of a DFS system that this link be robust, reliable, and virtually ubiquitous.

d)      Mobile Network: The carrier network provides transit connectivity for information originating at the customer handset. It is comprised of different nodes that enable communication including the different gateways to external providers and to DFS providers, which may be associated with the particular carrier or may be external entities requiring Internet communication. Within this network resides gateways such as for USSD, IVR, STK and SMS, internal databases such as HLRs and VLRs, and Internet gateways that can act as connection points to the DFS provider. In cases where the mobile network operator also provides the DFS services, gateways to those services will be maintained within their internal network. The Mobile Switching Center (MSC) is at the core of the different nodes within the mobile network, to facilitate routing of communications using user data from the HLR or VLR. [ in Annex 1](file:///C:/Users/kibuuka/AppData/Local/Microsoft/Windows/INetCache/Content.Outlook/3K7XJPWX/Annex%201.docx) shows detailed network nodes in the Mobile network, the SMSC gateway (GW), SAT(SIM Application Toolkit) GW, USSD gateway, IVR and internet GW enable use of the respective access modes for the user, we also show the MNO billing system for its purpose when used in some deployments by the MNO for  charges on SMS, IVR or internet. A Mobile Virtual Network Operator (MVNO) may provide the services of the MNO to the DFS provider and the customer but the wireless network infrastructure is still provided by a network operator or enabler.

e)      DFS Provider: The DFS provider interfaces the application contents originating in mobile operator networks with the back-end financial providers and for administering the customer’s information in a secure fashion, and allowing for services, such as audits. In order for these operations to be secure, the DFS operator must be confident that the person accessing the data is who they claim to be. Audit logs must also be enabled to allow assessment of the contents of data within the network and of commands issued through the DFS application. Determining customer identity, credentialing, storing customer transaction data, providing enabling interfaces like API’s for third parties, processing transactions from the different sources,  is also a role performed by the DFS operator.

f)       Third-Party Providers: External providers allow for the interfacing between carrier-based mobile money systems and provide the basis for connecting with back-end financial networks such as the banking infrastructure. Other roles that can be assumed by these external providers include operating the IT system or performing customer support, and, in some cases, they may interface directly between DFS systems or act as service and transaction aggregators.

g)      Digital Financial Services Application: The application provides the interface by which the customer interacts with the DFS ecosystem. Applications can vary widely in the interfaces and richness of experience they provide to the customer, from menu-based systems on feature phones, designed to communicate via USSD, STK or SMS to voice designs that make use of IVR, or rich graphical interfaces on smartphones with end-to-end transport security provided by Internet-standard cryptographic algorithms. Interactions may occur using special application menus enabled by code, password, fingerprint, etc., enabling users to send money, make bill payments, top-up airtime, and check account balances.

### Elements of a DFS ecosystem based on applications and digital wallets (e.g Google Pay, Apple pay, WeChat Pay, Samsung Pay). <a href="#_toc25774566" id="_toc25774566"></a>

There are different elements in ecosystems based on digital wallet models, among the key models are; device-centric mobile proximity wallet, device-centric mobile in-app wallet, Card-not-present card-on-file wallet, QR code and digital checkout wallets. All these have different technology platforms and employ different security models.

&#x20;

<figure><img src=".gitbook/assets/DFS ecosystem based on applications and digital wallets.png" alt=""><figcaption><p>DFS ecosystem based on applications and digital wallets</p></figcaption></figure>

We describe each of the components of this ecosystem below:

a)   **Mobile Device**

The mobile device provides a platform for the mobile wallets to be accessed, it hosts the digital wallet/application, the device OS and the secure element which is key for securing the DFS and application data.

<figure><img src=".gitbook/assets/Mobile Device Components.png" alt=""><figcaption><p>Figure 8 - Mobile device components</p></figcaption></figure>

The figure below illustrates some of the components of the user’s mobile device.

i.             The NFC controller and the NFC antenna: The NFC controller handles Near Field Communication protocols and routes communication between the application and the Secure Element, and between the Secure Element and the point-of-sale terminal. The NFC antenna relays the signals between the controller and the POS terminal.

&#x20; ii.            The Secure Element: The Secure Element (SE) is a tamper-resistant platform, typically a one-chip secure microcontroller designed for securely hosting applications and their confidential and cryptographic data. The use of the SE depends on the type of mobile wallet application and the type of mobile payment modes, for example, the SE in Apple devices emulates the card when used for Apple Pay. SEs exist in different forms to address the requirements of the various payment applications or digital wallets and their market needs. The SE can be an embedded and integrated in the mobile device hardware such as the SE in the iPhone. The SE can also be a SIM/UICC, networks using the GSM standard prefer this more commonly in the form of SIM Toolkit (STK) applications that leverage on the SIM as the secure element to offer a secure mobile money application. The SE can also be a secure memory card that is pluggable into the mobile device.

&#x20;iii.             Host Card Emulation:  Mobile devices can emulate a contactless card using Host Card Emulation (HCE), which does not rely on a hardware secure element for storage of sensitive data such as payment card data.  The HCE is a software infrastructure solution that enables a mobile wallet app to securely communicate through the NFC controller to pass payment card credentials or payment tokens to a contactless NFC-enabled POS terminal or reader, eliminating the need to use a secure element (SE). HCE is most commonly used on Android mobile devices to support Google Pay.

&#x20;

&#x20;iv.             Mobile Wallets:  Mobile Wallets are applications/services accessed through the device that allows the wallet holder to securely access, manage and perform financial transactions like payments. Mobile Wallets like Samsung Pay and Apple Pay are specific to the device and the software and can be used as a replacement for credit and debit cards. On the other hand, other mobile/digital wallets are device agnostic and securely store the user’s payment information and passwords for numerous payment methods and websites which enables completion of transactions easily and quickly and allows the use stronger authentication like biometrics, examples of other digital wallets are Google Pay, WeChat pay, Paypal, Alipay.

&#x20;**b)     Merchant**

Merchants accept payments from customers for goods or services, through a point of sale terminal or other means like a customer scanning a QR code or input of the merchant number into their payment application. Mobile devices are also used by merchants for payments, hence another inherent source of vulnerabilities.

&#x20;**c)      Point of Sale Terminals**

A Point of Sale (POS) terminal is an electronic device used to process mobile payments at the merchant location. The communication channels between the POS terminal and the Mobile device for proximity payments is through contactless Near Field Communication (NFC), Quick Response (QR) codes or Magnetic Strip Technology (MST). 3G, 4G, and Wi-Fi are prevalently used for mobile wallets. Any risk that exists on a standard desktop or laptop computer may also exist on a mobile device.

&#x20;Along with the standard communication methods of traditional desktop and laptop computers, mobile devices may also include multiple cellular technologies (e.g., LTE and GSM), GPS, Bluetooth, infrared (IR), and near-field communication (NFC) capabilities. Risk is further increased by removable media (e.g., SIM card and SD card), the internal electronics used for testing by the manufacturer, embedded sensors, and biometric readers.

**i.            Near Field Communication (NFC)**: NFC is a wireless communication protocol based on radio-frequency technology that allows data to be exchanged between devices that are a few centimetres apart.  A wallet on an NFC-enabled mobile device is a software application stored on the mobile phone that manages and initiates payments. The mobile wallet accesses payment credentials such as tokenized payment cards, bank accounts, loyalty coupons, or financial information stored on the mobile phone in a trusted environment. The physical phone is used to initiate a payment transaction by tapping or holding the mobile device near a contactless-enabled POS terminal.

&#x20;**ii.            Magnetic Strip Technology (MST**): Magnetic Secure Transmission, or MST, generates a magnetic signal like that of a traditional payment card when swiped. The magnetic signal is then sent from the device to the POS terminal. MST is enabled on some Samsung mobile phones.

&#x20;**iii.            QR codes:** QR codes offer contactless payment alternatives in two ways:

**a.       Payer scans the merchant’s QR code**, the merchant generates a transaction QR code or displays their assigned static QR code, the payer will then scan the code using their phone camera and the payment application will interpret the payment or merchant details to initiate the transaction that can be completed by entering a PIN

**b.       Merchant scans payers QR code**; the customer through their payment application will generate a unique transaction-specific QR code to the merchant; the merchant scans the code through their payment application using a QR scanner to initiate the transaction that can be completed by entering a PIN.

&#x20;**iv.            3G/4G and WiFi**

In addition to 3G and 4G cellular networks, mobile devices can also connect to wireless (Wi-Fi) networks, these networks enable the mobile application on the device to interact with the payment service providers. 3G, 4G, and WiFi networks are usually provided by the Mobile Network Operator.

**d)     Token Service Provider (TSP)**

The TSP manages the life cycle of tokens. Additional services typically include, creating and storing tokens, managing the token lifecycle, processing token transactions, performing token-to-PAN mapping, cardholder validation, including provisioning services, key management for device-based wallets using HCE, verification services for the transaction and device validity.

**e)      Acquirer**

The acquirer is the financial institution or bank that passes the merchant's transactions along to the applicable issuing banks to receive payment.

**f)       Issuer**

The issuer is the financial institution that issues credit cards to consumers on behalf of the card networks

**g)      Wallet Service Provider (WSP)**

WSPs offer specific wallet solutions that use various communications technology for mobile payments.

**h)     Payment Service Provider (PSP)**

PSPs provide the various methods that allow a merchant to accept payments from mobile and digital wallets. The PSP can connect to multiple acquirers as well as payment and card networks. By enlisting the services of a PSP, the merchant becomes less dependent on financial institutions to manage transactions, since the PSP can manage bank accounts as well as relationships with the external network.



&#x20;
