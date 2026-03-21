---
title: "Differentiable Programming"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 1
weight: 9
---

# Differentiable Programming



> [!info] Concept (Level 1)
> ==Differentiable programming is a paradigm where programs are thoroughly differentiable, allowing for automatic differentiation of algorithms.== This is attractive for the DL community as it extends beyond standard neural networks to more general computations. Supporting this in compilers is challenging due to differences in data structures and language semantics. It requires significant changes to compiler designs to handle control flow and operation abstraction. ==Embracing this paradigm opens up new research opportunities for high-order auto differentiation.==

## Usage in this paper

==The paper highlights differentiable programming as a future direction with little current support in DL compilers.== It notes difficulties in transforming imperative languages like Julia to symbolic IRs like XLA HLO. The authors suggest that expanding compiler capability to support this would open large research opportunities. This concept represents the cutting edge of what DL compilers might evolve to support.

## References

> [!quote] Section 7 (p. 29)
> "Unfortunately, there is little support for differential programming in existing DL compilers."
> *Noting the current lack of support.*



## Sub-Concepts

The concept of Differentiable Programming unfolds across three interconnected dimensions within DL compiler design. **Imperative-to-Symbolic IR Transformation** establishes the foundational challenge by addressing how imperative language constructs must be converted to symbolic intermediate representations. This directly enables **Control Flow and Operation Abstraction** which handles the complex semantics required for differentiation through program structures. Finally, understanding both reveals why **Auto-Differentiation Compiler Support** is critical for enabling high-order differentiation capabilities that extend beyond standard neural networks.

- [[sub_concepts/Imperative-to-Symbolic_IR_Transformation/Imperative-to-Symbolic_IR_Transformation|Imperative-to-Symbolic IR Transformation]]
- [[sub_concepts/Control_Flow_and_Operation_Abstraction/Control_Flow_and_Operation_Abstraction|Control Flow and Operation Abstraction]]
- [[sub_concepts/Auto-Differentiation_Compiler_Support/Auto-Differentiation_Compiler_Support|Auto-Differentiation Compiler Support]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Imperative-to-Symbolic_IR_Transformation/Imperative-to-Symbolic_IR_Transformation]]
- [[sub_concepts/Control_Flow_and_Operation_Abstraction/Control_Flow_and_Operation_Abstraction]]
- [[sub_concepts/Auto-Differentiation_Compiler_Support/Auto-Differentiation_Compiler_Support]]
