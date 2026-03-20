---
title: "Automatic Differentiation Capability"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Automatic Differentiation Capability

[[../Differentiable_Programming|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Differentiable programming is a paradigm where programs are thoroughly differentiable, enabling automatic differentiation of algorithms.== This paradigm is attractive for the DL community as it allows gradient-based optimization of arbitrary programs. It moves beyond static graphs to allow dynamic computation structures to be optimized via gradients. Many compiler projects have adopted differentiable programming including Myia, Flux, and Julia. ==However, existing DL compilers provide little support for differentiable programming, presenting significant research opportunities.==

## Usage in this paper

==In this paper, this capability is identified as a future research direction in Section 7.== The authors note the challenge of supporting it in existing DL compilers due to current limitations. This gap highlights the need for new compiler architectures that can handle gradient computation natively.

## References

> [!quote] Section 1 (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection, which we hope to boost the research in the DL compiler community."
> *This quote from the Introduction lists differentiable programming as a key future insight for DL compiler research.*





## Backlinks

- [[../Differentiable_Programming]]
