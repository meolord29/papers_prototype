---
title: "Progressive Lowering Stages"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning", "abstraction-levels"]
depth_level: 3
weight: 9
---

# Progressive Lowering Stages

[[../../Multi-level_Intermediate_Representations|← Parent]]

> [!info] Concept (Level 3)
> Progressive lowering stages represent the hierarchical transformation process where models move through multiple IR levels during compilation. ==Each level captures different abstraction granularities, from high-level neural network operators down to low-level tensor operations.== ==This staged approach prevents premature loss of semantic information that would occur with single-level IR designs.== The multiple levels facilitate targeted optimizations specific to neural network structures at appropriate abstraction layers. This design is crucial for maintaining portability across diverse hardware architectures while enabling deep structural analysis throughout the compilation process.

## Usage in this paper

The paper highlights progressive lowering as a distinguishing feature that separates DL compilers from traditional compilers. ==The authors dissect this component to show how it enables different optimization strategies at different compilation stages.== This multi-level approach allows the compiler to apply framework-level optimizations before hardware-specific transformations. The survey emphasizes that IR design is critical for supporting the rapid evolution of DL models through these lowering stages.

## References

> [!quote] Section 1 (p. 2)
> "Similar to traditional compiler, DL compilers also adopt the layered design including frontend, intermediate representation (IR) and backend."
> *Describing the layered architecture of DL compilers*

> [!quote] Section 1 (p. 3)
> "We dissect the commonly adopted design architecture of existing DL compilers, and provide detailed analysis of the key design components such as multi-level IRs"
> *Outlining the paper's contributions regarding IR analysis*





## Backlinks

- [[../../Multi-level_Intermediate_Representations]]
