---
title: "ONNX"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 10
---

# ONNX

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==ONNX (Open Neural Network Exchange) defines a unified format for representing DL models to facilitate model conversion.== It allows computation graphs built by different DL frameworks to be easily transformed into a standard format. ==With ONNX, it becomes easier to convert models between DL frameworks like PyTorch and MXNet.== This interoperability reduces redundant engineering efforts when supporting emerging DL models. ==It serves as a common input format for many DL compilers.==

## Usage in this paper

In the survey, ONNX is mentioned as a key enabler for interoperability among DL frameworks. ==As shown in the taxonomy, compilers like TVM and nGraph support ONNX input formats to import models.== For several DL frameworks that are not directly supported yet, ONNX adds converters to them. This makes ONNX a critical bridge in the compiler input pipeline.

## References

> [!quote] Introduction (p. 1)
> "To provide interoperability, ONNX has been proposed, that defines a unified format for representing DL models to facilitate model conversion between different DL frameworks."
> *Introduces ONNX as a solution for framework interoperability.*



## Sub-Concepts

The role of ONNX in the deep learning compiler ecosystem unfolds through three interconnected dimensions. **Unified Model Representation Format** establishes the foundational schema that defines how models are stored independently of specific frameworks. This standardization directly enables the **Framework Interoperability Bridge**, which allows models to flow seamlessly between competing environments like PyTorch and TensorFlow without redundant engineering. Once models are standardized and interchangeable, they can be efficiently ingested by compilation tools through **Compiler Input Standardization**, which simplifies frontend design. Together, these aspects illustrate how ONNX acts as the central hub that connects model creation to optimized hardware deployment. Understanding this flow reveals why ONNX is considered a critical enabler for interoperability among DL frameworks in the survey.

- [[sub_concepts/Unified_Model_Representation_Format/Unified_Model_Representation_Format|Unified Model Representation Format]]
- [[sub_concepts/Framework_Interoperability_Bridge/Framework_Interoperability_Bridge|Framework Interoperability Bridge]]
- [[sub_concepts/Compiler_Input_Standardization/Compiler_Input_Standardization|Compiler Input Standardization]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Unified_Model_Representation_Format/Unified_Model_Representation_Format]]
- [[sub_concepts/Framework_Interoperability_Bridge/Framework_Interoperability_Bridge]]
- [[sub_concepts/Compiler_Input_Standardization/Compiler_Input_Standardization]]
