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
> ==Auto-tuning is a technique used to automatically determine optimal parameter configurations in the enormous search space of hardware-specific optimizations.== It typically includes four key components: parameterization (defining data and target parameters), cost model (predicting performance), searching technique (genetic algorithm, simulated annealing, reinforcement learning), and acceleration methods. Auto-tuning is essential for exploiting the full potential of complex hardware like GPUs where manual tuning is impractical. ==ML-based cost models enable the system to learn and improve predictions as new configurations are explored.==

## Usage in this paper

Section 4.4.2 provides detailed analysis of auto-tuning across TVM, TC, and XLA. The paper compares different cost models (black-box, ML-based, pre-defined) and searching techniques (GA, SA, RL). ==Performance evaluation shows tuned TVM achieves 41.26× speedup on GPU compared to untuned version, demonstrating auto-tuning's critical importance.==

## References

> [!quote] Section 4.4.2 (p. 19)
> "Due to the enormous search space for parameter tuning in hardware-specific optimizations, it is necessary to leverage auto-tuning to determine the optimal parameter configurations."
> *Explains why auto-tuning is necessary*



## Sub-Concepts

- [[sub_concepts/Cost_Model_Types|Cost Model Types]]
- [[sub_concepts/Search_Techniques|Search Techniques]]
- [[sub_concepts/Hardware-Specific_Parameter_Optimization|Hardware-Specific Parameter Optimization]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Cost_Model_Types]]
- [[sub_concepts/Search_Techniques]]
- [[sub_concepts/Hardware-Specific_Parameter_Optimization]]
