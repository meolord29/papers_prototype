---
title: "Operator Fusion"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 9
---

# Operator Fusion

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Operator fusion is an indispensable optimization that combines multiple operators into a single kernel to improve efficiency.== ==It enables better sharing of computation, eliminates intermediate memory allocations, facilitates further optimization by combining loop nests, and reduces launch and synchronization overhead.== Different compilers implement fusion differently: TVM classifies operators into categories with fusion rules, TC uses polyhedral transformations, and Glow applies operator stacking. Identifying and fusing complicated graph patterns remains an active research challenge.

## Usage in this paper

==The paper discusses operator fusion in Section 4.3.2 as a key block-level optimization.== TVM's approach classifies operators into injective, reduction, complex-out-fusible, and opaque categories with corresponding fusion rules. Recent works are exploring aggressive fusion plans for blocks with multiple broadcast and reduce nodes.

## References

> [!quote] Section 4.3.2 (p. 15)
> "Operator fusion is indispensable optimization of DL compilers. It enables better sharing of computation, eliminates intermediate allocations, facilitates further optimization by combining loop nests."
> *Explains the benefits of operator fusion*



## Sub-Concepts

- [[sub_concepts/Intermediate_Memory_Elimination|Intermediate Memory Elimination]]
- [[sub_concepts/Kernel_Launch_and_Synchronization_Overhead_Reducti|Kernel Launch and Synchronization Overhead Reduction]]
- [[sub_concepts/Survey_Taxonomy_of_Fusion_Approaches|Survey Taxonomy of Fusion Approaches]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Intermediate_Memory_Elimination]]
- [[sub_concepts/Kernel_Launch_and_Synchronization_Overhead_Reducti]]
- [[sub_concepts/Survey_Taxonomy_of_Fusion_Approaches]]
