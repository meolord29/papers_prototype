---
title: "Auto-Differentiation Compiler Support"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 2
weight: 9
---

# Auto-Differentiation Compiler Support

[[../../Differentiable_Programming|← Parent]]

> [!info] Concept (Level 2)
> This sub-concept encompasses the compiler infrastructure needed to support automatic differentiation across general computations beyond neural networks. ==Auto-differentiation requires the compiler to track operations, build computation graphs, and generate gradient computation code automatically.== The compiler must handle both forward and reverse mode differentiation depending on the program structure and performance requirements. Supporting high-order derivatives adds additional complexity as the compiler must differentiate its own differentiation logic. ==This capability extends the DL compiler paradigm from optimizing fixed neural architectures to optimizing learnable algorithms.==

## Usage in this paper

The paper positions auto-differentiation support as a future direction with little current implementation in existing DL compilers. Current compilers like TVM and XLA focus on optimizing predefined neural network operations rather than general differentiable code. ==The authors suggest that supporting this paradigm would allow DL compilers to handle more general computations beyond standard neural networks.== This represents an evolution from framework-specific optimization to general differentiable program compilation.

## References

> [!quote] Section 1 (p. 3)
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection"
> *Differentiable programming identified as a key future research insight for DL compiler community*



## Sub-Concepts

The concept of Auto-Differentiation Compiler Support unfolds across three interconnected dimensions within the DL compiler architecture. **Computation Graph Construction** establishes the foundational capability by enabling compilers to track operations and build intermediate representations that capture computational dependencies. This directly enables **Gradient Code Generation** which leverages the graph structure to automatically produce efficient backward pass implementations for derivative computation. Finally, understanding both reveals why **Differentiable Programming Extension** is critical as it represents the evolution from optimizing fixed neural networks to supporting general learnable algorithms beyond standard DL models.

- [[sub_concepts/Computation_Graph_Construction/Computation_Graph_Construction|Computation Graph Construction]]
- [[sub_concepts/Gradient_Code_Generation/Gradient_Code_Generation|Gradient Code Generation]]
- [[sub_concepts/Differentiable_Programming_Extension/Differentiable_Programming_Extension|Differentiable Programming Extension]]


## Backlinks

- [[../../Differentiable_Programming]]
- [[sub_concepts/Computation_Graph_Construction/Computation_Graph_Construction]]
- [[sub_concepts/Gradient_Code_Generation/Gradient_Code_Generation]]
- [[sub_concepts/Differentiable_Programming_Extension/Differentiable_Programming_Extension]]
