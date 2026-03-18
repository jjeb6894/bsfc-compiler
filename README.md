# bsfc-compiler
Experimental compiler architecture exploring bidirectional fixpoint optimization (BSFC), convergent IR transformations, and AI-assisted code generation beyond traditional SSA pipelines.
# BSFC Compiler
### Bidirectional Semantic Fixpoint Compilation
**Author: Jamie Ellul Bonici**

---

## Overview

BSFC is an experimental compiler architecture that models compilation as a **bidirectional fixpoint convergence process**.

Unlike traditional SSA-based pipelines, BSFC continuously refines IR both upward and downward until convergence:

    IR = T↑(T↓(IR))

---

## Research

**Bidirectional Semantic Fixpoint Compilation**  
Jamie Ellul Bonici  
arXiv:2603.11872 [cs.PL] (submitted)

---

## Key Features

- Bidirectional IR transformations  
- Fixpoint convergence instead of pass ordering  
- Cost-aware optimization  
- Translation witnesses for verification  

---

## Benchmarks

- ~14–18% performance improvement vs LLVM-style pipelines  
- ~85% reduction in optimization variance  
- Deterministic convergence behavior  

See `/benchmarks/benchmark.md`

---

## CLI

Run:

    cargo run --bin bsfc-cli -- --compare llvm

---

## Vision

A next-generation compiler architecture combining:

- systems optimization  
- VM design  
- AI-assisted compilation  
