---
title: "Differentiable Programming Extension"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 9
---

# Differentiable Programming Extension

[[../../Auto-Differentiation_Compiler_Support|← Parent]]

> [!info] Concept (Level 3)
> Differentiable programming extension represents the evolution of DL compilers from optimizing fixed neural architectures to supporting general learnable algorithms across diverse computational domains. ==This capability requires the compiler infrastructure to support automatic differentiation across general computations beyond traditional neural network operations.== The extension enables programmers to write arbitrary differentiable code that the compiler can optimize and deploy efficiently on various hardware targets. ==This paradigm shift moves beyond framework-specific models to general-purpose differentiable program compilation.== Supporting this extension opens new application areas including scientific computing, physics simulation, and optimization problems that require gradient-based methods.

## Usage in this paper

==The paper explicitly identifies differentiable programming as one of the key future research directions for DL compiler development.== The authors note that current compilers like TVM and XLA focus on optimizing predefined neural network operations rather than general differentiable code. Supporting this extension would represent a significant evolution in the DL compiler paradigm. The paper positions this as an important insight for boosting research in the DL compiler community toward more general differentiable program support.

## References

> [!quote] Section 1 (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection, which we hope to boost the research in the DL compiler community."
> *Explicitly lists differentiable programming as a future research direction for DL compilers*

> [!quote] Section 1 (p. 1)
> "This is the first survey paper focusing on the design architecture of DL compilers, which we hope can pave the road for future research towards DL compiler."
> *Establishes the paper's goal of guiding future DL compiler research directions*





## Backlinks

- [[../../Auto-Differentiation_Compiler_Support]]
