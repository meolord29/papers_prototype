---
title: "Dynamic Shape"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 1
weight: 9
---

# Dynamic Shape



> [!info] Concept (Level 1)
> ==Dynamic shape refers to the capability of a compiler to handle tensor dimensions that are not known until runtime.== This feature is essential for models with variable input sizes, common in NLP and reinforcement learning. Supporting dynamic shapes requires relaxing bound inference and dimension checking during compilation. It adds complexity to memory planning and optimization passes which often rely on static information. ==As models become more flexible, robust dynamic shape support becomes a critical requirement.==

## Usage in this paper

==The paper identifies dynamic shape support as a key differentiator in the taxonomy of DL compilers.== It notes that while TVM and XLA support it, others like TC and Glow have limitations. The conclusion highlights dynamic shape as a future research direction due to its popularity in emerging models. This concept underscores a current limitation and future opportunity in compiler design.

## References

> [!quote] Section 7 (p. 27)
> "Existing DL compilers require more research efforts to support dynamic shape efficiently for emerging dynamic models."
> *Calling for future research on dynamic shapes.*



## Sub-Concepts

The concept of Dynamic Shape unfolds across three interconnected dimensions that define compiler capability. **Runtime Dimension Inference** establishes the foundational challenge by addressing how compilers handle tensor dimensions unknown until execution time. This directly constrains **Memory Planning for Variable Tensors** which must allocate resources without complete static information, creating a dependency between inference and allocation strategies. Finally, understanding both reveals why **Optimization Pass Adaptation** is critical, as traditional optimization passes relying on static bounds must be redesigned to work with dynamic constraints. Together, these sub-concepts form a cascade where each limitation propagates to the next, explaining why dynamic shape support remains a key differentiator among DL compilers.

- [[sub_concepts/Runtime_Dimension_Inference/Runtime_Dimension_Inference|Runtime Dimension Inference]]
- [[sub_concepts/Memory_Planning_for_Variable_Tensors/Memory_Planning_for_Variable_Tensors|Memory Planning for Variable Tensors]]
- [[sub_concepts/Optimization_Pass_Adaptation/Optimization_Pass_Adaptation|Optimization Pass Adaptation]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Runtime_Dimension_Inference/Runtime_Dimension_Inference]]
- [[sub_concepts/Memory_Planning_for_Variable_Tensors/Memory_Planning_for_Variable_Tensors]]
- [[sub_concepts/Optimization_Pass_Adaptation/Optimization_Pass_Adaptation]]
