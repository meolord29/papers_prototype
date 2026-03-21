---
title: "Optimized Kernel Library Selection"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning", "kernel-libraries", "vendor-optimization"]
depth_level: 3
weight: 7
---

# Optimized Kernel Library Selection

[[../../Operator-level_IR|← Parent]]

> [!info] Concept (Level 3)
> ==Optimized kernel library selection involves choosing from pre-validated, highly optimized implementations of common operators provided by hardware vendors or community libraries.== This approach leverages existing high-performance libraries such as BLAS, cuBLAS, MKL-DNN, and cuDNN that contain hand-tuned kernels for specific operations on specific hardware. The operator-level IR must support integration with these libraries while maintaining the flexibility to fall back to generated code when library support is unavailable. ==This sub-concept provides a balance between the reliability of proven implementations and the flexibility of compiler-generated code.== Library selection becomes particularly important for common operations where vendor optimizations have reached maturity through extensive engineering effort.

## Usage in this paper

The paper discusses optimized kernel libraries as one of the three primary backend optimization strategies enabled by operator-level IR in DL compilers. The authors note that while libraries like cuDNN and MKL-DNN provide excellent performance, they usually fall behind rapid DL model development and fail to utilize DL chips efficiently for new operations. ==The survey positions library selection as complementary to auto-tuning, creating a hybrid approach where compilers can leverage libraries when available and generate code otherwise.== ==This capability is presented as essential for achieving high performance across diverse hardware platforms.==

## References

> [!quote] Section 1 (p. 2)
> "On general-purpose hardware, the highly optimized linear algebra libraries such as Basic Linear Algebra Subprograms (BLAS) libraries (e.g., MKL and cuBLAS) serve as the basics for efficient computation of DL models."
> *Describes the role of optimized libraries in DL computation on general-purpose hardware*

> [!quote] Section 1 (p. 2)
> "However, the drawback of relying on the libraries is that they usually fall behind the rapid development of DL models, and thus fail to utilize the DL chips efficiently."
> *Explains the limitation of library-based approaches that DL compilers address*





## Backlinks

- [[../../Operator-level_IR]]
