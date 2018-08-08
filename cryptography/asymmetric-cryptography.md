# Asymmetric (Public Key) Cryptography

Any party can encrypt a message using the public key of the receiver, but only
the receiver can decrypt the message using their private key

Quite computationally intensive

Hybrid encryption is generally used, whereby a session key is used to encrypt
the document using symmetrical encryption, and the session key is encrypted
using the public key of the recipient. The recipient can then decrypt the
session key and using that decrypt the rest of the message
