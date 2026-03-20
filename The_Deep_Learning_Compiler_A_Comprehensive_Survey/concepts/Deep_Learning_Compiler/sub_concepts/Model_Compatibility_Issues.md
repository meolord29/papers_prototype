---
title: "Model Compatibility Issues"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Model Compatibility Issues

[[../Dynamic_Shape|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==Model compatibility issues arise when DL compilers encounter tensors with dynamic shapes that they cannot properly handle.== ==The evaluation in the paper reveals compatibility problems when nGraph encounters tensors with dynamic shapes, failing to run several models.== These failures demonstrate the practical limitations of current dynamic shape implementations. Compatibility issues can prevent certain models from being deployed on specific compiler-hardware combinations. Addressing these issues is crucial for achieving broader model portability across the DL ecosystem.

## Usage in this paper

The paper uses compatibility issues as evidence for why dynamic shape support needs improvement. ==The evaluation section demonstrates concrete failures when dynamic shapes are not properly supported.== This empirical evidence supports the claim that dynamic shape handling is a critical area for future research and development.

## References

> [!quote] Section 6 (p. 14)
> "The evaluation reveals compatibility problems when nGraph encounters tensors with dynamic shapes, failing to run several models."
> *Performance evaluation section showing practical limitations of current compiler support*





## Backlinks

- [[../Dynamic_Shape]]
