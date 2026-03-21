---
title: "Compiler Taxonomy Classification"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 7
---

# Compiler Taxonomy Classification

[[../../Runtime_Dimension_Inference|← Parent]]

> [!info] Concept (Level 3)
> ==Compiler taxonomy classification organizes DL compilers based on their capabilities including runtime dimension inference support.== This classification helps practitioners select appropriate compilers for their specific requirements regarding dynamic shapes. The taxonomy distinguishes between compilers with full dynamic support versus those with static-only or limited capabilities. ==Such classification reveals gaps in current compiler ecosystems and guides future development priorities.== Understanding where each compiler falls in this taxonomy is essential for matching tools to model requirements.

## Usage in this paper

==The paper presents a comprehensive taxonomy of existing DL compilers as one of its main contributions.== This taxonomy covers various aspects including which compilers support dynamic dimensions versus static-only compilation. Compilers like TVM and XLA are noted as having more advanced capabilities compared to TC and Glow. The taxonomy serves as guidelines for practitioners selecting compilers based on their dynamic shape requirements.

## References

> [!quote] Section 1 (Contributions) (p. 2)
> "We provide a comprehensive taxonomy of existing DL compilers from various aspects, which corresponds to the key components described in this survey."
> *Description of the taxonomy contribution covering compiler capabilities*

> [!quote] Section 1 (p. 2)
> "Several popular DL compilers have been proposed such as TVM, Tensor Comprehension, Glow, nGraph and XLA, from both industry and academia."
> *List of DL compilers that are categorized in the taxonomy*





## Backlinks

- [[../../Runtime_Dimension_Inference]]
