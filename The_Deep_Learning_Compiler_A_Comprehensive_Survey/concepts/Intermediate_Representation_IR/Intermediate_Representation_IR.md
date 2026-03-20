---
title: "Intermediate Representation (IR)"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 9
---

# Intermediate Representation (IR)

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Intermediate Representation is an abstraction of the program used for program optimizations in compilers.== ==In DL compilers, IR serves as the bridge between high-level model definitions and low-level hardware-specific code.== The IR design significantly impacts the expressiveness of computation graphs and determines how compilers analyze and optimize the model. A well-designed IR captures computation dependencies, control flow, and semantic information while providing extensibility for customized operators.

## Usage in this paper

==The paper emphasizes that the uniqueness of DL compilers lies in the design of multi-level IRs.== High-level IR (graph IR) resides in the frontend for hardware-independent optimizations, while low-level IR resides in the backend for hardware-specific optimizations. Different compilers implement IR differently: TVM uses Relay/Halide, nGraph uses nGraph IR, XLA uses HLO for both levels.

## References

> [!quote] Section 3 (p. 7)
> "Generally, IR is an abstraction of the program and is used for program optimizations. Specifically, the DL models are translated into multi-level IRs in DL compilers."
> *Explains the role of IR in DL compiler architecture*



## Sub-Concepts

- [[sub_concepts/Multi-level_IR_Architecture|Multi-level IR Architecture]]
- [[sub_concepts/IR_Implementation_Variations_Across_Compilers|IR Implementation Variations Across Compilers]]
- [[sub_concepts/IR_Role_in_Frontend_and_Backend_Optimizations|IR Role in Frontend and Backend Optimizations]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Multi-level_IR_Architecture]]
- [[sub_concepts/IR_Implementation_Variations_Across_Compilers]]
- [[sub_concepts/IR_Role_in_Frontend_and_Backend_Optimizations]]
