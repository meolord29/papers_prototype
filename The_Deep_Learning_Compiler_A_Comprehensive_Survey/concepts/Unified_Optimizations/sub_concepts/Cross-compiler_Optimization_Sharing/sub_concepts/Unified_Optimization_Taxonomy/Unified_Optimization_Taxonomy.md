---
title: "Unified Optimization Taxonomy"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 7
---

# Unified Optimization Taxonomy

[[../../Cross-compiler_Optimization_Sharing|← Parent]]

> [!info] Concept (Level 3)
> ==Unified Optimization Taxonomy refers to the comprehensive categorization and documentation of optimization techniques across different DL compilers in a standardized framework.== This taxonomy organizes optimizations by their application level (frontend, IR-level, backend) and by their transformation type (operator fusion, memory optimization, kernel optimization). By creating a common vocabulary and classification system, the taxonomy enables compiler developers to identify equivalent or similar optimizations across different compiler implementations. The taxonomy serves as a reference guide that reduces the learning curve for understanding optimization techniques developed in other compilers. ==This systematic documentation is essential for cross-compiler sharing because it makes optimization knowledge discoverable and comparable.== Without such taxonomy, optimization techniques remain siloed within individual compiler projects, preventing community-wide advancement.

## Usage in this paper

The paper provides a comprehensive taxonomy of existing DL compilers from various aspects corresponding to key components described in the survey. This taxonomy aims to provide guidelines about compiler selection for practitioners and give thorough summary for researchers. The survey documents existing optimization techniques comprehensively to facilitate sharing by making them visible and comparable across compilers. This contributes to the parent concept by creating the knowledge infrastructure needed for optimization techniques to be shared and reused across the community.

## References

> [!quote] Section 5 (p. 2)
> "We provide a comprehensive taxonomy of existing DL compilers from various aspects, which corresponds to the key components described in this survey. The target of this taxonomy is to provide guidelines about the selection of DL compilers for the practitioners considering their requirements, as well as to give a thorough summary of the DL compilers for researchers."
> *Describing the taxonomy contribution of the paper*

> [!quote] Section 4 (p. 2)
> "We present detailed analysis on the design of multi-level IRs and illustrate the commonly adopted optimization techniques."
> *Explaining how the paper documents optimization techniques*





## Backlinks

- [[../../Cross-compiler_Optimization_Sharing]]
