---
title: "Optimized Kernel Libraries"
date: 2026-03-20
tags: ["concept", "depth-3"]
depth_level: 3
weight: 7
---

# Optimized Kernel Libraries

[[../../Backend_Optimization|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 3)
> Optimized kernel libraries are vendor-provided collections of pre-optimized functions tailored for specific hardware architectures. ==These libraries include implementations like cuBLAS, MKL-DNN, and cuDNN that provide highly efficient operations for convolution, pooling, normalization, and activation.== They serve as the foundation for efficient computation by leveraging years of hardware-specific tuning and optimization expertise. ==However, relying solely on libraries has drawbacks as they usually fall behind the rapid development of DL models.== DL compilers integrate these libraries while also generating custom kernels when needed for flexibility.

## Usage in this paper

The paper discusses optimized kernel libraries as part of backend optimizations alongside hardware-specific optimization and auto-tuning. It notes that on general-purpose hardware, highly optimized linear algebra libraries such as BLAS serve as the basics for efficient computation of DL models. The survey explains that hardware vendors have released specially optimized libraries tailored for DL computations. This component is presented as essential for practitioners evaluating DL compiler capabilities.

## References

> [!quote] Section 1 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Explanation of library-based optimization approaches for DL hardware*





## Backlinks

- [[../../Backend_Optimization]]
- [[sub_concepts/Vendor-Specific_DL_Libraries/Vendor-Specific_DL_Libraries]]
- [[sub_concepts/Linear_Algebra_Foundation_Libraries/Linear_Algebra_Foundation_Libraries]]
- [[sub_concepts/Advanced_Optimization_Tools/Advanced_Optimization_Tools]]
