# Asymmetric Encryption: Enhancing Security in Communication

## Onderwerp
Asymmetric encryption, also known as public-key cryptography, is a method of encryption where two different keys are used for encryption and decryption. This technique provides a more secure way of exchanging sensitive information compared to symmetric encryption.

## Key-terms
1. **Asymmetric Encryption**: A cryptographic technique that uses a pair of keys - public and private - to encrypt and decrypt messages.
2. **Public Key**: A key that is shared publicly and used for encrypting messages.
3. **Private Key**: A key that is kept secret and used for decrypting messages.
4. **Key Pair**: A combination of a public key and a private key.
5. **Cryptography**: The practice and study of techniques for secure communication.

## Opdracht
1. Generate a key pair using a key pair generator tool like [JSEncrypt](https://travistidwell.com/jsencrypt/demo/).
2. Share the public key on the public Slack channel.
3. Encrypt a message using the recipient's public key.
4. Send the encrypted message to the recipient via the public Slack channel.
5. The recipient decrypts the message using their private key.

## Gebruikte bronnen
- [JSEncrypt Demo](https://travistidwell.com/jsencrypt/demo/)
- [Wikipedia - Public-key Cryptography](https://en.wikipedia.org/wiki/Public-key_cryptography)

## Ervaren problemen
During the exercise, one potential problem is ensuring the authenticity of the public key. Without proper verification, there's a risk of a man-in-the-middle attack where an attacker intercepts the public key and substitutes their own, allowing them to decrypt and read messages intended for the recipient.

To mitigate this issue, it's essential to establish a secure channel for sharing public keys, such as using a trusted website or verifying the key through other secure means.

## Resultaat

![error](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/56a81453b212b54166b188098cd3e45b75e86ea2/00_includes/Security1/Asymmetric%20encryption/Schermafbeelding%202024-04-03%20152746.png)

![error](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/56a81453b212b54166b188098cd3e45b75e86ea2/00_includes/Security1/Asymmetric%20encryption/Schermafbeelding%202024-04-03%20164522.png)