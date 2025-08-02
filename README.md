# Project: Build "meg" Programming Language

This document outlines the steps to build the "meg" programming language from scratch, including its virtual machine, compiler, and language features.

## Phase 1: The Virtual Machine (VM)

- [x] **Project Setup**
    - [x] Create a Cargo workspace.
    - [x] Create `meg-vm`, `meg-cli`, and `meg` crates.
- [ ] **Instruction Set Definition**
    - [ ] Define a simple set of opcodes (e.g., `OP_RETURN`, `OP_CONSTANT`).
    - [ ] Create a struct to represent an instruction.
- [ ] **Chunk of Bytecode**
    - [ ] Create a `Chunk` struct to store bytecode.
    - [ ] Implement a way to write instructions and constants to the chunk.
- [ ] **The Virtual Machine**
    - [ ] Create a `VM` struct.
    - [ ] Implement the fetch-decode-execute loop.
    - [ ] Implement the execution for `OP_RETURN` and `OP_CONSTANT`.
    - [ ] Implement a stack.
- [ ] **Debugging**
    - [ ] Create a disassembler to print the instructions in a chunk.
    - [ ] Implement a way to trace the VM's execution.

## Phase 2: The Compiler

- [ ] **Scanner (Lexer)**
    - [ ] Implement a scanner to turn source code into a stream of tokens.
    - [ ] Define all the token types (keywords, operators, literals, etc.).
- [ ] **Compiler**
    - [ ] Implement a compiler that takes the stream of tokens and generates bytecode.
    - [ ] Implement parsing for simple expressions.
    - [ ] Handle operator precedence.
- [ ] **Values**
    - [ ] Represent values in the VM (numbers, booleans, nil).
- [ ] **More Instructions**
    - [ ] Add instructions for arithmetic operations (`OP_ADD`, `OP_SUBTRACT`, etc.).
    - [ ] Add instructions for unary and binary operators.

## Phase 3: Language Features

- [ ] **Global Variables**
    - [ ] Implement instructions for defining and accessing global variables.
- [ ] **Local Variables**
    - [ ] Implement instructions for local variables.
    - [ ] Manage variable scopes.
- [ ] **Control Flow**
    - [ ] Implement `if` statements.
    - [ ] Implement logical operators.
    - [ ] Implement `while` and `for` loops.
- [ ] **Functions**
    - [ ] Implement function calls.
    - [ ] Handle arguments and return values.
    - [ ] Implement native functions.
- [ ] **Closures**
    - [ ] Implement closures and upvalues.

## Phase 4: Advanced Topics

- [ ] **Garbage Collection**
    - [ ] Implement a garbage collector to manage memory automatically.
- [ ] **Classes and Instances**
    - [ ] Implement classes, methods, and initializers.
    - [ ] Implement inheritance.

## Phase 5: Beyond the VM (Future)

- [ ] **Native Code Generation**
    - [ ] Explore using a backend like LLVM to generate native code.
