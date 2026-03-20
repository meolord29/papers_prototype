---
title: "The Deep Learning Compiler: A Comprehensive Survey"
date: 2026-03-20
tags: ['paper', 'research', 'deep-learning', 'compiler', 'optimization', 'intermediate-representation', 'auto-tuning', 'hardware-acceleration']
paper_type: survey
sections_detected: ['Abstract', 'Introduction', 'Background', 'Common Design Architecture', 'Key Components', 'Taxonomy', 'Evaluation', 'Conclusion']
analysis_depth: 2
analysis_breadth: 3
weight: 10
analyzed: true
---

# The Deep Learning Compiler: A Comprehensive Survey

## 🚀 The Journey Begins

Welcome to an illuminating exploration of deep learning compilers, the unsung heroes bridging the gap between cutting-edge AI models and the diverse hardware that powers them. As we journey through this comprehensive survey, you'll discover how these specialized compilers transform high-level model definitions into highly optimized code across CPUs, GPUs, and custom accelerators. Prepare to uncover the intricate architecture of multi-level intermediate representations, the sophisticated optimization techniques at frontend and backend, and the performance insights that reveal which compilers truly deliver. This tour will equip you with a deep understanding of what makes DL compilers unique and where the field is heading next.

---


## 🗺️ Chapter 1: Abstract & Introduction

As we begin our exploration, we encounter the fundamental challenge that sparked the DL compiler revolution: the difficulty of deploying various deep learning models on diverse hardware has boosted research and development in the community. Imagine standing at the crossroads where rapidly evolving neural network architectures meet an ever-expanding landscape of hardware accelerators from Google TPUs to NVIDIA GPUs to custom ASICs. ==This is where DL compilers emerge as the essential bridge, taking model definitions from frameworks like TensorFlow and PyTorch as input, then generating optimized code implementations for various hardware as output.==

==What makes this fascinating is that while several DL compilers have emerged from both industry and academia, none of the existing surveys had analyzed their unique design architecture comprehensively until this paper.== The authors position their work as the first survey focusing specifically on DL compiler design architecture, with emphasis on DL-oriented multi-level IRs and frontend/backend optimizations. ==This leads us to understand that the uniqueness of DL compilers lies not just in applying traditional compilation techniques, but in designing multi-level intermediate representations and DL-specific optimizations that traditional compilers simply cannot handle.==

==The paper's contributions are substantial: dissecting commonly adopted design architectures, providing comprehensive taxonomy of existing compilers, presenting quantitative performance comparisons, and highlighting future research directions.== As we move forward, keep in mind that this survey aims to pave the road for future DL compiler research, making it an invaluable guide for both practitioners selecting compilers and researchers pushing the boundaries of what's possible.

> [!quote] Abstract & Introduction
> "This is the first survey paper focusing on the design architecture of DL compilers, which we hope can pave the road for future research towards DL compiler."
> *This quote establishes the novelty and significance of the survey, positioning it as foundational work for the DL compiler community*

> [!info] 🔗 Concept: [[concepts/Deep_Learning_Compiler/Deep_Learning_Compiler|Deep Learning Compiler]]
> 
> Domain-specific compilers that transform DL models into optimized code for diverse hardware targets
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Intermediate_Representation_IR/Intermediate_Representation_IR|Intermediate Representation (IR)]]
> 
> Program abstraction used for optimizations, bridging model definitions and hardware code
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Multi-level_IR/Multi-level_IR|Multi-level IR]]
> 
> Layered IR design enabling both hardware-independent and hardware-specific optimizations
> 
> *Explore this concept further by clicking the link above.*

---

## 🗺️ Chapter 2: Background: Frameworks & Hardware

Now we step into the ecosystem that DL compilers must navigate, starting with the diverse landscape of deep learning frameworks. ==Picture a bustling marketplace where TensorFlow, PyTorch, MXNet, CNTK, and others each offer unique strengths and tradeoffs in their designs.== The interoperability challenge becomes critical here, which is why ONNX emerged to define a unified format for representing DL models and facilitate conversion between different frameworks. This fragmentation at the framework level is precisely why compilers are needed to provide a unified path to efficient execution.

As we explore further, we encounter an equally diverse hardware landscape that DL compilers must target. The computing characteristics of deep learning, particularly matrix multiplication, have spurred chip architects to design customized accelerators for higher efficiency. Internet giants like Google with TPU, processor vendors like NVIDIA with Turing, and even startups are investing tremendous resources in developing DL chips. ==The hardware can be divided into three categories: general-purpose hardware with software-hardware co-design, dedicated hardware fully customized for DL models, and neuromorphic hardware inspired by biological brain science.==

==This leads us to a critical insight: to embrace the hardware diversity, it is important to map the computation to DL hardware efficiently.== ==While optimized libraries like BLAS, cuDNN, and TensorRT serve as basics for efficient computation, they usually fall behind the rapid development of DL models and fail to utilize DL chips efficiently.== This is where DL compilers provide their value, incorporating DL-oriented optimizations like layer and operator fusion that enable highly efficient code generation while leveraging mature tool-chains from general-purpose compilers for better portability.

> [!quote] Background: Frameworks & Hardware
> "The DL compilers take the model definitions described in the DL frameworks as inputs, and generate efficient code implementations on various DL hardware as outputs."
> *This quote defines the core function of DL compilers in bridging frameworks and hardware*

> [!info] 🔗 Concept: [[concepts/Frontend_Optimizations/Frontend_Optimizations|Frontend Optimizations]]
> 
> Hardware-independent graph-level optimizations applied before code generation
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Backend_Optimizations/Backend_Optimizations|Backend Optimizations]]
> 
> Hardware-specific optimizations for efficient code generation on target platforms
> 
> *Explore this concept further by clicking the link above.*

---

## 🗺️ Chapter 3: Common Design Architecture

As we arrive at the heart of our journey, we discover the common design architecture that unites all DL compilers despite their different implementations. The architecture primarily contains two parts: the compiler frontend and the compiler backend, with intermediate representation spread across both. ==Think of this as a sophisticated translation pipeline where DL models enter at the frontend as computation graphs, undergo hardware-independent transformations and optimizations, then pass through to the backend where hardware-specific optimizations and code generation occur.==

==The high-level IR, also known as graph IR, resides in the frontend and represents computation and control flow in a hardware-independent manner.== The design challenge here is the ability of abstraction that can capture and express diverse DL models while establishing control flow and dependencies between operators and data. This provides an interface for graph-level optimizations and contains rich semantic information for compilation. ==The low-level IR, in contrast, is designed for hardware-specific optimization and code generation on diverse hardware targets, needing to be fine-grained enough to reflect hardware characteristics.==

What makes this architecture powerful is how it separates concerns: the frontend handles hardware-independent transformations including node-level, block-level, and dataflow-level optimizations, while the backend transforms high-level IR into low-level IR and performs hardware-specific optimizations. The backend can leverage third-party tool-chains like LLVM for general-purpose optimizations or take advantage of prior knowledge about DL models and hardware characteristics for more efficient code generation. ==This layered design with multi-level IRs is what truly distinguishes DL compilers from their traditional counterparts.==

> [!quote] Common Design Architecture
> "However, the uniqueness of DL compiler lies in the design of multi-level IRs and DL specific optimizations."
> *This quote captures the essential differentiator that makes DL compilers unique in the compilation landscape*

> [!info] 🔗 Concept: [[concepts/Operator_Fusion/Operator_Fusion|Operator Fusion]]
> 
> Combining multiple operators into single kernel to reduce overhead and improve efficiency
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping|Hardware Intrinsic Mapping]]
> 
> Mapping IR instructions to hardware-optimized kernels for maximum performance
> 
> *Explore this concept further by clicking the link above.*

---

## 🗺️ Chapter 4: Key Components: IR & Optimizations

Now we dive deep into the key components that make DL compilers work, starting with the sophisticated world of intermediate representations. The representation of graph IR influences expressiveness and decides how compilers analyze computation graphs. ==DAG-based IR is traditional, with nodes representing atomic DL operators and edges representing tensors, organized as directed acyclic graphs.== However, this has deficiencies like semantic ambiguity, which let-binding-based IR solves by offering let expressions with restricted scope. Different compilers adopt different strategies: TVM's Relay IR uses both DAG and let-binding, while XLA's HLO uses function-based representation.

As we explore the low-level IR implementations, we encounter three major categories that shape how compilers generate hardware-specific code. ==Halide-based IR separates computation from schedule, trying various possible schedules and choosing the best one.== Polyhedral-based IR uses linear programming and affine transformations to optimize loop-based codes with greater flexibility than Halide. Other unique IRs like Glow's instruction-based expression and MLIR's dialect system offer alternative approaches. The low-level IR is eventually lowered to LLVM IR in most compilers, benefiting from LLVM's mature optimizer and code generator.

This leads us to the optimization techniques that truly unlock performance. ==Frontend optimizations work at the graph level with node-level elimination, block-level algebraic simplification and operator fusion, and dataflow-level CSE and DCE.== Backend optimizations include hardware intrinsic mapping, memory allocation and fetching, memory latency hiding, loop-oriented optimizations, and parallelization. ==The combination of these optimizations at multiple levels is what enables DL compilers to generate code that can outperform manually optimized implementations.==

> [!quote] Key Components: IR & Optimizations
> "Operator fusion is indispensable optimization of DL compilers. It enables better sharing of computation, eliminates intermediate allocations, facilitates further optimization by combining loop nests."
> *This quote emphasizes operator fusion as a critical optimization technique in DL compilers*

> [!info] 🔗 Concept: [[concepts/Auto-tuning/Auto-tuning|Auto-tuning]]
> 
> Automatic determination of optimal optimization parameters through search and learning
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Polyhedral_Model/Polyhedral_Model|Polyhedral Model]]
> 
> Mathematical framework for loop optimization using linear programming and affine transformations
> 
> *Explore this concept further by clicking the link above.*

---

## 🗺️ Chapter 5: Evaluation & Performance

As we reach the empirical validation portion of our journey, we encounter rigorous performance comparisons that separate claims from reality. The authors evaluated five major DL compilers (TVM, nGraph, TC, Glow, and XLA) on 19 neural network models across different CPU and GPU platforms. What emerges from this comprehensive evaluation is a nuanced picture where different compilers excel in different scenarios, but clear patterns emerge about what drives performance.

==The most striking discovery is that tuned TVM almost achieves the best performance on both CPU and GPU across all models, especially on lightweight models like MobileNet and MNASNet series.== The performance difference between tuned and untuned TVM is negligible on CPU but quite significant on GPU, with an average 41.26× speedup. ==This reveals a critical insight: GPU has more complicated thread and memory hierarchy than CPU, thus to exploit the computation power, GPU requires more fine-grained scheduling where auto-tuning exhibits its effectiveness.==

As we examine per-layer performance, interesting patterns emerge about compiler strengths. ==nGraph achieves better convolution layer performance on CPU, benefiting from co-design of Intel hardware and software with DNNL library.== TVM performs better on GPU across compilers. Glow falls behind on 1×1 convolutions and depth-wise separable convolutions. XLA's performance varies dramatically depending on whether models come from ONNX or TensorFlow Hub, revealing compatibility challenges. ==These findings demonstrate that compiler selection should consider target hardware, model characteristics, and whether auto-tuning is feasible for the deployment scenario.==

> [!quote] Evaluation & Performance
> "The tuned TVM (tuned with 200 trials) almost achieves the best performance on both CPU and GPU across all models, especially on lightweight models."
> *This quote summarizes the key performance finding from the evaluation section*

> [!info] 🔗 Concept: [[concepts/Dynamic_Shape/Dynamic_Shape|Dynamic Shape]]
> 
> Handling tensors with unknown dimensions at compile time, critical for flexible models
> 
> *Explore this concept further by clicking the link above.*

> [!info] 🔗 Concept: [[concepts/Quantization/Quantization|Quantization]]
> 
> Reducing numerical precision to improve efficiency while maintaining model accuracy
> 
> *Explore this concept further by clicking the link above.*

---

## 🗺️ Chapter 6: Future Directions & Conclusion

As we conclude our journey through the DL compiler landscape, we look toward the horizon where exciting research opportunities await. The authors highlight several critical directions that will shape the future of DL compilers, starting with dynamic shape and pre/post-processing support. ==Dynamic models are becoming increasingly popular, especially in NLP where input shapes may change during execution, yet existing compilers require more research to support this efficiently.== Additionally, as models become more complex, their control flow will include complicated pre/post-processing that currently becomes a bottleneck when executed by Python interpreters.

==Advanced auto-tuning represents another frontier where current techniques focusing on individual operators must evolve.== The combination of local optimal does not lead to global optimal, and new optimization targets beyond execution time should be considered, such as memory footprint and energy consumption for edge computing. The polyhedral model combined with auto-tuning presents promising opportunities, though challenges remain in supporting sparse tensors. Subgraph partitioning opens possibilities for integrating graph libraries and enabling heterogeneous parallel execution across diverse computation units.

This leads us to the final insights about unified optimizations, differentiable programming, privacy protection, and training support. ==Currently, training is far less supported than inference in DL compilers, but expanding this capability would open large research opportunities.== Privacy protection in edge-cloud systems presents opportunities for compilers to guide noise insertion across layers automatically. ==The vision is clear: DL compilers will evolve from inference optimization tools to comprehensive platforms supporting the entire ML lifecycle while enabling efficient co-design of compilers and hardware accelerators.==

> [!quote] Future Directions & Conclusion
> "We highlight several insights for the future development of DL compilers, including dynamic shape and pre-/post-processing, advanced auto-tuning, polyhedral model, subgraph partitioning, quantization, unified optimizations, differentiable programming and privacy protection."
> *This quote summarizes the comprehensive future research directions identified by the authors*

> [!info] 🔗 Concept: [[concepts/Differentiable_Programming/Differentiable_Programming|Differentiable Programming]]
> 
> Programming paradigm enabling automatic differentiation of arbitrary programs
> 
> *Explore this concept further by clicking the link above.*

---


## 🔍 Deeper Explorations

Throughout this journey, we've encountered concepts that branch into rich topic areas. Here's your map to explore them further:

### From Abstract

- [[concepts/Deep_Learning_Compiler/Deep_Learning_Compiler|Deep Learning Compiler]] — Domain-specific compilers that transform DL models into optimized code for diverse hardware targets

### From Introduction

- [[concepts/Intermediate_Representation_IR/Intermediate_Representation_IR|Intermediate Representation (IR)]] — Program abstraction used for optimizations, bridging model definitions and hardware code
- [[concepts/Multi-level_IR/Multi-level_IR|Multi-level IR]] — Layered IR design enabling both hardware-independent and hardware-specific optimizations
- [[concepts/Frontend_Optimizations/Frontend_Optimizations|Frontend Optimizations]] — Hardware-independent graph-level optimizations applied before code generation
- [[concepts/Backend_Optimizations/Backend_Optimizations|Backend Optimizations]] — Hardware-specific optimizations for efficient code generation on target platforms

### From Section 3

- [[concepts/Auto-tuning/Auto-tuning|Auto-tuning]] — Automatic determination of optimal optimization parameters through search and learning
- [[concepts/Polyhedral_Model/Polyhedral_Model|Polyhedral Model]] — Mathematical framework for loop optimization using linear programming and affine transformations

### From Section 4.3.2

- [[concepts/Operator_Fusion/Operator_Fusion|Operator Fusion]] — Combining multiple operators into single kernel to reduce overhead and improve efficiency

### From Section 4.4.1

- [[concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping|Hardware Intrinsic Mapping]] — Mapping IR instructions to hardware-optimized kernels for maximum performance

### From Section 4.1.2

- [[concepts/Dynamic_Shape/Dynamic_Shape|Dynamic Shape]] — Handling tensors with unknown dimensions at compile time, critical for flexible models

### From Table 1

- [[concepts/Quantization/Quantization|Quantization]] — Reducing numerical precision to improve efficiency while maintaining model accuracy

### From Section 7

- [[concepts/Differentiable_Programming/Differentiable_Programming|Differentiable Programming]] — Programming paradigm enabling automatic differentiation of arbitrary programs


## 📊 Key Insights

As we conclude our journey through this paper, several critical insights emerge:

### 🔴 TVM with auto-tuning achieves best performance across CPU and GPU

Tuned TVM almost achieves the best performance on both CPU and GPU across all models, especially on lightweight models. The performance difference between tuned and untuned TVM is negligible on CPU but quite significant on GPU (41.26× speedup on average).

### 🔴 Multi-level IR design is the unique differentiator for DL compilers

Unlike traditional compilers, DL compilers employ multi-level intermediate representations with high-level graph IR for hardware-independent optimizations and low-level IR for hardware-specific code generation.

### 🟡 Frontend optimizations converge at three levels

Hardware-independent optimizations in the frontend converge at node-level (elimination), block-level (algebraic simplification, operator fusion), and dataflow-level (CSE, DCE, memory planning).

### 🟡 Auto-tuning is essential for GPU optimization

GPU has more complicated thread and memory hierarchy than CPU, thus requires more fine-grained scheduling. Auto-tuning exhibits its effectiveness in determining optimal scheduling parameters on GPU.

### 🟡 Training support remains limited in current DL compilers

Current DL compilers mainly focus on inference optimization. Training support is limited: nGraph only on NNP-T, TC only for single kernels, Glow experimental, TVM under development, XLA relies on TensorFlow.

### 🟡 Dynamic shape support is increasingly important

Dynamic models are becoming more popular, especially in NLP where input shapes may change during execution. Existing DL compilers require more research to support dynamic shape efficiently.


## 🔗 Quick Reference

**All Concepts in This Paper:**

- [[concepts/Deep_Learning_Compiler/Deep_Learning_Compiler|Deep Learning Compiler]]
- [[concepts/Backend_Optimizations/Backend_Optimizations|Backend Optimizations]]
- [[concepts/Frontend_Optimizations/Frontend_Optimizations|Frontend Optimizations]]
- [[concepts/Intermediate_Representation_IR/Intermediate_Representation_IR|Intermediate Representation (IR)]]
- [[concepts/Multi-level_IR/Multi-level_IR|Multi-level IR]]
- [[concepts/Auto-tuning/Auto-tuning|Auto-tuning]]
- [[concepts/Polyhedral_Model/Polyhedral_Model|Polyhedral Model]]
- [[concepts/Dynamic_Shape/Dynamic_Shape|Dynamic Shape]]
- [[concepts/Operator_Fusion/Operator_Fusion|Operator Fusion]]
- [[concepts/Hardware_Intrinsic_Mapping/Hardware_Intrinsic_Mapping|Hardware Intrinsic Mapping]]
- [[concepts/Differentiable_Programming/Differentiable_Programming|Differentiable Programming]]
- [[concepts/Quantization/Quantization|Quantization]]