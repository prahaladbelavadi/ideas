# Conditions:

The password entered to validate the authenticity of a person is visible to everyone.
The password must be different the next time entered.

# Proposal:

An automatic password changing mechanism system that changes upon each use allowing the user to publicly enter or grant one time access to anything.
------------------------------------------
# Solution:

![One way hashing](https://www.cs.rit.edu/~ark/lectures/onewayhash/SHA256Fig1.png)

  E(x,y) -> C
  D(x,C) -> y
  Where 
  - E(x,y) means encryption of x,y
  - D(x,C) mans decryption of x,C
  - x is seed password(can be anything)
  - y is salt or a Pseudo random generated recorded string to randomize entry

- Recursive One way hash
  One way hash of the seed password is recursively hashed to a certain number of times to yeild C<sub>n</sub> where the seed password has been hashed n number of times.
  
# Usage: 
    C<sub>n</sub> has to be parsed to the server to authenticate and verify the identity of the person.
    Upon being authenticated once, C<sub>n-1</sub> needs to be parsed to the server to authenticate and verify the identity of the person for the second time.
    
    
    
Resources:
- Bruce 's book introduction to applied cryptography
