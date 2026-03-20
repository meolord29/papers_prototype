---
title: "Dynamic Shape"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 9
---

# Dynamic Shape

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Dynamic shape refers to the capability of DL compilers to handle tensors with unknown dimension sizes at compile time.== ==This is increasingly important as dynamic models become more popular, especially in NLP where input shapes may change during execution.== Supporting dynamic shapes requires relaxed bound inference, dimension checking, and extra mechanisms to guarantee memory validity. Current compilers use different approaches: TVM uses Any, XLA uses None, and nGraph uses PartialShape class.

## Usage in this paper

==The paper identifies dynamic shape support as a key future research direction in Section 7.== Table 1 shows varying support across compilers: TVM, nGraph, and XLA support it while TC and Glow do not. The evaluation reveals compatibility problems when nGraph encounters tensors with dynamic shapes, failing to run several models.

## References

> [!quote] Section 7 (p. 27)
> "Dynamic model becomes more and more popular in the field of DL, whose input shape or even model itself may change during execution."
> *Highlights the growing importance of dynamic shape support*



## Sub-Concepts

- [[sub_concepts/Compiler_Support_Variability|Compiler Support Variability]]
- [[sub_concepts/Runtime_Dimension_Handling|Runtime Dimension Handling]]
- [[sub_concepts/Memory_Validity_Guarantees|Memory Validity Guarantees]]
- [[sub_concepts/Model_Compatibility_Issues|Model Compatibility Issues]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Compiler_Support_Variability]]
- [[sub_concepts/Runtime_Dimension_Handling]]
- [[sub_concepts/Memory_Validity_Guarantees]]
- [[sub_concepts/Model_Compatibility_Issues]]
