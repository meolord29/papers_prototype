---
title: "Compiler Support Variability"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Compiler Support Variability

[[../Dynamic_Shape|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Different deep learning compilers exhibit varying levels of dynamic shape support across the ecosystem.== This variability creates challenges for practitioners who need to select appropriate compilers for their specific model requirements. ==Some compilers like TVM, nGraph, and XLA explicitly support dynamic shapes, while others like TC and Glow do not.== This inconsistency affects model portability and deployment decisions across different hardware targets. Understanding which compilers support dynamic shapes is critical for selecting the right toolchain for dynamic models.

## Usage in this paper

==The paper uses compiler support variability to categorize and compare existing DL compilers in Table 1.== This comparison helps practitioners understand which compilers can handle dynamic models versus static-only models. The variability analysis informs the recommendation that dynamic shape support is a key differentiator when selecting compilers for NLP and other dynamic workloads.

## References

> [!quote] Section 7 (p. 15)
> "Table 1 shows varying support across compilers: TVM, nGraph, and XLA support it while TC and Glow do not."
> *Discussion of dynamic shape support across different DL compilers in the taxonomy table*





## Backlinks

- [[../Dynamic_Shape]]
