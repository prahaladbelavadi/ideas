# Proposal:
   Nonce concept session key issued by the blockchain to have tokenless blockchains.
   
   The blockchain issues nonces(non repeating entity) upon a request made to the protocol.
   The nonces issued are session keys that are differerent each time and valid for that particular instance only.
   
   The information to be stored are signed by the necesaary authority and encrypted under that session key.
   
   The session key holds the time stamp and a signature that ensures that the protocol released the token for the person that requested it
   and no one else.
   
   The session keys is relayed back with the encrypted information and the transaction is recorded by the blockchain.
   
   The recepient has an option to unlock the information by signing for the transaction that releases the information.
   
   The sender knows that the information has been read when the transaction is signed for and the session key stays valid until signed for.
   
   Upon expiry of the session key, the sender knows that the message encrypted has been read and signed for by the recepient authority. 
