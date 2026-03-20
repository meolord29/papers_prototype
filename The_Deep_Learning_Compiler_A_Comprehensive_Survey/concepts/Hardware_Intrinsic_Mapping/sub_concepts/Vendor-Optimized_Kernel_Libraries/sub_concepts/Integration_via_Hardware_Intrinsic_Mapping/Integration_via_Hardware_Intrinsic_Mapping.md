---
title: "Integration via Hardware Intrinsic Mapping"
date: 2026-03-20
tags: ["concept", "depth-3"]
depth_level: 3
weight: 8
---

# Integration via Hardware Intrinsic Mapping

[[../../Vendor-Optimized_Kernel_Libraries|← Parent]] → [[../../../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 3)
> Integration via hardware intrinsic mapping represents the mechanism by which DL compilers connect high-level operations to vendor-optimized library functions during code generation. ==This approach allows compilers to transform intermediate representation operations to invoke these library functions rather than generating generic code from scratch.== ==Hardware intrinsic mapping serves as a bridge between the compiler's optimization pipeline and the actual target implementations provided by vendors.== The mapping rules reference specific library functions during the backend code generation phase to ensure optimal hardware utilization. This integration strategy enables compilers to leverage years of vendor optimization work while maintaining flexibility for operations not covered by libraries.

## Usage in this paper

The paper discusses hardware intrinsic mapping as a key backend optimization technique that DL compilers employ to leverage vendor libraries efficiently. This mechanism is contrasted with pure compiler-generated code to highlight the tradeoffs between library dependency and optimization flexibility. ==The survey positions intrinsic mapping as part of the broader backend optimization strategy alongside auto-tuning and hardware-specific optimizations.== This integration approach is presented as essential for achieving competitive performance across diverse hardware targets without reinventing optimization efforts.

## References

> [!quote] Section 1 (Introduction) (p. 2)
> "However, the drawback of relying on the libraries is that they usually fall behind the rapid development of DL models, and thus fail to utilize the DL chips efficiently."
> *Discussing limitations of library-based integration approaches*

> [!quote] Section 1 (Introduction) (p. 2)
> "To address the drawback of DL libraries and tools, as well as alleviate the burden of optimizing the DL models on each DL hardware manually, the DL community has resorted to the domain specific compilers for rescue."
> *Explaining the motivation for compiler-based solutions beyond library integration*





## Backlinks

- [[../../Vendor-Optimized_Kernel_Libraries]]
