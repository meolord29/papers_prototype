---
title: "Library Dependency Limitations"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 8
---

# Library Dependency Limitations

[[../../Operator_Implementation_Challenges|← Parent]]

> [!info] Concept (Level 3)
> Library dependency limitations describe the critical drawback of relying on vendor-provided optimized libraries for operator implementation. ==While libraries like MKL, cuBLAS, MKL-DNN, and cuDNN provide highly optimized implementations for common operations, they usually fall behind the rapid development of DL models.== ==This creates a gap where new operators or model architectures cannot utilize DL chips efficiently until library vendors update their implementations.== The lag time between model innovation and library support represents a significant bottleneck for practitioners. Additionally, these libraries are often hardware-specific, requiring separate implementations for different vendor ecosystems.

## Usage in this paper

The paper uses library dependency limitations to justify why DL compilers provide value beyond existing frameworks and libraries. The authors position compilers as a solution that alleviates the burden of optimizing DL models on each hardware manually. By generating code automatically rather than depending on pre-built libraries, compilers can support emerging models more rapidly. This challenge directly motivates the compiler-based approach over traditional library-dependent frameworks.

## References

> [!quote] Section 1 (p. 2)
> "However, the drawback of relying on the libraries is that they usually fall behind the rapid development of DL models, and thus fail to utilize the DL chips efficiently."
> *Explaining the fundamental limitation of library-based approaches*





## Backlinks

- [[../../Operator_Implementation_Challenges]]
