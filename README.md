
## Modified version of Aleo’s snarkVM with Optimized CUDA MSM & NTT

This repository is a fork of [Aleo’s snarkVM](https://github.com/AleoHQ/snarkVM) that integrates a custom, **optimized CUDA backend** for MSM (Multi-Scalar Multiplication) and NTT (Number Theoretic Transform) operations.

This version uses a **privately maintained fork of the `sppark` cryptographic library** for further optimization and experimental CUDA acceleration.

## 2. Build Guide

You can build this version of `snarkvm` from source as follows:

```bash
# Clone the repository (staging branch only)
git clone --branch staging --single-branch https://github.com/vargaconsulting/snarkVM.git
cd snarkVM

# Build and install snarkVM
cargo install --path .
```

To run `snarkvm`:

```bash
snarkvm
```


## License
## Proprietary CUDA Optimized Library

**Notice:**
This repository integrates a proprietary CUDA-accelerated library for MSM and NTT. The CUDA components are not included in this public codebase and are **not covered by the Apache 2.0 license**.
If you are interested in access, licensing, or consulting related to the CUDA optimizations, please contact [Steven Varga](mailto:steven@vargaconsulting.ca).

**The original codebase is licensed under the [Apache License, Version 2.0](./LICENSE).**
All modifications to open-source components comply with Apache v2.0 requirements.
