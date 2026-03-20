---
title: "Quantization"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 8
---

# Quantization

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Quantization is the process of reducing the precision of numerical representations in DL models to improve efficiency and reduce memory footprint.== Traditional quantization strategies use fixed schemes with little hardware customization, while DL compilers can leverage compilation-time optimization for more efficient strategies. ==Supporting quantization presents challenges including implementing new quantized operators without heavy engineering efforts and managing interaction with other optimizations.== Relay provides quantization rewriting flow that automatically generates quantized code for various schemes.

## Usage in this paper

==Table 1 shows quantization support varies: TVM (int8/fp16), nGraph (int8 with training), Glow (int8), XLA (int8/int16), while TC lacks support.== Section 7 identifies quantization as a future research direction, discussing challenges in operator implementation and optimization interaction. The paper suggests using dialects to implement quantized operators upon basic operators.

## References

> [!quote] Section 7 (p. 28)
> "Whereas, supporting quantization in DL compilers can leverage optimization opportunities during compilation to derive more efficient quantization strategies."
> *Explains the advantage of compiler-based quantization*



## Sub-Concepts

- [[sub_concepts/Quantization_Precision_Support|Quantization Precision Support]]
- [[sub_concepts/Quantized_Operator_Implementation|Quantized Operator Implementation]]
- [[sub_concepts/Quantization_Optimization_Interaction|Quantization Optimization Interaction]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Quantization_Precision_Support]]
- [[sub_concepts/Quantized_Operator_Implementation]]
- [[sub_concepts/Quantization_Optimization_Interaction]]
