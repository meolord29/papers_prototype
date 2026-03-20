---
title: "Auto-tuning"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 9
---

# Auto-tuning

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Auto-tuning is a technique used to automatically determine the optimal parameter configurations for compiler optimizations.== ==Due to the enormous search space for parameter tuning in hardware-specific optimizations, it is necessary to leverage auto-tuning to find the best settings.== It typically involves a cost model, a searching technique, and a parameterization strategy. This process alleviates the manual efforts required to derive optimal configurations for diverse hardware. ==It is particularly crucial for maximizing performance on complex accelerators like GPUs.==

## Usage in this paper

==Among the studied DL compilers in this survey, TVM, TC, and XLA support the auto-tuning.== Generally, the auto-tuning implementation includes four key components, such as parameterization, cost model, searching technique, and acceleration. TVM adopts machine learning-based cost models to predict performance using statistical approaches. This allows the compiler to adapt to new hardware without extensive manual engineering.

## References

> [!quote] Section 4.4.2 (p. 19)
> "Due to the enormous search space for parameter tuning in hardware-specific optimizations, it is necessary to leverage auto-tuning to determine the optimal parameter configurations."
> *Explains the necessity of auto-tuning in modern compilers.*



## Sub-Concepts

The concept of Auto-tuning unfolds across four interconnected dimensions that work together to optimize deep learning compiler performance. **Cost Model** establishes the foundation by predicting performance outcomes using machine learning approaches, which directly informs how parameters should be evaluated. This enables **Parameterization Strategy** to define the search space of tunable configurations that the compiler can explore. **Searching Technique** then systematically navigates this parameterized space to find optimal solutions, while **Acceleration** mechanisms ensure the entire tuning process completes efficiently. Together, these components form a cohesive auto-tuning pipeline that adapts DL compilers to diverse hardware without manual intervention.

- [[sub_concepts/Cost_Model/Cost_Model|Cost Model]]
- [[sub_concepts/Parameterization_Strategy/Parameterization_Strategy|Parameterization Strategy]]
- [[sub_concepts/Searching_Technique/Searching_Technique|Searching Technique]]
- [[sub_concepts/Acceleration/Acceleration|Acceleration]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Cost_Model/Cost_Model]]
- [[sub_concepts/Parameterization_Strategy/Parameterization_Strategy]]
- [[sub_concepts/Searching_Technique/Searching_Technique]]
- [[sub_concepts/Acceleration/Acceleration]]
