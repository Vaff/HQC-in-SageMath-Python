# HQC Cryptosystem in SageMath (Python)

This repository contains an implementation of the **Hamming Quasi-Cyclic (HQC)** public-key encryption scheme, built using [SageMath](https://www.sagemath.org/). It includes both encoding/decoding routines and illustrative cryptanalysis demonstrating known vulnerabilities.

## 🔐 What is HQC?

HQC is a post-quantum cryptographic scheme based on **code-based encryption**. It combines **Reed-Solomon** and **Reed-Muller** codes over GF(2^8), leveraging their concatenation to encode messages securely.

## 📁 Files

- `hqc.ipynb`: Main SageMath notebook implementing the HQC cryptosystem.
  - Key generation (`hqc_keygen`)
  - Encryption (`hqc_encrypt`)
  - Decryption (`hqc_decrypt`)
  - Reed-Muller and Reed-Solomon encoder/decoder functions
  - Sparse vector and polynomial utility functions
  - Example usage with performance metrics
  - ⚠️ Cryptanalysis demos showing how key or randomness reuse breaks security

## 🚀 Requirements

- [SageMath](https://www.sagemath.org/) (tested with version XX — _please specify if possible_)
- Python ≥ 3.8 (comes bundled with SageMath)

To run the notebook:
```bash
sage -n jupyter
# Then open `hqc.ipynb` in your browser
