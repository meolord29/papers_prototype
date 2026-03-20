---
title: "Placeholder-based Support"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Placeholder-based Support

[[../../Dynamic_Shape|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Placeholder-based Support represents the technical approach compilers use to handle unknown dimension sizes during compilation. ==Compilers like TVM and XLA have implemented mechanisms using placeholders to represent dimensions that will be determined at runtime.== This approach allows the compilation process to proceed without concrete dimension values while still enabling optimization. The placeholder system must maintain flexibility while not sacrificing too much performance compared to fully static compilation. ==This technique indicates a shift towards more flexible compilation strategies in the DL compiler community.==

## Usage in this paper

The paper discusses Placeholder-based Support as an emerging solution that some compilers have already started implementing. ==TVM and XLA are specifically mentioned as examples of compilers that have begun supporting unknown dimension sizes using this approach.== This demonstrates that the DL compiler community is actively working on solutions for dynamic shape challenges. The survey uses these examples to show the current state of the art and direction of development in the field.

## References

> [!quote] Parent Concept Description (p. 1)
> "Some compilers like TVM and XLA have started to support unknown dimension sizes using placeholders"
> *Describes current compiler support for dynamic shapes using placeholder mechanisms*



## Sub-Concepts

The concept of Placeholder-based Support unfolds across three interconnected dimensions in DL compiler design. **Runtime Dimension Abstraction** establishes the foundation by allowing compilers to proceed without concrete dimension values during the compilation phase. This directly enables **Compiler Flexibility Mechanisms** which maintain optimization capabilities while accommodating unknown shapes. Finally, understanding both reveals why **Dynamic Shape Integration** is critical for bridging the gap between static compilation benefits and runtime flexibility needs in modern DL workloads.

- [[sub_concepts/Runtime_Dimension_Abstraction/Runtime_Dimension_Abstraction|Runtime Dimension Abstraction]]
- [[sub_concepts/Compiler_Flexibility_Mechanisms/Compiler_Flexibility_Mechanisms|Compiler Flexibility Mechanisms]]
- [[sub_concepts/Dynamic_Shape_Integration/Dynamic_Shape_Integration|Dynamic Shape Integration]]


## Backlinks

- [[../../Dynamic_Shape]]
- [[sub_concepts/Runtime_Dimension_Abstraction/Runtime_Dimension_Abstraction]]
- [[sub_concepts/Compiler_Flexibility_Mechanisms/Compiler_Flexibility_Mechanisms]]
- [[sub_concepts/Dynamic_Shape_Integration/Dynamic_Shape_Integration]]
