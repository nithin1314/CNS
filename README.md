# CNS
RSA Digital Signature Scheme
This project implements a RSA Digital Signature Scheme using Python to demonstrate how public and private keys can be used to sign and verify the authenticity of messages. The scheme uses asymmetric cryptography to ensure the integrity and non-repudiation of the data being transmitted.

Overview
The RSA algorithm is a widely used asymmetric cryptographic system that utilizes a pair of keys: a public key (known to everyone) and a private key (kept secret). The primary goal of this system is to allow secure communications and validate the integrity of messages through digital signatures.

This implementation generates RSA key pairs (public and private), signs messages with the private key, and verifies the signature with the public key to confirm the authenticity of the message.

Features
Key Generation: Generates RSA public and private key pairs.
Message Signing: Signs a message using the private key.
Signature Verification: Verifies the authenticity of a message by checking its digital signature with the public key.
Mathematical Foundations: Includes implementations for:
Euclidean Algorithm: Used to compute the greatest common divisor (GCD).
Extended Euclidean Algorithm: Used to find the multiplicative inverse for key generation in RSA.
Dependencies
rsa: A Python package used to implement the RSA cryptography and digital signature algorithms.
Functions
generate_keys(): Generates RSA key pairs (public and private keys) with 2048-bit security.
sign_message(message, private_key): Signs a given message using the private key.
verify_signature(message, signature_hex, public_key): Verifies the digital signature of a message using the public key.
euclid(m, n): Computes the greatest common divisor (GCD) of two numbers using the Euclidean algorithm.
exteuclid(a, b): Computes the multiplicative inverse of a number modulo another using the extended Euclidean algorithm.
