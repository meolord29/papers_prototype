---
title: "Framework Interoperability"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 7
---

# Framework Interoperability

[[../../Graph-level_IR|← Parent]]

> [!info] Concept (Level 3)
> Framework Interoperability addresses the challenge of supporting multiple deep learning frameworks within a single compiler infrastructure. ==This sub-concept involves creating unified representation formats that facilitate model conversion between different DL frameworks like TensorFlow, PyTorch, MXNet, and CNTK.== Standards like ONNX define common formats for representing DL models to reduce redundant engineering efforts when supporting emerging models. ==The graph-level IR serves as the abstraction layer that enables framework-agnostic optimization while preserving model semantics.== Achieving interoperability is essential for reducing the burden of optimizing DL models on each hardware platform manually.

## Usage in this paper

The paper discusses Framework Interoperability as a key motivation for developing DL compilers with graph-level IR capabilities. ==The survey analyzes how different compilers implement the graph-level to achieve interoperability between frameworks while preserving model semantics for optimization.== ONNX is highlighted as a solution that defines a unified format for representing DL models to facilitate model conversion. The DL compilers take the DL models described in different DL frameworks as input, and then generate optimized codes for diverse DL hardware as output.

## References

> [!quote] Section 1 (p. 1)
> "To provide interoperability, ONNX [66] has been proposed, that defines a unified format for representing DL models to facilitate model conversion between different DL frameworks."
> *Explaining the need for interoperability standards*

> [!quote] Section 1 (p. 2)
> "The DL compilers take the DL models described in different DL frameworks as input, and then generate optimized codes for diverse DL hardware as output."
> *Describing the input-output relationship of DL compilers*





## Backlinks

- [[../../Graph-level_IR]]
