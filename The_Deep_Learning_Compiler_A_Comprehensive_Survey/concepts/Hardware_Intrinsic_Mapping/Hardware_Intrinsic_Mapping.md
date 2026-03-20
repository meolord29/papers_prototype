---
title: "Hardware Intrinsic Mapping"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 9
---

# Hardware Intrinsic Mapping

[[../../../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Hardware intrinsic mapping transforms specific low-level IR instructions to highly optimized kernels on the hardware.== This technique allows the compiler to leverage handcrafted micro-kernels provided by hardware vendors for specific operations. ==It results in significant performance gains by utilizing specialized instructions like SIMD or tensor cores.== Without this mapping, compilers might generate generic code that underutilizes hardware capabilities. ==It is a key component of backend optimization strategies.==

## Usage in this paper

In TVM, the hardware intrinsic mapping is realized in the method of extensible tensorization. ==This method enables the compiler backend to apply hardware implementations as well as highly optimized handcraft micro-kernels to a specific pattern of operations.== Whereas, Glow supports hardware intrinsic mapping such as quantization. This shows how different compilers implement mapping to suit their specific design goals.

## References

> [!quote] Section 4.4.1 (p. 17)
> "Hardware intrinsic mapping can transform a certain set of low-level IR instructions to kernels that have already been highly optimized on the hardware."
> *Defines the function of intrinsic mapping in backend optimization.*



## Sub-Concepts

The concept of Hardware Intrinsic Mapping unfolds across three interconnected implementation strategies within DL compilers. **Extensible Tensorization** establishes the foundational mechanism by enabling compilers to apply hardware-specific implementations to operation patterns, which directly enables **Vendor-Optimized Kernel Libraries** to be leveraged for maximum performance. These libraries provide the actual optimized kernels that tensorization maps to, while **Quantization Support** represents a specialized form of intrinsic mapping that targets reduced precision hardware capabilities. Together, these sub-concepts demonstrate how different DL compilers implement hardware intrinsic mapping to suit their specific design goals, with TVM emphasizing extensibility and Glow focusing on quantization optimizations.

- [[../../Extensible_Tensorization|Extensible Tensorization]]
- [[../../../Vendor-Optimized_Kernel_Libraries/Vendor-Optimized_Kernel_Libraries|Vendor-Optimized Kernel Libraries]]
- [[../../../Quantization_Support/Quantization_Support|Quantization Support]]


## Backlinks

- [[../../Extensible_Tensorization]]
- [[../../../Vendor-Optimized_Kernel_Libraries/Vendor-Optimized_Kernel_Libraries]]
- [[../../../Quantization_Support/Quantization_Support]]
