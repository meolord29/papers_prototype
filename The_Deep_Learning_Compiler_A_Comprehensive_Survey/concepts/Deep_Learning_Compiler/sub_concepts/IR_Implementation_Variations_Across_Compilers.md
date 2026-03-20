---
title: "IR Implementation Variations Across Compilers"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# IR Implementation Variations Across Compilers

[[../Intermediate_Representation_IR|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Different DL compilers implement Intermediate Representation using distinct approaches and naming conventions tailored to their design goals. ==TVM employs Relay for high-level representation and Halide for low-level code generation, providing flexibility across diverse hardware targets.== nGraph uses its own nGraph IR as a unified representation layer between frameworks and backends. ==XLA utilizes HLO (High-Level Optimizer) for both high-level and low-level optimization stages.== These variations reflect different trade-offs in expressiveness, optimization capabilities, and hardware support that each compiler prioritizes.

## Usage in this paper

The paper uses these IR implementation variations to build a comprehensive taxonomy of existing DL compilers from various aspects. ==By comparing different IR implementations, the authors provide guidelines about the selection of DL compilers for practitioners considering their requirements.== This comparison helps researchers understand the thorough summary of DL compilers and their design choices. The variations are analyzed to illustrate how different compilers address the challenge of mapping computation to diverse DL hardware efficiently.

## References

> [!quote] Section 1 (p. 2)
> "Several popular DL compilers have been proposed such as TVM, Tensor Comprehension, Glow, nGraph and XLA, from both industry and academia."
> *Introduction listing the DL compilers surveyed in the paper*

> [!quote] Section 1 (p. 3)
> "We provide a comprehensive taxonomy of existing DL compilers from various aspects, which corresponds to the key components described in this survey."
> *Paper contributions describing the taxonomy based on compiler components including IR*





## Backlinks

- [[../Intermediate_Representation_IR]]
