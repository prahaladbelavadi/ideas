# DRM management tool

__Proposal__: An open source tool for excercising DRM rights.

Obtaining a file must bring with it a signature of the author and publishing house. 
People can verify if the content is authentic and from the author and publishing house. 

Author provided must be able to:
- Sign the file and include his public address in the file's keyring
- Obtain the buyer's public key and encrypt the signed(Author's signature) file  with the buyer's public key such that nobody apart from the buyer can view the contents of the file.
- Enforce his rules over who views his content and make availability for previews (Ability to revoke keys)
- Provide options for his buyers to share his content by adding their intended-share recipient's public key to the file's keyring enforcing a chain of public keys to determine who bought it and how it travels along.
- Obtain royalties through sharing, buying and selling of his content beyond the initial point of sale.

For different licences, different structure of implementation is followed from which the author can secure his content and the content is linked to the author for verification.

**Disclaimer:**
This is not intended to replace publishing houses or any middlemen albeit that could be a possibility if the author decided to self publish. 
However, publishing houses, middlemen and marketplaces have their own respective roles to play.
This is intended to remain open source such that everyone has an equal opportunity, however if someone wishes otherwise, there isn't much we can do apart from gaining a significantly larger traction on our open source version.

_This is work in progress_ :)
