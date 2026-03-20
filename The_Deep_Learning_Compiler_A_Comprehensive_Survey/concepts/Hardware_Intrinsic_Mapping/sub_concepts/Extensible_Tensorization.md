---
title: "Extensible Tensorization"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Extensible Tensorization

[[../Hardware_Intrinsic_Mapping|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Extensible tensorization is a mechanism that allows compilers to declare hardware intrinsic behavior and define lowering rules for specific operation patterns.== This approach enables the compiler to transform high-level intermediate representation instructions into highly optimized kernel implementations that are tailored for specific hardware architectures. The extensibility aspect means that new hardware intrinsics can be added without modifying the core compiler infrastructure, providing flexibility for supporting emerging hardware features. This technique is particularly important for deep learning workloads where operations like matrix multiplication and convolution dominate computation time. ==By enabling custom tensorization rules, compilers can leverage vendor-specific optimizations that would otherwise be inaccessible through generic code generation.==

## Usage in this paper

==In this paper, extensible tensorization is presented as TVM's primary approach to realizing hardware intrinsic mapping within the backend optimization framework.== The paper explains that TVM uses this mechanism to map IR patterns to hardware-specific implementations, enabling significant performance gains on diverse DL hardware. ==This optimization is discussed as one of five widely adopted backend optimization approaches in Section 4.4.1, highlighting its importance in the DL compiler ecosystem.== The approach allows TVM to support various hardware targets without requiring complete redesign of the compilation pipeline.

## References

> [!quote] Section 4.4.1 (p. 15)
> "TVM realizes this through extensible tensorization that declares hardware intrinsic behavior and lowering rules"
> *Describing TVM's approach to hardware intrinsic mapping in backend optimizations*

> [!quote] Section 1 (p. 2)
> "To embrace the hardware diversity, it is important to map the computation to DL hardware efficiently"
> *Explaining the motivation for hardware-specific optimization techniques*





## Backlinks

- [[../Hardware_Intrinsic_Mapping]]
