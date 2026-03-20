---
title: "Search Techniques"
date: 2026-03-20
tags: ["concept", "depth-2"]
depth_level: 2
weight: 9
---

# Search Techniques

[[../Auto-tuning|← Parent]] → [[../../../The_Deep_Learning_Compiler_A_Comprehensive_Survey|📄 The Deep Learning Compiler: A Comprehensive Survey]]

> [!info] Concept (Level 2)
> Search techniques are algorithms used to navigate the enormous parameter space to find optimal configurations efficiently. ==The paper identifies three main categories: genetic algorithms (GA) that use evolutionary principles, simulated annealing (SA) that employs probabilistic acceptance of worse solutions, and reinforcement learning (RL) that learns optimal policies through trial and error.== Each technique has different trade-offs in terms of convergence speed, solution quality, and computational overhead. Genetic algorithms are population-based and can explore diverse regions simultaneously. ==Reinforcement learning represents the most advanced approach, enabling the tuner to learn from past tuning experiences across different models and hardware configurations.==

## Usage in this paper

The paper discusses search techniques as part of the comprehensive analysis of auto-tuning mechanisms in DL compilers. Different compilers employ different search strategies depending on their design goals and target hardware characteristics. ==The performance evaluation demonstrates that proper search technique selection can achieve significant speedups, with tuned TVM achieving 41.26× speedup on GPU compared to untuned version.== This shows the critical importance of search technique optimization in practical DL compiler deployments.

## References

> [!quote] Section 1 (Contributions) (p. 2)
> "We dissect the commonly adopted design architecture of existing DL compilers, and provide detailed analysis of the key design components such as multi-level IRs, frontend optimizations and backend optimizations"
> *The paper commits to detailed analysis of backend optimizations including auto-tuning search techniques*





## Backlinks

- [[../Auto-tuning]]
