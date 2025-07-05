# HQC Cryptosystem in SageMath (Python)

This repository contains an implementation of the **Hamming Quasi-Cyclic (HQC)** public-key encryption scheme, built using [SageMath](https://www.sagemath.org/). It includes full encoding/decoding routines and demonstrations of known vulnerabilities to help understand its cryptographic behavior.

## Academic Purpose

This implementation was developed as part of my Master's thesis in cryptography. It serves both as a functional HQC cryptosystem and a study of potential misuse scenarios that break its security guarantees.

## What is HQC?

HQC is a post-quantum cryptographic scheme based on **code-based encryption**, relying on **Reed-Solomon** and **Reed-Muller** codes. It has been submitted to the NIST post-quantum cryptography standardization process.

Official paper: [HQC Specification (2025-02-19)](https://pqc-hqc.org/doc/hqc-specification_2025-02-19.pdf)

## Files

- `hqc.ipynb`: Main SageMath notebook implementing the HQC cryptosystem.
  - Key generation (`hqc_keygen`)
  - Encryption (`hqc_encrypt`)
  - Decryption (`hqc_decrypt`)
  - Reed-Muller and Reed-Solomon encoders/decoders
  - Sparse vector and polynomial utility functions
  - Examples 
  - Attacks

## Requirements

- [SageMath](https://www.sagemath.org/) — tested with version 10.6
- Python ≥ 3.8 (bundled with SageMath)

To run:
```bash
sage -n jupyter
# Open `hqc.ipynb` in your browser
```

## Security Warning

This implementation is for educational and research purposes only. This is not suitable for production or secure communication. Do not use this code in real-world systems.
