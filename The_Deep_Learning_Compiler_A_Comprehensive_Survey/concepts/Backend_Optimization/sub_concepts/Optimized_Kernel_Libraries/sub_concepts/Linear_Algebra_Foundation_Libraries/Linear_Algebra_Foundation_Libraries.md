---
title: "Linear Algebra Foundation Libraries"
date: 2026-03-20
tags: ["concept", "depth-3"]
depth_level: 3
weight: 7
---

# Linear Algebra Foundation Libraries

[[../../Optimized_Kernel_Libraries|← Parent]] → [[../../../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 3)
> Linear algebra foundation libraries represent the computational backbone upon which deep learning operations are built, providing highly optimized implementations of basic mathematical operations. ==These libraries include Basic Linear Algebra Subprograms (BLAS) such as MKL and cuBLAS that serve as the basics for efficient computation of DL models on general-purpose hardware.== ==DL frameworks often convert complex operations like convolution into matrix multiplication and then invoke GEMM functions from these BLAS libraries for execution.== This approach leverages decades of optimization work in numerical computing to accelerate DL workloads efficiently. The foundation libraries enable hardware vendors to build more specialized DL libraries on top of these proven computational primitives.

## Usage in this paper

The paper positions linear algebra foundation libraries as the computational basics that enable efficient DL model execution on general-purpose hardware. ==The survey explains that on general-purpose hardware, these highly optimized linear algebra libraries serve as the fundamentals for DL computation.== ==DL compilers build upon this foundation by incorporating these libraries into their backend optimization strategy while adding additional DL-specific optimizations.== This layered approach allows compilers to leverage mature, well-optimized code while extending functionality for emerging DL requirements.

## References

> [!quote] Section 1 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Explanation of BLAS libraries as computational foundation for DL*





## Backlinks

- [[../../Optimized_Kernel_Libraries]]
