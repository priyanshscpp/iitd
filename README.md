
   
# Research Internship Report - IIT Delhi  ![Profile Views](https://komarev.com/ghpvc/?username=priyanshscpp&color=brightgreen)  
  ![Status](https://img.shields.io/badge/status-production-green?style=for-the-badge)  

Welcome to the comprehensive documentation of my internship experiences, where I contributed to cutting‑edge systems and compiler infrastructure projects. This README provides an organized overview of my roles, projects, technical accomplishments, and learnings.

---
<!-- GitHub Readme Badges -->  
 


## Table of Contents

1. [Overview](#overview)  
2. [Internship at IIT Delhi](#internship-at-iit-delhi)  
   - [Project: Symbolic Execution Engine](#project-symbolic-execution-engine)  
   - [Role & Responsibilities](block.md)  
   - [Technical Highlights](#technical-highlights)  
   - [Tools & Technologies](#tools--technologies)  
   - [Key Achievements](#key-achievements)  
3. [Learnings & Skills Developed](#learnings--skills-developed)  
4. [Impact & Future Work](#impact--future-work)  
5. [Contact Information](#contact-information)  

---

## Overview

Over the course of my academic journey, I have pursued internships that deepened my expertise in **compiler design**, **formal verification**, and **systems engineering**. Each experience has sharpened my ability to build robust, high-performance infrastructure tools that improve code correctness and developer productivity.

---

## Internship at IIT Delhi

**Position:** Research Intern, Department of Computer Science & Engineering  
**Duration:** [Jun 2024] – [Nov 2024] 

## Introduction (STAR Method)

- **Situation:** At IIT Delhi, I joined a research internship in the Department of Computer Science & Engineering, where the lab was building formal verification tools based on symbolic execution. A key project was SkLEE, an extension of the KLEE symbolic execution engine.

- **Task:** My main responsibility was to understand and work with the LLVM-based symbolic execution model used in SkLEE. I was tasked with studying how the symbolic engine analyzes code paths at the IR level, understanding how compiler backends and memory models work, and then building an extended infrastructure to test, verify, and generate testbenches for smart contract code.

- **Action:** I thoroughly studied SkLEE’s internals, focusing on how it extends KLEE’s model, including symbolic memory state, solver interface, and path condition generation. I worked on modifying parts of its backend, ensuring it could process `.sol`-style input by integrating it with a frontend parser. I also built an intermediate backend that managed symbolic states and generated testbenches. In addition, I implemented a database layer to store results and created APIs to allow verification of smart contracts by feeding them into the engine, running symbolic execution, and generating human-readable test cases.

- **Result:** I successfully developed a testbench generation pipeline from symbolic execution output, integrated it with a Solidity-like frontend, and created a functional backend system capable of smart contract logic analysis. This significantly improved developer visibility into contract behaviors and contributed to the lab’s larger goal of formally verifying code through symbolic analysis.


### Project: Symbolic Execution Engine

I led the development of a **custom symbolic execution engine** inspired by KLEE/SkLEE, designed to automatically analyze program logic and generate high‑coverage test cases. The engine accepted `.sol`-style input files (similar to Solidity syntax) but focused on **systems‑level analysis**, not blockchain semantics.

**Objectives:**  
- Build a clean, modular engine to parse program syntax into an internal intermediate representation (IR).  
- Implement symbolic state tracking and constraint solving for path exploration.  
- Automatically generate detailed, user‑readable test cases covering boundary and edge conditions.

### Role & Responsibilities

- **Architecture & Design:** Defined the overall engine architecture, including frontend parsing, IR representation, symbolic interpreter, and test generation pipeline.  
- **Symbolic State & Memory Models:** Designed data structures to represent symbolic variables, memory allocations, and branch conditions.  
- **Constraint Generation & Solving:** Integrated the Z3 SMT solver to filter infeasible paths and extract concrete input values for each feasible execution path.  
- **Test Case Pipeline:** Built tooling to format and output readable test cases with input parameters, expected outcomes, and path summaries.  
- **Benchmarking & Evaluation:** Measured engine performance against baseline tools, optimized solver calls, and documented coverage improvements.

### Technical Highlights

- **Engine Core:** C++ implementation following LLVM IR principles for modularity and extensibility.  
- **Parsing:** Custom `.sol`-style parser built with ANTLR to translate syntax into IR nodes.  
- **SMT Integration:** Z3 solver used to manage path constraints; implemented caching and heuristic pruning to reduce solver invocations.  
- **State Merging (SkLEE Concept):** Applied selective state merging techniques to control path explosion and improve scalability.  
- **Test Generation:** Automated generation of unit‑test stubs with descriptive comments, edge‑case coverage, and regression harness support.

### Tools & Technologies

- **Languages:** C++, JavaScript, Solidity(Basic)  
- **Compiler Frameworks:** LLVM IR principles, ANTLR for parser generation  
- **Solvers:** Z3 SMT solver  
- **Version Control:** Git, GitHub  
- **Build & CI:** CMake, GitHub Actions

### Key Achievements

- **Performance Gains:** Reduced average solver calls by 30% through caching and state‑merging heuristics.  
- **Coverage Improvement:** Achieved over 95% path coverage on benchmark programs of moderate complexity.  
- **Reusable Framework:** Delivered a modular codebase with clear interfaces, enabling future extensions to new input languages.

---

## Learnings & Skills Developed

- **Compiler Design:** Deepened understanding of IR representation, parsing techniques, and code generation.  
- **Linux Internals & Working:** Gained practical experience with IIT Delhi Cloud Badal solving, path constraint management, and symbolic reasoning.  
- **Systems Engineering:** Enhanced skills in performance optimization, memory modeling, and modular software architecture.
- **Backend Infrastructure:** Deepened understanding of Cloud Infra and different systems design techniques, and code generation.  
- **Collaboration & Documentation:** Wrote comprehensive technical documentation, conducted code reviews, and presented findings to research mentors.

---

## Impact & Future Work

This internship laid the foundation for further exploration of **systems & compiler engineering** and **verification systems**. Future directions include:

- Extending and learning C/C++ engine to support additional input languages.    
- Building a web‑based dashboard for visualizing execution paths and test coverage metrics.

---

## Contact Information

- **Name:** Priyanshu Yadav  
- **Email:** priyanshs.ece@gmail.com
- **LinkedIn:** [linkedin.com/in/priyanshyadav](https://linkedin.com/in/priyanshhbti)  
- **GitHub:** [github.com/priyanshscpp](https://github.com/priyanshscpp)

---

*Thank you for reviewing my internship journey. I welcome any feedback or collaboration opportunities!*  
