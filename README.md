# WLP4 Compiler

> This project was done as coursework so it cannot be openly shared as per Policy 71 of the University of Waterloo, the source code is available upon request.

A compiler for WLP4, a compact C-like programming language used to teach compiler construction. The project implements the major stages of a compiler pipeline, from scanning source code into tokens to generating low-level MIPS assembly.

## What is WLP4?

WLP4 is a strict subset of C++ built around procedures, `int` and `int*` types, arithmetic expressions, pointer operations, dynamic memory allocation, conditional statements, loops, and basic output. A WLP4 program ends with a special main procedure called `wain`, making the language small enough to compile end-to-end while still covering realistic compiler concepts such as lexical analysis, context-free parsing, semantic validation, type checking, stack-frame layout, and code generation.

Official language references:

- [WLP4 Programming Language Tutorial](https://student.cs.uwaterloo.ca/~cs241/wlp4/WLP4tutorial.html)
- [WLP4 Programming Language Specification](https://student.cs.uwaterloo.ca/~CS241/wlp4/)

## Demo

https://github.com/user-attachments/assets/56a36c61-d54c-4b29-9f74-2a2d8b0f67fa

## Technical Highlights

- Built a DFA-based scanner for tokenizing WLP4 source programs
- Implemented table-driven SLR parsing to construct a parse tree
- Added semantic analysis for declarations, procedure signatures, scopes, and invalid program states
- Implemented type checking for integers, pointers, expressions, assignments, comparisons, and function calls
- Generated MIPS assembly for expressions, control flow, procedure calls, stack management, printing, and heap allocation
- Managed runtime behavior for stack frames, local variables, parameters, pointer arithmetic, and memory access
