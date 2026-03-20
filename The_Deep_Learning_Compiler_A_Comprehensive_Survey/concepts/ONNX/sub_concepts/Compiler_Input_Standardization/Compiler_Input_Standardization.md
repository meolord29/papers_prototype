---
title: "Compiler Input Standardization"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 8
---

# Compiler Input Standardization

[[../../ONNX|← Parent]] → [[../../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> ==ONNX serves as a critical entry point for deep learning compilation pipelines in modern architectures.== Many compilers adopt ONNX as a primary input format to streamline their frontend processing stages. This standardization allows compiler developers to focus on optimization rather than parsing diverse framework APIs. ==It creates a unified interface between the training frameworks and the inference optimization tools.== Consequently, this reduces the complexity of maintaining multiple input adapters for the system.

## Usage in this paper

The survey identifies that DL compilers take model definitions described in DL frameworks as inputs. ==This makes ONNX a critical bridge in the compiler input pipeline as it standardizes these definitions.== It enables the compilers to handle models from frameworks not directly supported by building converters to ONNX first. Thus, the compiler backend can remain agnostic to the source framework details.

## References

> [!quote] Section 1 (p. 2)
> "The DL compilers take the model definitions described in the DL frameworks as inputs"
> *Introduction describing the input mechanism of DL compilers*





## Backlinks

- [[../../ONNX]]
