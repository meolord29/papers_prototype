---
title: "Performance Measurement and Selection"
date: 2026-03-21
tags: ["deep-learning", "compiler-optimization", "hardware-acceleration", "intermediate-representation", "auto-tuning"]
depth_level: 3
weight: 8
---

# Performance Measurement and Selection

[[../../Search_Algorithm_Strategies|← Parent]]

> [!info] Concept (Level 3)
> Performance measurement and selection provides the evaluation mechanism that guides search algorithm decisions toward high-performance configurations. ==This component involves executing candidate configurations and measuring their actual runtime performance on target hardware.== The selection process compares multiple configurations to identify the optimal one based on performance metrics. Accurate measurement is critical because search algorithms rely on this feedback to refine their exploration strategies. ==The quality of performance selection directly impacts the speedups achieved by auto-tuned compilers compared to untuned versions.==

## Usage in this paper

==The paper provides quantitative performance comparison among DL compilers to show the effectiveness of optimizations including auto-tuning.== The evaluation compares both end-to-end and per-layer performance to demonstrate how well search strategies identify high-performance configurations. This performance-driven approach validates that search algorithm effectiveness directly impacts practical performance gains. The paper's open-sourced evaluation scripts enable reproducibility of performance measurement and selection outcomes.

## References

> [!quote] Section 1 (p. 3)
> "We have provided the quantitative performance comparison among DL compilers on CNN models, including full-fledged models and lightweight models."
> *Describes the evaluation methodology used to assess compiler optimization effectiveness*





## Backlinks

- [[../../Search_Algorithm_Strategies]]
