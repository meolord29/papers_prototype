---
title: "Differentiable Programming"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 8
---

# Differentiable Programming

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Differentiable programming is a programming paradigm where programs are thoroughly differentiable, enabling automatic differentiation of algorithms.== This paradigm is attractive for the DL community as it allows gradient-based optimization of arbitrary programs. Many compiler projects have adopted differentiable programming including Myia, Flux, and Julia. ==However, existing DL compilers provide little support for differentiable programming, presenting significant research opportunities.==

## Usage in this paper

==Section 7 identifies differentiable programming as a future research direction, noting the challenge of supporting it in existing DL compilers.== Difficulties come from data structure and language semantic differences between imperative languages and symbolic IRs. The paper mentions that realizing transformation from Julia to XLA HLO IR requires addressing control flow and semantic differences.

## References

> [!quote] Section 7 (p. 29)
> "Differentiable programming is a programming paradigm, where the programs are differentiable thoroughly. Algorithms written in differentiable programming paradigm can be automatically differentiated."
> *Defines differentiable programming paradigm*



## Sub-Concepts

- [[sub_concepts/Automatic_Differentiation_Capability|Automatic Differentiation Capability]]
- [[sub_concepts/Imperative_to_Symbolic_IR_Transformation|Imperative to Symbolic IR Transformation]]
- [[sub_concepts/Control_Flow_and_Semantic_Differences|Control Flow and Semantic Differences]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Automatic_Differentiation_Capability]]
- [[sub_concepts/Imperative_to_Symbolic_IR_Transformation]]
- [[sub_concepts/Control_Flow_and_Semantic_Differences]]
