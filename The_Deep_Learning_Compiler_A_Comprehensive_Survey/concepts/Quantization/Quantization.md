---
title: "Quantization"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 5
---

# Quantization

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Quantization is a technique that reduces the precision of numbers used in neural network computations to save memory and increase speed.== Traditional quantization strategies applied in DL frameworks are based on a set of fixed schemes and datatypes with little customization. ==Whereas, supporting quantization in DL compilers can leverage optimization opportunities during compilation to derive more efficient quantization strategies.== This allows for hardware-specific precision tuning like INT8 or FP16. ==It is vital for deploying models on resource-constrained edge devices.==

## Usage in this paper

The paper discusses quantization as a future direction where compilers can automate the insertion of quantized operators. ==For example, Relay provides a quantization rewriting flow that can automatically generate quantized code for various schemes.== To support quantization, there are several challenges to be solved in DL compilers regarding operator implementation. This highlights the complexity of integrating quantization into the compilation flow.

## References

> [!quote] Section 7 (p. 28)
> "Whereas, supporting quantization in DL compilers can leverage optimization opportunities during compilation to derive more efficient quantization strategies."
> *Explains the advantage of compiler-supported quantization.*





## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
