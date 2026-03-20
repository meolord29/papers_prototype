---
title: "Searching Technique"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Searching Technique

[[../../Auto-tuning|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Searching technique refers to the algorithmic approach used to explore the parameter space and identify optimal configurations. ==Given the enormous search space for parameter tuning in hardware-specific optimizations, efficient search strategies are necessary to find the best settings without exhaustive enumeration.== Common techniques include genetic algorithms, simulated annealing, Bayesian optimization, and reinforcement learning-based approaches. The search technique must balance exploration of new configurations with exploitation of known good regions. ==The effectiveness of the searching technique directly determines whether auto-tuning can discover high-performance configurations within reasonable time constraints.==

## Usage in this paper

The paper positions searching technique as a critical component of the auto-tuning process in DL compilers. It is mentioned alongside cost model and parameterization as part of the four key components. ==The paper emphasizes that due to the enormous search space for parameter tuning, it is necessary to leverage auto-tuning with appropriate searching techniques to find optimal configurations for diverse hardware.==

## References

> [!quote] Section 4 (Backend Optimizations) (p. 3)
> "Due to the enormous search space for parameter tuning in hardware-specific optimizations, it is necessary to leverage auto-tuning to find the best settings."
> *Rationale for auto-tuning and search techniques*



## Sub-Concepts

The concept of Searching Technique in DL compilers unfolds across three interconnected dimensions that collectively enable effective auto-tuning. **Auto-tuning Strategy** establishes the foundational approach by defining how the compiler systematically explores configuration options to find optimal performance. This directly enables **Hardware-Specific Search** which adapts the search process to account for the unique characteristics of diverse DL accelerators and their architectural constraints. Finally, understanding both reveals why **Parameter Space Reduction** is critical, as it narrows the enormous search space to make the auto-tuning process computationally feasible within reasonable time constraints. Together, these sub-concepts form a cohesive framework where the strategy determines the method, hardware-specificity ensures relevance, and space reduction guarantees practicality.

- [[sub_concepts/Auto-tuning_Strategy/Auto-tuning_Strategy|Auto-tuning Strategy]]
- [[sub_concepts/Hardware-Specific_Search/Hardware-Specific_Search|Hardware-Specific Search]]
- [[sub_concepts/Parameter_Space_Reduction/Parameter_Space_Reduction|Parameter Space Reduction]]


## Backlinks

- [[../../Auto-tuning]]
- [[sub_concepts/Auto-tuning_Strategy/Auto-tuning_Strategy]]
- [[sub_concepts/Hardware-Specific_Search/Hardware-Specific_Search]]
- [[sub_concepts/Parameter_Space_Reduction/Parameter_Space_Reduction]]
