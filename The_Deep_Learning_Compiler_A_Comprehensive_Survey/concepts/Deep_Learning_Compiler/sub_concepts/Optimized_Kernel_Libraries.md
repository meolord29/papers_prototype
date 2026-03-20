---
title: "Optimized Kernel Libraries"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Optimized Kernel Libraries

[[../Backend_Optimizations|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Optimized kernel libraries consist of pre-compiled, highly efficient routines designed for specific hardware architectures to accelerate deep learning operations. ==These libraries include Basic Linear Algebra Subprograms (BLAS) such as MKL and cuBLAS which serve as the basics for efficient computation of DL models.== ==Additionally, hardware vendors have released specially optimized libraries tailored for DL computations, including forward and backward convolution, pooling, normalization, and activation.== While effective, relying solely on these libraries often falls behind the rapid development of DL models and fails to utilize the DL chips efficiently. Consequently, compilers often integrate these libraries to handle standard operations while customizing others.

## Usage in this paper

The paper positions optimized kernel libraries as a foundational element that deep learning compilers leverage to ensure performance on standard operations. It notes that tools like TensorRT support a large collection of highly optimized GPU kernels alongside graph optimization techniques. ==However, the survey highlights that compilers are necessary to address the drawback of relying on libraries which usually fall behind the rapid development of DL models.== This integration allows compilers to balance flexibility with the raw performance of vendor-specific implementations.

## References

> [!quote] Section 1 (p. 2)
> "hardware vendors have released specially optimized libraries tailored for DL computations (e.g., MKL-DNN and cuDNN)"
> *This quote appears in the Introduction where the authors discuss existing hardware support and the limitations of relying solely on vendor libraries.*





## Backlinks

- [[../Backend_Optimizations]]
