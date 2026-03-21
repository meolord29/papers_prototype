---
title: "Hardware-Specific Kernel Libraries"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning", "kernel-libraries", "vendor-optimization"]
depth_level: 3
weight: 8
---

# Hardware-Specific Kernel Libraries

[[../../Tensor_Intrinsic_Mapping|← Parent]]

> [!info] Concept (Level 3)
> ==Hardware-Specific Kernel Libraries refer to the optimized computational kernels provided by hardware vendors for accelerating deep learning operations on specific platforms.== These libraries include highly tuned implementations like cuDNN for NVIDIA GPUs, MKL-DNN for Intel CPUs, and vendor-specific libraries for dedicated DL accelerators. They encapsulate hardware-specific optimizations such as memory access patterns, instruction scheduling, and specialized compute units like tensor cores. ==The libraries serve as the target implementations that tensor intrinsic mapping mechanisms can invoke through declarative lowering rules.== This approach allows compilers to leverage decades of vendor optimization expertise without reimplementing low-level optimizations.

## Usage in this paper

In this paper, Hardware-Specific Kernel Libraries are discussed as both a precursor to and target of tensor intrinsic mapping approaches. The survey explains how DL frameworks traditionally convert operations to library calls like GEMM functions in BLAS libraries. ==However, the paper notes that relying solely on libraries falls behind rapid DL model development, motivating compiler-based approaches.== Tensor intrinsic mapping bridges this gap by enabling compilers to selectively invoke these libraries while maintaining flexibility for new operations.

## References

> [!quote] Section 2 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Explaining the role of optimized libraries in DL computation before introducing compiler approaches*





## Backlinks

- [[../../Tensor_Intrinsic_Mapping]]
