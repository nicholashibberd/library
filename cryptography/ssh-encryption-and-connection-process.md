# SSH Encryption and Connection Process

The SSH encryption and connection process uses two types of encryption
techniques:

**Asymmetrical encryption**  (public and private keys) is used for
authentication and the establishment of a shared secret.

**Symmetrical encryption** (one key used to both encrypt and decrypt messages)
is used for encryption of the messages between the two parties

- TCP connection made by client

- Server responds with protocol versions it supports and with its public host
key

- Client checks public host key against known hosts

- Client and server use [Diffie-Hellman](https://gist.github.com/nicholashibberd/2c875828f43286484456269959c313ca)
algorithm to produce a shared private key which is used to encrypt all future
messages

SSH encryption process uses forward secrecy as new encryption keys are generated
for every connection

