## OBC IDENTITY MANAGEMENT (MEMBERSHIP SERVICE)
&nbsp;
##### What is unique about OBC’s membership service module?
The design and implementation of the membership service module encompass many of the latest advances in cryptography, which we believe make it stand apart from other alternatives.

In addition to supporting generally-expected requirements such as preserving the privacy of transactions and making them auditable, OBC’s membership service module also introduces the concept of enrollment and transaction certificates. Infinite number of transaction certificates can be generated from their parent enrollment certificates (issued to validated users). This design ensures that asset tokens (which can be represented by transaction certificates) can only be created by verified owners, and private keys of asset tokens can be regenerated if lost. 

Furthermore, the design of the system allows transaction certificates to both expire and be revoked, which allows issuers to have greater control over the asset tokens they issued on a distributed chain.

Finally, like most other modules on OBC, you can always replace the default membership service implementation with another option.


&nbsp;
##### Would its membership service make OBC a centralized solution?

No, because membership service does not provide, deploy, validate, or execute transactions and business logics. Membership service’s only role is to issue digital certificates to validated entities wishing to participate in an OBC network, and it does not aware how and when these certificates are used in any particular OBC network.

Membership service does, however, server as the central regulator of the OBC networks it is servicing, as the certificates issued by the membership service are used by OBC networks to regulate and manage their users.
