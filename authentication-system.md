# Proposal: A decentralized solution to authenticate documents, people and identity.

## Abstract: 

- #### is it necessary :
For long, giant tech companies have undertaken the task of securing and validating our two factor authentications. [Google](https://www.google.com/landing/2step/) and [Apple](https://support.apple.com/en-in/HT204915) being one of the many centralized ones out there. 
Banks, Exchanges and many instutions require the use of 2 Factor Authentication to identify their customers. 2 factor Authentication plays an important role in not only securing the identity of a person but also prevent uncalculated, unintended actions by malicius entities. It is by all means a grave necessity in our digital lives.

We encounter many instances where independent entities implement 2 Factor authentication to independently establish and secure their customer's user journey where ~~~__Needs to be completed!__~~

- #### Why :

As Muneeb Ali rightly said, no single entity should have as much power such that the world relies simply on that single entity not choosing to be evil. 2 Factor authentication is extremely important to the vast majority of our population and it being administered by a single entity leads to a single point of failure despite their best attempts to thwart it.

- #### Solution :
A platform to serve as a one stop solution for all authentication requests.

- #### Working:
  - Authenticator:
    A person intending to authenticate someone requests the platform named say authenticato to issue a session key encrypted with the authenticator's public key.
Authenticato issues a session key signed with the platform's private key to be verified and then decrypted by the authenticator. The session key with authenticato's signature is signed again with the authenticator's private key and then sent across a secure channel to the person requesting to be authenticated(Authentee). The authentee receives a signed session key from the authenticator within which lies authenticato's signature as well.
Authentee verifies both signatures againts their public key available on authenticato and then appends their (authentee) signature to a hash generated from a nonce+private key that they(authentee) alone knows.

The signature and the hash sent by the authentee is encrypted and stored for a defined duration on the authentee's machine as a cookie or a file that can be used to further extend the period of duration for which the access key is valid.

 - Authenticato:

 - Authentee:

###### References:
- [Wikipedia 2 Factor Authentication](https://en.wikipedia.org/wiki/Multi-factor_authentication)
- [![](https://img.youtube.com/vi/qtOIh93Hvuw/maxresdefault.jpg)](https://www.youtube.com/watch?v=qtOIh93Hvuw)
