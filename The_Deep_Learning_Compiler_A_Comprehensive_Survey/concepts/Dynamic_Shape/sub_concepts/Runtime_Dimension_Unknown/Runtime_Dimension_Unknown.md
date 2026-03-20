---
title: "Runtime Dimension Unknown"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Runtime Dimension Unknown

[[../../Dynamic_Shape|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Runtime Dimension Unknown refers to the core characteristic where input tensor dimensions are not known until the model actually executes.== ==This creates a fundamental challenge for compilers that traditionally rely on static analysis during compilation time.== The uncertainty means optimization decisions cannot be fully made ahead of execution, requiring more flexible compilation strategies. This aspect is particularly problematic for performance-critical applications where compile-time optimizations provide significant speedups. The inability to know dimensions upfront forces compilers to generate more generic code that can handle multiple possible shapes.

## Usage in this paper

In this paper, Runtime Dimension Unknown is presented as the foundational challenge that defines the dynamic shape problem space. ==The survey identifies this as a key reason why existing DL compilers require more research efforts to support dynamic models efficiently.== This concept frames the entire discussion around why dynamic shape support remains a significant challenge for static compilation graphs. The paper uses this to motivate future research directions in DL compiler development.

## References

> [!quote] Section 1 (Introduction) (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection"
> *Dynamic shape is listed as a key future research direction for DL compilers*



## Sub-Concepts

The concept of Runtime Dimension Unknown unfolds across three interconnected dimensions that define the dynamic shape challenge in DL compilers. **Dynamic Shape Support** establishes the foundational requirement by identifying why runtime dimension uncertainty creates compilation challenges. This directly enables **Multi-level IR Design** which provides the architectural flexibility needed to handle variable tensor shapes during execution. Finally, understanding both reveals why **Compilation-Time Optimization Limitations** is critical, as static analysis cannot fully optimize code when dimensions remain unknown until runtime, forcing compilers to adopt more flexible strategies.

- [[sub_concepts/Dynamic_Shape_Support/Dynamic_Shape_Support|Dynamic Shape Support]]
- [[sub_concepts/Multi-level_IR_Design/Multi-level_IR_Design|Multi-level IR Design]]
- [[sub_concepts/Compilation-Time_Optimization_Limitations/Compilation-Time_Optimization_Limitations|Compilation-Time Optimization Limitations]]


## Backlinks

- [[../../Dynamic_Shape]]
- [[sub_concepts/Dynamic_Shape_Support/Dynamic_Shape_Support]]
- [[sub_concepts/Multi-level_IR_Design/Multi-level_IR_Design]]
- [[sub_concepts/Compilation-Time_Optimization_Limitations/Compilation-Time_Optimization_Limitations]]
