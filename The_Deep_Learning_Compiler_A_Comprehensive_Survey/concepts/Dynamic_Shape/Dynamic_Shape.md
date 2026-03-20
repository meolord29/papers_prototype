---
title: "Dynamic Shape"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 10
---

# Dynamic Shape

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==Dynamic shape refers to the ability of a model to handle input tensors with dimensions that are not known until runtime.== This feature is becoming increasingly popular in fields like natural language processing where input lengths vary. ==Existing DL compilers require more research efforts to support dynamic shape efficiently for emerging dynamic models.== Supporting this requires relaxing bound inference and dimension checking mechanisms. ==It remains a significant challenge for static compilation graphs.==

## Usage in this paper

The survey highlights dynamic shape as a key future direction for DL compiler research. ==Particularly, in the area of NLP, models may accept inputs of various shapes, which is challenging for DL compilers since the shape of data is unknown until runtime.== Some compilers like TVM and XLA have started to support unknown dimension sizes using placeholders. This indicates a shift towards more flexible compilation strategies.

## References

> [!quote] Section 7 (p. 27)
> "Existing DL compilers require more research efforts to support dynamic shape efficiently for emerging dynamic models."
> *Identifies dynamic shape support as a future research direction.*



## Sub-Concepts

The concept of Dynamic Shape unfolds across several interconnected challenges in DL compiler design. **Runtime Dimension Unknown** establishes the fundamental problem by defining why tensor dimensions cannot be determined during compilation time. This directly necessitates **Placeholder-based Support** which provides the technical mechanism compilers use to handle these unknown dimensions. Understanding both reveals why **NLP Model Requirements** drive the practical demand for dynamic shape capabilities in real-world applications. Finally, these challenges collectively expose the **Static Compilation Graph Limitations** that traditional compilers face when adapting to dynamic workloads.

- [[sub_concepts/Runtime_Dimension_Unknown/Runtime_Dimension_Unknown|Runtime Dimension Unknown]]
- [[sub_concepts/Placeholder-based_Support/Placeholder-based_Support|Placeholder-based Support]]
- [[sub_concepts/NLP_Model_Requirements/NLP_Model_Requirements|NLP Model Requirements]]
- [[sub_concepts/Static_Compilation_Graph_Limitations/Static_Compilation_Graph_Limitations|Static Compilation Graph Limitations]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Runtime_Dimension_Unknown/Runtime_Dimension_Unknown]]
- [[sub_concepts/Placeholder-based_Support/Placeholder-based_Support]]
- [[sub_concepts/NLP_Model_Requirements/NLP_Model_Requirements]]
- [[sub_concepts/Static_Compilation_Graph_Limitations/Static_Compilation_Graph_Limitations]]
