---
title: "Dynamic Shape Support"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 9
---

# Dynamic Shape Support

[[../../Runtime_Dimension_Inference|← Parent]]

> [!info] Concept (Level 3)
> ==Dynamic shape support refers to the compiler's ability to handle tensor dimensions that are not known until runtime execution.== This capability is essential for models with variable-length sequences, flexible batch sizes, or input-dependent computation graphs. Without dynamic shape support, compilers must either reject such models or resort to inefficient padding and static bounds. The support requires infrastructure to defer shape determination from compile-time optimization phases to runtime execution. ==This forms a critical differentiator between compilers designed for research flexibility versus production deployment.==

## Usage in this paper

==The paper identifies dynamic shape support as a key future research direction for DL compilers in the contributions section.== It positions this capability as essential for emerging models with flexible input requirements that cannot be predetermined. The survey highlights dynamic shape alongside other advanced features like auto-tuning and quantization as areas needing further development. This underscores the current limitation in many existing compilers.

## References

> [!quote] Section 1 (Contributions) (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection"
> *List of future research directions highlighting dynamic shape as a key area*





## Backlinks

- [[../../Runtime_Dimension_Inference]]
