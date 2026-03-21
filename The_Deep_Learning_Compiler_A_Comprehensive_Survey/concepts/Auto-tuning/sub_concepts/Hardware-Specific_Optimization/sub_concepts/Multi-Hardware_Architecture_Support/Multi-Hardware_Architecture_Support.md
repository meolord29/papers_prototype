---
title: "Multi-Hardware Architecture Support"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 9
---

# Multi-Hardware Architecture Support

[[../../Hardware-Specific_Optimization|← Parent]]

> [!info] Concept (Level 3)
> ==Multi-hardware architecture support refers to the capability of DL compilers to efficiently map computations across diverse DL hardware categories and vendor platforms.== The paper identifies three main hardware categories: general-purpose hardware with software-hardware co-design, dedicated hardware fully customized for DL models, and neuromorphic hardware inspired by biological brain science. Examples include Google TPU, NVIDIA Turing, Intel NNP, and specialized accelerators from startups like Cambricon and Graphcore. ==Each hardware type has unique computing characteristics such as matrix multiplication engines, tensor cores, and high-bandwidth memory that require different optimization approaches.== The ability to generate hardware-optimized code automatically across these diverse platforms reduces engineering burden and improves portability.

## Usage in this paper

==The paper emphasizes that DL compilers must map computation to diverse DL hardware efficiently, which is a core challenge addressed by hardware-specific optimization.== It notes that the design of DL hardware would become even more diverse in the foreseeable future, making multi-hardware support increasingly critical. ==The survey highlights that DL compilers leverage mature tool-chains from general-purpose compilers like LLVM to provide better portability across diverse hardware architectures.== This demonstrates how multi-hardware support is integral to the hardware-specific optimization goal in DL compiler design.

## References

> [!quote] Section 1 (p. 1)
> "Generally, the DL hardware can be divided into the following categories: 1) general-purpose hardware with software-hardware co-design, 2) dedicated hardware fully customized for DL models, and 3) neuromorphic hardware inspired by biological brain science."
> *Categorizing different types of DL hardware architectures*

> [!quote] Section 1 (p. 2)
> "Moreover, existing DL compilers also leverage mature tool-chains from general-purpose compilers (e.g., LLVM), which provides better portability across diverse hardware architectures."
> *Explaining how DL compilers achieve hardware portability*





## Backlinks

- [[../../Hardware-Specific_Optimization]]
