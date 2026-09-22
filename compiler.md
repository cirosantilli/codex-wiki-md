# Compiler

↑ **Parent:** [Programming language](programming-language-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compiler)

A [compiler](compiler.md) translates a program from one representation to another while aiming to preserve its [programming language semantics](programming-language-semantics.md). Its input might be [source code](source-code.md) or an [intermediate representation](intermediate-representation.md); its output might be another [programming language](programming-language-split.md), [bytecode](bytecode.md), an [intermediate representation](intermediate-representation.md), or [machine code](machine-code.md). Producing [machine code](machine-code.md) is therefore one possible destination, rather than the definition of [compilation](compilation.md). For example, the [LLVM](llvm.md) 20.1.0 tutorial translates an [abstract syntax tree](abstract-syntax-tree.md) into an [intermediate representation](intermediate-representation.md) before introducing execution.[LLVM 20.1.0 documentation; Implementing a language with LLVM, chapter 3, sections 3.1 and 3.5: AST to LLVM IR and the initial driver that prints IR](llvm-20-1-0-documentation/3-kaleidoscope-code-generation-to-llvm-ir.md)

[Compilation](compilation.md) can use an [abstract syntax tree](abstract-syntax-tree.md) for checking and transformations such as [constant folding](constant-folding.md) before producing [machine code](machine-code.md). These are useful possibilities, not a compulsory sequence of separate stages for every [compiler](compiler.md). The central distinction is between translating a program and executing its operations: a [compiler](compiler.md) can translate `x*(2+3)-4` without knowing the input value of `x`, whereas an [interpreter](interpreter-computing.md) needs that value to produce this [program expression](program-expression.md)'s result.

Different representations expose different questions. [Source code](source-code.md) preserves what a programmer wrote; an [abstract syntax tree](abstract-syntax-tree.md) exposes grouping; a [type system](type-system.md) checks permitted combinations; a [stack machine](stack-machine.md) makes operand movement explicit. Retaining [abstract syntax tree source locations](abstract-syntax-tree-source-location.md) across [compilation](compilation.md) helps an error message identify the original construct even after [constant folding](constant-folding.md) has changed its shape. A malformed `x*(2+)-4` is a [programming language syntax](programming-language-syntax.md) error; an unavailable `x` in the valid example is instead a missing input. Locating the failing rule is more helpful than treating both as an unexplained execution failure.

**Table of contents**

- [Compilation](compilation.md)
  - [Compilation arithmetic example](compilation-arithmetic-example.md)
  - [Just-in-time compilation](just-in-time-compilation.md)
- [Intermediate representation](intermediate-representation.md)
  - [Bytecode](bytecode.md)
- [LLVM](llvm.md)

## ↑ Ancestors (3)

1. [Programming language](programming-language-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Abstract syntax tree](abstract-syntax-tree.md)
- [Compilation](compilation.md)
- [Compilation arithmetic example](compilation-arithmetic-example.md)
- [Compiler](compiler.md)
- [Source code](source-code.md)
