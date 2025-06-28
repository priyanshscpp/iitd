
   
# Research Internship Report - IIT Delhi  ![Profile Views](https://komarev.com/ghpvc/?username=priyanshscpp&color=brightgreen)  
  ![Status](https://img.shields.io/badge/status-production-green?style=for-the-badge)  

Welcome to the comprehensive documentation of my internship experiences, where I contributed to cutting‑edge systems and compiler infrastructure projects. This README provides an organized overview of my roles, projects, technical accomplishments, and learnings.

---
<!-- GitHub Readme Badges -->  
 


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


# SkLEE Smart Contract Verification Tool

## Introduction

SkLEE is an advanced formal verification tool developed within the Department of Computer Science & Engineering at IIT Delhi. Built upon the foundation of the KLEE symbolic execution engine, SkLEE extends its capabilities to provide robust analysis and testbench generation for smart contracts. This project aims to enhance the reliability and security of smart contract code by formally verifying its behavior through symbolic execution.

## My Role and Contributions

During my research internship, my primary responsibility was to delve into SkLEE's LLVM-based symbolic execution model. This involved a deep dive into how the symbolic engine analyzes code paths at the Intermediate Representation (IR) level, understanding the intricacies of compiler backends and memory models.

My key contributions include:

* **Understanding SkLEE's Architecture:** Thoroughly studied the internals of SkLEE, focusing on its extensions to KLEE's core model, including symbolic memory state management, solver interface integration, and path condition generation.
* **Frontend Integration for Solidity:** Modified SkLEE's backend to process `.sol`-style input by integrating it with a specialized frontend parser, enabling direct analysis of Solidity smart contracts.
* **Intermediate Backend Development:** Built an intermediate backend responsible for managing symbolic states and generating comprehensive testbenches. This component translates symbolic execution outputs into practical test cases.
* **Database Layer and API Development:** Implemented a persistent database layer to store verification results and developed APIs. These APIs facilitate feeding smart contracts into the engine, executing symbolic analysis, and generating human-readable test cases for developers.

## Features

* **Symbolic Execution for Smart Contracts:** Leverages the power of symbolic execution to explore all possible execution paths of smart contract code.
* **LLVM IR Level Analysis:** Operates at the LLVM Intermediate Representation (IR) level, providing low-level and precise code analysis.
* **Solidity Compatibility:** Integrated with a frontend parser to directly process and analyze `.sol` (Solidity) files.
* **Automated Testbench Generation:** Automatically generates comprehensive test cases based on symbolic execution output, aiding in developer understanding and debugging.
* **Symbolic State Management:** Manages complex symbolic memory states and path conditions during execution.
* **Database for Results:** Stores verification results in a structured database for easy access and analysis.
* **API for Verification:** Provides APIs to streamline the process of submitting smart contracts for verification and retrieving generated test cases.

## How it Works (Conceptual Overview)

1.  **Input:** A Solidity smart contract (`.sol` file) is provided as input.
2.  **Frontend Parsing:** The integrated frontend parser converts the Solidity code into an intermediate representation suitable for SkLEE.
3.  **Symbolic Execution:** SkLEE's symbolic execution engine takes this IR and explores all possible execution paths, maintaining symbolic values for variables and generating path conditions.
4.  **Backend Processing:** The modified backend processes the symbolic execution results, managing symbolic states and preparing data for testbench generation.
5.  **Testbench Generation:** The intermediate backend generates human-readable test cases based on the symbolic execution output, capturing different execution scenarios and their corresponding inputs/outputs.
6.  **Results Storage & API:** Verification results and generated testbenches are stored in a database, accessible via dedicated APIs.

## Installation and Usage (Conceptual)

*(Note: Detailed installation and usage instructions would typically go here, including prerequisites, build steps, and example commands. As this is a README for a past project, these are conceptual placeholders.)*

**Prerequisites:**

* LLVM
* Clang
* Z3 (or other SMT solver)
* Solidity compiler (for frontend integration)
* Python (for scripting, APIs, and database interaction)

**Building SkLEE:**

```bash
# Example commands (actual commands would depend on project structure)
git clone <sklee-repository-url>
cd sklee
mkdir build
cd build
cmake ..
make

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
