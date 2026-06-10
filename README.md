# NovaLang VM

A modern educational programming language and stack-based virtual machine built from scratch in C++.

## Overview

NovaLang VM is a deep systems programming project focused on understanding how real programming languages work internally.

The project includes:

* Lexer
* Parser
* AST (Abstract Syntax Tree)
* Bytecode Compiler
* Stack-Based Virtual Machine
* Garbage Collector
* AI Debugger
* Web Playground

The goal is to explore compiler engineering, runtime systems, memory management, and VM architecture through a fully custom language implementation.

---

# Architecture

```txt
Source Code
    ↓
Lexer
    ↓
Tokens
    ↓
Parser
    ↓
AST
    ↓
Bytecode Compiler
    ↓
Virtual Machine
    ↓
Program Execution
```

---

# Core Components

## Lexer

Converts source code into tokens.

Example:

```nova
let x = 5 + 10;
```

Tokens:

```txt
LET IDENTIFIER EQUAL NUMBER PLUS NUMBER SEMICOLON
```

---

## Parser

Builds an Abstract Syntax Tree (AST) from tokens.

Responsible for:

* syntax validation
* operator precedence
* expression parsing

---

## Compiler

Converts AST nodes into bytecode instructions.

Example bytecode:

```txt
PUSH 5
PUSH 10
ADD
STORE x
```

---

## Virtual Machine

Executes bytecode instructions using a stack-based execution model.

Features:

* instruction dispatch
* runtime stack
* variable scopes
* function calls

---

## Memory System

Custom memory management system with planned garbage collection support.

Planned:

* heap allocation
* mark-and-sweep GC
* memory visualization

---

## AI Debugger

AI-assisted debugging system that explains compiler and runtime errors in natural language.

Example:

```txt
Undefined variable 'x'
```

AI Explanation:

```txt
The variable 'x' was used before being declared.
```

---

# Tech Stack

## Core Runtime

* C++17
* CMake

## Frontend Playground

* Next.js
* Tailwind CSS
* Monaco Editor

## Backend Services

* FastAPI

## Visualization

* D3.js

## AI Integration

* OpenAI API / Groq API

---

# Planned Features

## Language Features

* Variables
* Arithmetic
* Conditions
* Loops
* Functions
* Arrays
* Objects

## VM Features

* Stack execution
* Bytecode interpreter
* Function call stack
* Runtime scopes

## Educational Features

* AST visualization
* Stack visualization
* Bytecode inspector
* Memory inspector

---

# Development Roadmap

## Phase 1 — Core Frontend

* [ ] Token system
* [ ] Lexer
* [ ] Parser
* [ ] AST generation

## Phase 2 — Compiler

* [ ] Bytecode generation
* [ ] Constants table
* [ ] Variable resolution

## Phase 3 — VM

* [ ] Stack machine
* [ ] Instruction execution
* [ ] Runtime environment

## Phase 4 — Language Features

* [ ] Loops
* [ ] Functions
* [ ] Arrays
* [ ] Objects

## Phase 5 — Memory System

* [ ] Heap allocator
* [ ] Garbage collector
* [ ] Memory visualization

## Phase 6 — AI Features

* [ ] AI debugger
* [ ] Error explanations
* [ ] Optimization suggestions

## Phase 7 — Playground

* [ ] Browser IDE
* [ ] Live execution
* [ ] Stack visualizer

---

# Project Goals

This project exists to deeply understand:

* compiler design
* runtime systems
* virtual machines
* memory management
* bytecode execution
* programming language internals

The long-term goal is to build a fully interactive educational platform for learning how programming languages work internally.

---

# Current Status

Early architecture and compiler design phase.

Currently working on:

* token system
* AST design
* bytecode architecture
* VM execution model

---

# Build Instructions

## Clone Repository

```bash
git clone https://github.com/yourusername/novalang-vm.git
cd novalang-vm
```

## Build

```bash
mkdir build
cd build
cmake ..
make
```

---

# Inspiration

Inspired by:

* Lua VM
* CPython bytecode
* JVM architecture
* Crafting Interpreters
* LLVM concepts

---

# License

MIT License
