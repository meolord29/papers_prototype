---
title: "Cross-compiler Optimization Sharing"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 2
weight: 9
---

# Cross-compiler Optimization Sharing

[[../../Unified_Optimizations|← Parent]]

> [!info] Concept (Level 2)
> ==Cross-compiler Optimization Sharing represents the initiative to enable reuse of state-of-the-art optimization techniques across different DL compilers in the ecosystem.== Currently, each compiler has developed its own advantages and optimization strategies, but there is no standard mechanism for sharing these best practices. ==This sub-concept addresses the redundancy in compiler development efforts across the industry by creating pathways for knowledge transfer.== The goal is to accumulate optimization force so that advances in one compiler can benefit the entire DL compiler community. This sharing mechanism reduces the engineering burden on individual compiler teams and accelerates overall progress in the field.

## Usage in this paper

The paper advocates for unifying optimizations so that best practices from each compiler can be reused across the community. The authors point to MLIR as a promising initiative towards this direction with its flexible dialect system that enables cross-compiler compatibility. This concept frames the conclusion's vision for the future of the DL compiler community and is highlighted as a potential research direction. The survey aims to provide guidelines that facilitate this sharing by documenting existing optimization techniques comprehensively.

## References

> [!quote] Section 1 (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection"
> *Listing unified optimizations as a future research direction*

> [!quote] Section 1 (p. 2)
> "To provide interoperability, ONNX has been proposed, that defines a unified format for representing DL models to facilitate model conversion between different DL frameworks."
> *Discussing interoperability initiatives that enable optimization sharing*



## Sub-Concepts

The concept of Cross-compiler Optimization Sharing unfolds through three interconnected mechanisms that enable knowledge transfer across the DL compiler ecosystem. **Multi-level IR Architecture** establishes the foundational infrastructure by providing layered intermediate representations that different compilers can understand and transform. This directly enables **MLIR Dialect System** which offers flexible dialect definitions allowing compilers to express optimizations in a standardized yet extensible manner. Finally, **Unified Optimization Taxonomy** documents and categorizes existing optimization techniques comprehensively, making it possible for compiler developers to identify which best practices from one compiler can be adapted to another, completing the sharing pipeline from infrastructure to implementation to documentation.

- [[sub_concepts/Multi-level_IR_Architecture/Multi-level_IR_Architecture|Multi-level IR Architecture]]
- [[sub_concepts/MLIR_Dialect_System/MLIR_Dialect_System|MLIR Dialect System]]
- [[sub_concepts/Unified_Optimization_Taxonomy/Unified_Optimization_Taxonomy|Unified Optimization Taxonomy]]


## Backlinks

- [[../../Unified_Optimizations]]
- [[sub_concepts/Multi-level_IR_Architecture/Multi-level_IR_Architecture]]
- [[sub_concepts/MLIR_Dialect_System/MLIR_Dialect_System]]
- [[sub_concepts/Unified_Optimization_Taxonomy/Unified_Optimization_Taxonomy]]
