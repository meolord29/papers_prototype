---
title: "Vendor-Optimized Kernel Integration"
date: 2026-03-20
tags: ["concept", "depth-3"]
depth_level: 3
weight: 8
---

# Vendor-Optimized Kernel Integration

[[../../Extensible_Tensorization|← Parent]] → [[../../../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 3)
> ==Vendor-optimized kernel integration refers to the capability of DL compilers to leverage existing highly optimized libraries provided by hardware vendors.== These libraries include Basic Linear Algebra Subprograms (BLAS) libraries such as MKL and cuBLAS that serve as basics for efficient computation of DL models. Hardware vendors have released specially optimized libraries tailored for DL computations including forward and backward convolution, pooling, normalization, and activation. The extensible tensorization approach allows compilers to integrate these vendor libraries while maintaining flexibility for custom implementations. ==This integration is crucial for achieving competitive performance without reinventing optimized kernels for every hardware target.==

## Usage in this paper

==In the paper, extensible tensorization enables TVM to leverage vendor-provided optimized kernels while maintaining flexibility for new hardware targets.== The approach demonstrates how TVM's backend optimization strategy differs from other compilers by emphasizing extensibility. This makes the compiler adaptable to the rapidly developing landscape of DL hardware from various vendors.

## References

> [!quote] Section 2 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Describes vendor-optimized libraries used for DL computation*





## Backlinks

- [[../../Extensible_Tensorization]]
