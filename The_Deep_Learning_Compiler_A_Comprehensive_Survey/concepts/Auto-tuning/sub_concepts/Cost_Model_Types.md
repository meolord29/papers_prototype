---
title: "Cost Model Types"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Cost Model Types

[[../Auto-tuning|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Cost models are predictive mechanisms that estimate the performance of different parameter configurations without exhaustive execution. The paper discusses three primary types: black-box models that treat the system as opaque, ML-based models that learn from historical tuning data, and pre-defined models based on expert knowledge. ML-based cost models are particularly significant as they enable the system to learn and improve predictions as new configurations are explored during the tuning process. These models reduce the search space complexity by predicting which configurations are likely to perform well before actual execution. ==The choice of cost model directly impacts tuning efficiency and final performance outcomes.==

## Usage in this paper

In this paper, cost model types are analyzed as a key component of auto-tuning within the backend optimization framework. ==Section 4.4.2 compares different cost models across TVM, TC, and XLA compilers to demonstrate their relative effectiveness.== The paper emphasizes that ML-based approaches represent an advancement over traditional black-box methods for deep learning compiler optimization. This comparison helps practitioners understand which tuning strategies work best for different hardware targets.

## References

> [!quote] Section 1 (Contributions) (p. 2)
> "backend optimizations (including hardware-specific optimization, auto-tuning and optimized kernel libraries)"
> *Auto-tuning is identified as one of the key backend optimization components in DL compilers*

> [!quote] Section 1 (Future Directions) (p. 3)
> "advanced auto-tuning"
> *Advanced auto-tuning is highlighted as a future research direction for DL compiler development*





## Backlinks

- [[../Auto-tuning]]
