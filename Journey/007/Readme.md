# SEC01-AWS200 — Create a new CMK in KMS and encrypt an object

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/176993446-44d35c72-72b5-49ed-bc21-378728708950.png" height="400" width="800" ></p>

## Introduction

✍️ Why? 
- AWS KMS keys (KMS keys) are the primary resource in AWS KMS. You can use a KMS key to encrypt, decrypt, and re-encrypt data. It can also generate data keys that you can use outside of AWS KMS. Typically, you'll use symmetric encryption KMS keys, but you can create and use asymmetric KMS keys for encryption or signing, and create and use HMAC KMS keys to generate and verify HMAC tags.

## Prerequisite

✍️ What?
- An AWS KMS key is a logical representation of a cryptographic key. A KMS key contains metadata, such as the key ID, key spec, key usage, creation date, description, and key state. Most importantly, it contains a reference to the key material that is used when you run cryptographic operations with the KMS key.

- You create KMS keys in AWS KMS. Symmetric KMS keys and the private keys of asymmetric KMS key never leave AWS KMS unencrypted. To use or manage your KMS keys, you must use AWS KMS. For information about creating and managing KMS keys, see Managing keys. For information about using KMS keys, see the AWS Key Management Service API Reference.

- By default, AWS KMS creates the key material for a KMS key. You cannot extract, export, view, or manage this key material. Also, you cannot delete this key material; you must delete the KMS key. However, you can import your own key material into a KMS key or create the key material for a KMS key in the AWS CloudHSM cluster associated with an AWS KMS custom key store.

- AWS KMS also supports multi-Region keys, which let you encrypt data in one AWS Region and decrypt it in a different AWS Region.


## Cloud Service Provider
- Amazon Web Services

## Difficulty

- Level 200 (Intermediate)

## Project's Author(s)

- [Andrew Brown](https://twitter.com/andrewbrown)

## Objectives

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/176993520-440aa364-2fa4-4104-812e-7376fa415084.png" height="400" width="800" ></p>

### You need to complete the following:

- Create a new Customer Master Key (CMK) in Key Management Service (KMS)
- Create a new S3 bucket
- Upload an object (file) to the S3 Bucket
- Encrypt the uploaded file with your custom CMK

### You need to answer the following:

- What is a Hardware Security Module (HSM)?
- What is the difference between multi-tenant and single-tenant HSM?
- What is the cost for for CloudHSM?
- What is key rotation?
- How much do KMS keys cost?

## Ideas

- Creating a single CMK key will result in $1 USD per month so ensure
  you delete your key at the end of this project.

## References

- [Key Management Service](https://aws.amazon.com/kms/)
- [CloudHSM](https://aws.amazon.com/cloudhsm/)
- [AWS Key Management Service concepts](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html)
