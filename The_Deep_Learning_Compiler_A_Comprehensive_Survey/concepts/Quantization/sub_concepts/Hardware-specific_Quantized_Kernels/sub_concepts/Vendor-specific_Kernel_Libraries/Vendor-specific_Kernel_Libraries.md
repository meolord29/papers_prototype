---
title: "Vendor-specific Kernel Libraries"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning", "vendor-libraries", "kernel-optimization"]
depth_level: 3
weight: 7
---

# Vendor-specific Kernel Libraries

[[../../Hardware-specific_Quantized_Kernels|← Parent]]

> [!info] Concept (Level 3)
> Vendor-specific kernel libraries are specialized computational libraries provided by hardware manufacturers that contain highly optimized implementations of common deep learning operations. ==These libraries include examples such as NVIDIA's cuDNN and cuBLAS, Intel's MKL-DNN, and other architecture-specific implementations tailored for their hardware.== ==Each library exploits unique architectural features like tensor cores, vector units, or specialized memory hierarchies to maximize performance.== The libraries typically cover fundamental operations including convolution, pooling, normalization, and activation functions. Maintaining compatibility with these diverse vendor libraries presents significant engineering challenges for compiler developers who must support multiple hardware platforms simultaneously.

## Usage in this paper

The paper positions vendor-specific kernel libraries as foundational building blocks that DL compilers leverage for backend optimization. ==The survey notes that on general-purpose hardware, highly optimized linear algebra libraries such as BLAS serve as the basics for efficient computation of DL models.== DL compilers can invoke these vendor libraries to generate efficient code implementations on various DL hardware without manual optimization. However, the paper also notes the drawback that these libraries usually fall behind the rapid development of DL models, motivating compiler-based solutions.

## References

> [!quote] Section 2 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Explaining how DL frameworks utilize optimized libraries for efficient computation*





## Backlinks

- [[../../Hardware-specific_Quantized_Kernels]]
