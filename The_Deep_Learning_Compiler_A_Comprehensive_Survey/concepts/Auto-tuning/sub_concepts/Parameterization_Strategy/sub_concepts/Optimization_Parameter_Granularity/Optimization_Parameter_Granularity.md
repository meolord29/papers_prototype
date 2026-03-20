---
title: "Optimization Parameter Granularity"
date: 2026-03-20
tags: ["concept", "depth-3"]
depth_level: 3
weight: 7
---

# Optimization Parameter Granularity

[[../../Parameterization_Strategy|← Parent]] → [[../../../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 3)
> Optimization Parameter Granularity addresses the balance between expressiveness and search space size in the parameterization strategy. Fine-grained parameters provide more optimization opportunities but exponentially increase the search space complexity. Coarse-grained parameters reduce search complexity but may miss optimal configurations for specific hardware-model combinations. ==A well-designed parameterization strategy ensures that optimal configurations are reachable while keeping the search tractable.== ==The granularity choice directly affects auto-tuning efficiency and the quality of generated code across different DL compilers.==

## Usage in this paper

The paper identifies parameterization as working in conjunction with the cost model to define what configurations can be tuned within DL compilers. Optimization Parameter Granularity is critical for enabling sophisticated search techniques to discover high-performance configurations. The paper highlights advanced auto-tuning as a future research direction, implying current granularity approaches need improvement. This aspect is essential for supporting diverse DL models across various hardware architectures efficiently.

## References

> [!quote] Section 1 (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning"
> *Discussion of future research directions including advanced auto-tuning*





## Backlinks

- [[../../Parameterization_Strategy]]
