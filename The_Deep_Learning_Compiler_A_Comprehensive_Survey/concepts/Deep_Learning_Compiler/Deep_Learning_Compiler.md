---
title: "Deep Learning Compiler"
date: 2026-03-20
tags: ["concept", "depth-1"]
depth_level: 1
weight: 10
---

# Deep Learning Compiler

[[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 1)
> ==A deep learning compiler is a domain-specific compiler that takes deep learning model definitions from various frameworks as input and generates optimized code implementations for diverse hardware targets as output.== ==Unlike traditional compilers, DL compilers incorporate DL-oriented optimizations such as layer and operator fusion, enabling highly efficient code generation.== They leverage mature tool-chains from general-purpose compilers while addressing the unique computing characteristics of neural networks. These compilers are essential for bridging the gap between rapidly evolving DL models and increasingly diverse hardware accelerators.

## Usage in this paper

==In this survey, DL compilers are the central subject of analysis, with five major compilers (TVM, nGraph, TC, Glow, XLA) examined in depth.== The paper dissects their common design architecture into frontend, multi-level IRs, and backend components. The authors provide comprehensive taxonomy and quantitative performance comparison to guide practitioners and researchers.

## References

> [!quote] Abstract (p. 1)
> "The DL compilers take the DL models described in different DL frameworks as input, and then generate optimized codes for diverse DL hardware as output."
> *Defines the fundamental purpose of DL compilers*



## Sub-Concepts

- [[sub_concepts/Multi-level_Intermediate_Representation_Architectu|Multi-level Intermediate Representation Architecture]]
- [[sub_concepts/Auto-Tuning|Auto-Tuning]]
- [[../Operator_Fusion/Operator_Fusion|Operator Fusion]]
- [[../Frontend_Optimizations/Frontend_Optimizations|Frontend Optimizations]]
- [[../Backend_Optimizations/Backend_Optimizations|Backend Optimizations]]
- [[../Intermediate_Representation_IR/sub_concepts/IR_Implementation_Variations_Across_Compilers|IR Implementation Variations Across Compilers]]
- [[../Intermediate_Representation_IR/sub_concepts/IR_Role_in_Frontend_and_Backend_Optimizations|IR Role in Frontend and Backend Optimizations]]
- [[../Multi-level_IR/sub_concepts/High-Level_Intermediate_Representation|High-Level Intermediate Representation]]
- [[../Multi-level_IR/sub_concepts/Low-Level_Intermediate_Representation|Low-Level Intermediate Representation]]
- [[../Frontend_Optimizations/sub_concepts/Node-level_Optimizations|Node-level Optimizations]]
- [[../Frontend_Optimizations/sub_concepts/Block-level_Optimizations|Block-level Optimizations]]
- [[../Frontend_Optimizations/sub_concepts/Dataflow-level_Optimizations|Dataflow-level Optimizations]]
- [[../Backend_Optimizations/sub_concepts/Optimized_Kernel_Libraries|Optimized Kernel Libraries]]
- [[../Backend_Optimizations/sub_concepts/Hardware-Specific_Code_Generation|Hardware-Specific Code Generation]]
- [[../Auto-tuning/sub_concepts/Cost_Model_Types|Cost Model Types]]
- [[../Auto-tuning/sub_concepts/Search_Techniques|Search Techniques]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Extensible_Tensorization|Extensible Tensorization]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Quantization-Aware_Intrinsic_Mapping|Quantization-Aware Intrinsic Mapping]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/SIMD_Opcode_Pattern_Matching|SIMD Opcode Pattern Matching]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Specialized_Hardware_Feature_Leveraging|Specialized Hardware Feature Leveraging]]
- [[../Dynamic_Shape/sub_concepts/Compiler_Support_Variability|Compiler Support Variability]]
- [[../Dynamic_Shape/sub_concepts/Runtime_Dimension_Handling|Runtime Dimension Handling]]
- [[../Dynamic_Shape/sub_concepts/Memory_Validity_Guarantees|Memory Validity Guarantees]]
- [[../Dynamic_Shape/sub_concepts/Model_Compatibility_Issues|Model Compatibility Issues]]
- [[../Quantization/sub_concepts/Quantization_Precision_Support|Quantization Precision Support]]
- [[../Quantization/sub_concepts/Quantized_Operator_Implementation|Quantized Operator Implementation]]
- [[../Quantization/sub_concepts/Quantization_Optimization_Interaction|Quantization Optimization Interaction]]
- [[../Polyhedral_Model/sub_concepts/Polyhedral-based_Intermediate_Representation|Polyhedral-based Intermediate Representation]]
- [[../Polyhedral_Model/sub_concepts/Hybrid_Integration_with_Halide_Framework|Hybrid Integration with Halide Framework]]
- [[../Polyhedral_Model/sub_concepts/Auto-tuning_Integration_Challenges|Auto-tuning Integration Challenges]]
- [[../Polyhedral_Model/sub_concepts/Loop_Transformation_Capabilities|Loop Transformation Capabilities]]
- [[../Differentiable_Programming/sub_concepts/Automatic_Differentiation_Capability|Automatic Differentiation Capability]]
- [[../Differentiable_Programming/sub_concepts/Imperative_to_Symbolic_IR_Transformation|Imperative to Symbolic IR Transformation]]
- [[../Differentiable_Programming/sub_concepts/Control_Flow_and_Semantic_Differences|Control Flow and Semantic Differences]]


## Backlinks

- [[../../The_Deep_Learning_Compiler_A_Comprehensive_Survey]]
- [[sub_concepts/Multi-level_Intermediate_Representation_Architectu]]
- [[sub_concepts/Auto-Tuning]]
- [[../Operator_Fusion/Operator_Fusion]]
- [[../Frontend_Optimizations/Frontend_Optimizations]]
- [[../Backend_Optimizations/Backend_Optimizations]]
- [[../Intermediate_Representation_IR/sub_concepts/IR_Implementation_Variations_Across_Compilers]]
- [[../Intermediate_Representation_IR/sub_concepts/IR_Role_in_Frontend_and_Backend_Optimizations]]
- [[../Multi-level_IR/sub_concepts/High-Level_Intermediate_Representation]]
- [[../Multi-level_IR/sub_concepts/Low-Level_Intermediate_Representation]]
- [[../Frontend_Optimizations/sub_concepts/Node-level_Optimizations]]
- [[../Frontend_Optimizations/sub_concepts/Block-level_Optimizations]]
- [[../Frontend_Optimizations/sub_concepts/Dataflow-level_Optimizations]]
- [[../Backend_Optimizations/sub_concepts/Optimized_Kernel_Libraries]]
- [[../Backend_Optimizations/sub_concepts/Hardware-Specific_Code_Generation]]
- [[../Auto-tuning/sub_concepts/Cost_Model_Types]]
- [[../Auto-tuning/sub_concepts/Search_Techniques]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Extensible_Tensorization]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Quantization-Aware_Intrinsic_Mapping]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/SIMD_Opcode_Pattern_Matching]]
- [[../Hardware_Intrinsic_Mapping/sub_concepts/Specialized_Hardware_Feature_Leveraging]]
- [[../Dynamic_Shape/sub_concepts/Compiler_Support_Variability]]
- [[../Dynamic_Shape/sub_concepts/Runtime_Dimension_Handling]]
- [[../Dynamic_Shape/sub_concepts/Memory_Validity_Guarantees]]
- [[../Dynamic_Shape/sub_concepts/Model_Compatibility_Issues]]
- [[../Quantization/sub_concepts/Quantization_Precision_Support]]
- [[../Quantization/sub_concepts/Quantized_Operator_Implementation]]
- [[../Quantization/sub_concepts/Quantization_Optimization_Interaction]]
- [[../Polyhedral_Model/sub_concepts/Polyhedral-based_Intermediate_Representation]]
- [[../Polyhedral_Model/sub_concepts/Hybrid_Integration_with_Halide_Framework]]
- [[../Polyhedral_Model/sub_concepts/Auto-tuning_Integration_Challenges]]
- [[../Polyhedral_Model/sub_concepts/Loop_Transformation_Capabilities]]
- [[../Differentiable_Programming/sub_concepts/Automatic_Differentiation_Capability]]
- [[../Differentiable_Programming/sub_concepts/Imperative_to_Symbolic_IR_Transformation]]
- [[../Differentiable_Programming/sub_concepts/Control_Flow_and_Semantic_Differences]]
