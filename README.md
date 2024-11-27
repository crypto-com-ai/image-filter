# Running Machine Learning models on Blockchain

To enable machine learning models to operate on a blockchain, two critical aspects need to be addressed:

1. **Privacy-Preserving Machine Learning**: Ensuring that sensitive data remains confidential during the entire
   process of training and inference.
2. **Zero-Knowledge Proof of Inference**: Verifying the correctness of an ML inference without revealing the
   model's inputs, outputs, or weights.

This demo focuses on the privacy-preserving machine learning aspect and introduces Fully Homomorphic Encryption
(FHE) as the foundation for achieving this.

## What is Fully Homomorphic Encryption?

Fully Homomorphic Encryption (FHE) is a form of encryption that allows computations to be performed directly on
encrypted data, without the need to decrypt it. This ensures that the dta remains private and secure throughout
the computation process.

### Key features of FHE

- **Confidentiality**: Raw data is never exposed. All operations occur on encrypted data, ensuring end-to-end
  privacy.
- **Computation over Encryption**: It supports arbitrary mathematical operations on ciphertexts. The result,
  when decrypted, is the same as if operations had been performed on plaintext data.
- **Decentralized ML Inference**: Using FHE, blockchain nodes can execute ML inferences on encrypted data,
  maintaining user privacy while leveraging the power of decentralized computation.

## Why FHE for privacy preserving ML?

In blockchaiun environments, where data is inherently decentralized and transparent, FHE is essential to:

- Protect sensitive data from being exposed to unauthorized entities.
- Enable secure ML inference on the blockchain while preserving both user privacy and the confidentiality of
  the ML model.

By employing FHE, ML computations can be securely outsourced to a decentralized network, paving the way for
secure and scalable on-chain machine learing.


## Run the application on your machine

### Install dependencies

First, create a virtual env and activate it:

```bash
`python3 -m venv .venv`
source .venv/bin/activate
```

Then, install required packages:

```bash
pip3 install pip --upgrade
pip3 install -U pip wheel setuptools --ignore-installed
pip3 install -r requirements.txt --ignore-installed
```

The above steps should only be done once.

## Run the app 

In a terminal, run:

```bash
source .venv/bin/activate
python3 generate_dev_files.py
python3 app.py
```

## Interact with the application

Open the given URL link (search for a line like `Running on local URL:  http://127.0.0.1:8888/`).
