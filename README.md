
   
# Internship Journey Documentation

Welcome to the comprehensive documentation of my internship experiences, where I contributed to cutting‑edge systems and compiler infrastructure projects. This README provides an organized overview of my roles, projects, technical accomplishments, and learnings.

---
<!-- GitHub Readme Badges -->  
  ![Profile Views](https://komarev.com/ghpvc/?username=priyanshscpp&color=brightgreen)  
  ![Status](https://img.shields.io/badge/status-production-green?style=for-the-badge)  
  ![Watchers](https://img.shields.io/github/watchers/priyanshscpp/internship-journey?style=social&label=Watchers)  
  ![Forks](https://img.shields.io/github/forks/priyanshscpp/internship-journey?style=social&label=Forks)  
  ![Stars](https://img.shields.io/github/stars/priyanshscpp/internship-journey?style=social&label=Stars)  
  ![Issues](https://img.shields.io/github/issues/priyanshscpp/internship-journey?style=for-the-badge&color=orange)  
  ![License](https://img.shields.io/github/license/priyanshscpp/internship-journey?style=for-the-badge&color=blue)  
  ![Last Commit](https://img.shields.io/github/last-commit/priyanshscpp/internship-journey?style=for-the-badge)  

## Table of Contents

1. [Overview](#overview)  
2. [Internship at IIT Delhi](#internship-at-iit-delhi)  
   - [Project: Symbolic Execution Engine](#project-symbolic-execution-engine)  
   - [Role & Responsibilities](#role--responsibilities)  
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
**Duration:** [Month Year] – [Month Year]

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

- **Languages:** C++, Python (scripting & automation)  
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
- **Linux Internals & Wokring:** Gained practical experience with SMT solving, path constraint management, and symbolic reasoning.  
- **Systems Engineering:** Enhanced skills in performance optimization, memory modeling, and modular software architecture.
- **Compiler Design:** Deepened understanding of IR representation, parsing techniques, and code generation.  
- **Collaboration & Documentation:** Wrote comprehensive technical documentation, conducted code reviews, and presented findings to research mentors.

---

## Impact & Future Work

This internship laid the foundation for further exploration of **automated program analysis** and **verification systems**. Future directions include:

- Extending the engine to support additional input languages (e.g., C, Rust).  
- Integrating advanced heuristics for dynamic state merging to handle larger codebases.  
- Building a web‑based dashboard for visualizing execution paths and test coverage metrics.

---

## Contact Information

- **Name:** Priyanshu Yadav  
- **Email:** pri.yadav@example.com  
- **LinkedIn:** [linkedin.com/in/priyanshyadav](https://linkedin.com/in/priyanshyadav)  
- **GitHub:** [github.com/priyanshscpp](https://github.com/priyanshscpp)

---

*Thank you for reviewing my internship journey. I welcome any feedback or collaboration opportunities!*  
