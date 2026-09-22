# Compilation

↑ **Parent:** [Compiler](compiler.md)

[Compilation](compilation.md) is the translation process performed by a [compiler](compiler.md), which may include checking and transforming an [abstract syntax tree](abstract-syntax-tree.md). Translation can finish before execution, or happen during execution through [just-in-time compilation](just-in-time-compilation.md). Reusing the translated representation can avoid repeated [parsing](parsing.md) and repeated [constant folding](constant-folding.md) when only the inputs change. This does not guarantee a speedup: translation itself costs work, and the choice of representation and execution mechanism matters.

<a id="image-compiler-representation-pipeline"></a>
![](compiler-representation-pipeline.png)

**[Figure 3](#image-compiler-representation-pipeline). One possible compilation pipeline for `x*(2+3)-4`, with execution from an abstract syntax tree, a stack machine instruction sequence, or machine code**.

**Table of contents**

- [Compilation arithmetic example](compilation-arithmetic-example.md)
- [Just-in-time compilation](just-in-time-compilation.md)

## ↑ Ancestors (4)

1. [Compiler](compiler.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Abstract syntax tree](abstract-syntax-tree.md)
- [Bytecode](bytecode.md)
- [Compilation](compilation.md)
- [Compilation arithmetic example](compilation-arithmetic-example.md)
- [Compiler](compiler.md)
- [Constant folding](constant-folding.md)
- [Interpreter arithmetic trace](interpreter-arithmetic-trace.md)
- [Interpreter (computing)](interpreter-computing.md)
- [Just-in-time compilation](just-in-time-compilation.md)
- [LLVM](llvm.md)
