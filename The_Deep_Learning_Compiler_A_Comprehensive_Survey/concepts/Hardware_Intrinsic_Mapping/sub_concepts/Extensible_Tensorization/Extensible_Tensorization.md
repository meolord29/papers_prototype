---
title: "Extensible Tensorization"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Extensible Tensorization

[[sub_concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Extensible tensorization is a method that enables the compiler backend to apply hardware implementations as well as highly optimized handcraft micro-kernels to a specific pattern of operations.== This approach allows DL compilers to transform high-level operations into hardware-specific instructions through pattern matching and substitution. ==The extensibility aspect means that new hardware targets can be supported by defining new tensorization rules without modifying the core compiler infrastructure.== This mechanism is crucial for achieving portability across diverse hardware architectures while maintaining high performance. The tensorization process essentially bridges the gap between abstract computation graphs and concrete hardware instructions.

## Usage in this paper

==In the paper, extensible tensorization is specifically identified as TVM's realization of hardware intrinsic mapping.== This method enables TVM to leverage vendor-provided optimized kernels while maintaining flexibility for new hardware targets. The approach demonstrates how TVM's backend optimization strategy differs from other compilers by emphasizing extensibility. This makes TVM particularly suitable for research scenarios where new hardware architectures are frequently introduced.

## References

> [!quote] Section 4 (p. 3)
> "In TVM, the hardware intrinsic mapping is realized in the method of extensible tensorization. This method enables the compiler backend to apply hardware implementations as well as highly optimized handcraft micro-kernels to a specific pattern of operations."
> *Discussion of TVM's backend optimization approach in the comprehensive survey*



## Sub-Concepts

The concept of Extensible Tensorization unfolds across three interconnected dimensions that enable DL compilers to bridge abstract operations with concrete hardware. **Hardware Intrinsic Mapping** establishes the foundation by defining how high-level operations translate to hardware-specific instructions. This directly enables **Pattern Matching and Substitution** which identifies operation patterns that can be replaced with optimized implementations. Finally, **Vendor-Optimized Kernel Integration** leverages existing optimized libraries while the extensibility architecture allows new hardware targets without modifying core infrastructure, making the system adaptable to emerging DL accelerators.

- [[sub_concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping|Hardware Intrinsic Mapping]]
- [[sub_concepts/Pattern_Matching_and_Substitution/Pattern_Matching_and_Substitution|Pattern Matching and Substitution]]
- [[sub_concepts/Vendor-Optimized_Kernel_Integration/Vendor-Optimized_Kernel_Integration|Vendor-Optimized Kernel Integration]]


## Backlinks

- [[sub_concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping]]
- [[sub_concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping]]
- [[sub_concepts/Pattern_Matching_and_Substitution/Pattern_Matching_and_Substitution]]
- [[sub_concepts/Vendor-Optimized_Kernel_Integration/Vendor-Optimized_Kernel_Integration]]
