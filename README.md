## Experiment 1: Private Blockchain
## Aim:

To implement a secure passwordless authentication system in PrivateBlock using public–private key cryptography, where users authenticate by signing a challenge instead of using passwords.

## Algorithm
Step 1: 
The user provides their public key to the system. The system stores this key as the user’s identity.

Step 2: 
When the user wants to log in, the system creates a random challenge (nonce) and sends it to the user.

Step 3: 
The user signs the challenge using their private key and sends the signature back to the system.

Step 4: 
The system verifies the signature using the stored public key.
If valid, the user is successfully authenticated.
