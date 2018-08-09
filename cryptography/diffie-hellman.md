# Diffie-Hellman

A method of securely exchanging cryptographic keys over a public network
(key-exchange algorithm)

- Two parties agree on an arbitary shared public key (large integer)
- Each produce a private key which they do not share with the other
- Each produce a new (different) key to send to the other by apply their private
key to the shared key.
- The other party can then apply their private key to the provided key to create
a matching private secret key
- This private secret key is a symmetric key used for encrypting and decrypting
messages from this point on.
