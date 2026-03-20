---
title: "Multi-level IR"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 10
---

# Multi-level IR

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Multi-level IR refers to the layered design where different abstraction levels of intermediate representations are used throughout the compilation pipeline.== High-level IR captures computation graphs with rich semantic information for graph-level optimizations, while low-level IR provides fine-grained representation for hardware-specific optimizations. ==This design allows DL compilers to apply both hardware-independent and hardware-dependent optimizations at appropriate abstraction levels.== The separation enables better portability across diverse hardware architectures while maintaining optimization effectiveness.

## Usage in this paper

==This concept is central to the paper's analysis, with Section 4.1 dedicated to high-level IR and Section 4.2 to low-level IR.== The authors classify high-level IR implementations into DAG-based, let-binding-based, and tensor computation representations. Low-level IR is categorized into Halide-based, polyhedral-based, and other unique IRs.

## References

> [!quote] Section 3 (p. 7)
> "However, the uniqueness of DL compiler lies in the design of multi-level IRs and DL specific optimizations."
> *Identifies multi-level IR as the key differentiator for DL compilers*



## Sub-Concepts

- [[sub_concepts/High-Level_Intermediate_Representation|High-Level Intermediate Representation]]
- [[sub_concepts/Low-Level_Intermediate_Representation|Low-Level Intermediate Representation]]
- [[sub_concepts/Multi-Level_IR_Architecture|Multi-Level IR Architecture]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/High-Level_Intermediate_Representation]]
- [[sub_concepts/Low-Level_Intermediate_Representation]]
- [[sub_concepts/Multi-Level_IR_Architecture]]
