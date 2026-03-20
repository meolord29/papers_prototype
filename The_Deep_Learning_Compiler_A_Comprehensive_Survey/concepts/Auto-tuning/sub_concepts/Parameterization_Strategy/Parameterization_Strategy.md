---
title: "Parameterization Strategy"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Parameterization Strategy

[[../../Auto-tuning|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Parameterization strategy defines how compiler optimizations are represented as tunable parameters within the auto-tuning framework. ==This involves identifying which aspects of code generation can be varied, such as loop unrolling factors, tile sizes, memory allocation strategies, and operator fusion decisions.== ==A well-designed parameterization strategy balances expressiveness with search space size, ensuring that optimal configurations are reachable while keeping the search tractable.== The strategy must capture hardware-specific characteristics to enable meaningful optimization choices. Without proper parameterization, even sophisticated search techniques cannot discover high-performance configurations for diverse DL hardware architectures.

## Usage in this paper

==The paper identifies parameterization as one of the four key components of auto-tuning implementation in DL compilers.== It works in conjunction with the cost model to define what configurations can be tuned. The paper notes that backend optimizations including auto-tuning are essential for mapping computations efficiently to diverse DL hardware, which requires careful parameterization of optimization choices.

## References

> [!quote] Section 4 (Backend Optimizations) (p. 3)
> "Generally, the auto-tuning implementation includes four key components, such as parameterization, cost model, searching technique, and acceleration."
> *Listing of auto-tuning components*

> [!quote] Section 1 (Introduction) (p. 2)
> "backend optimizations (including hardware-specific optimization, auto-tuning and optimized kernel libraries)"
> *Context of auto-tuning within backend optimizations*



## Sub-Concepts

The concept of Parameterization Strategy unfolds across three interconnected dimensions within DL compiler auto-tuning. **Search Space Definition** establishes the foundation by determining which optimization parameters can be varied during compilation. This directly enables **Hardware-Aware Parameter Selection** which ensures that the defined parameters capture hardware-specific characteristics for meaningful optimization choices. Finally, understanding both reveals why **Optimization Parameter Granularity** is critical for balancing expressiveness with search space size, ensuring optimal configurations remain reachable while keeping the search tractable across diverse DL hardware architectures.

- [[sub_concepts/Search_Space_Definition/Search_Space_Definition|Search Space Definition]]
- [[sub_concepts/Hardware-Aware_Parameter_Selection/Hardware-Aware_Parameter_Selection|Hardware-Aware Parameter Selection]]
- [[sub_concepts/Optimization_Parameter_Granularity/Optimization_Parameter_Granularity|Optimization Parameter Granularity]]


## Backlinks

- [[../../Auto-tuning]]
- [[sub_concepts/Search_Space_Definition/Search_Space_Definition]]
- [[sub_concepts/Hardware-Aware_Parameter_Selection/Hardware-Aware_Parameter_Selection]]
- [[sub_concepts/Optimization_Parameter_Granularity/Optimization_Parameter_Granularity]]
