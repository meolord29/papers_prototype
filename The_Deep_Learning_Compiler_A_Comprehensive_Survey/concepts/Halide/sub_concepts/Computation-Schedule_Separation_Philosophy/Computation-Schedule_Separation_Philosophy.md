---
title: "Computation-Schedule Separation Philosophy"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Computation-Schedule Separation Philosophy

[[../../Halide|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Computation-Schedule Separation Philosophy embodies Halide's fundamental design principle that decouples algorithm definition from execution optimization.== ==Rather than prescribing a specific scheduling scheme directly, this philosophy allows compilers to explore various possible schedules and autonomously select the optimal one.== This separation enables flexible optimization of memory references and loop nests without constraining the computational logic. The approach has proven extensible and efficient in DL compilers, enabling adaptation to diverse hardware architectures. This philosophy represents a paradigm shift from traditional compilers where scheduling decisions are often hardcoded into the compilation process.

## Usage in this paper

The paper leverages this philosophy to explain why Halide-based compilers demonstrate superior optimization capabilities across diverse DL hardware targets. This separation principle is cited as the reason Halide's approach has proven extensible and efficient in modern DL compilers like TVM. ==The survey uses this concept to contrast Halide-based approaches with fixed-scheduling alternatives, highlighting the flexibility advantages.== Understanding this philosophy helps explain the design choices behind multi-level IR implementations in the surveyed compilers.

## References

> [!quote] Section 4 (p. 4)
> "The fundamental philosophy of Halide is the separation of computation and schedule. Rather than giving a specific scheme directly, the compilers adopting Halide try various possible schedules and choose the best one."
> *This quote explains the core design principle that makes Halide influential in DL compiler architecture*



## Sub-Concepts

The Computation-Schedule Separation Philosophy unfolds across three interconnected dimensions within DL compiler design. **Multi-level IR Architecture** establishes the foundation by creating distinct abstraction layers that separate computational semantics from scheduling decisions. This architectural separation directly enables **Auto-tuning Framework** which can explore various scheduling possibilities without constraining the underlying algorithmic logic. Finally, understanding both reveals why **Hardware-specific Optimization** is critical, as it allows the separated schedule to adapt efficiently across diverse DL hardware architectures. Together, these sub-concepts demonstrate how the philosophy transforms traditional compilation into a flexible, hardware-aware optimization process.

- [[sub_concepts/Multi-level_IR_Architecture/Multi-level_IR_Architecture|Multi-level IR Architecture]]
- [[sub_concepts/Auto-tuning_Framework/Auto-tuning_Framework|Auto-tuning Framework]]
- [[sub_concepts/Hardware-specific_Optimization/Hardware-specific_Optimization|Hardware-specific Optimization]]


## Backlinks

- [[../../Halide]]
- [[sub_concepts/Multi-level_IR_Architecture/Multi-level_IR_Architecture]]
- [[sub_concepts/Auto-tuning_Framework/Auto-tuning_Framework]]
- [[sub_concepts/Hardware-specific_Optimization/Hardware-specific_Optimization]]
