# Interpreter (computing)

↑ **Parent:** [Programming language](programming-language-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interpreter_(computing))

An [interpreter](interpreter-computing.md) executes a program's operations according to its [programming language semantics](programming-language-semantics.md). It can recursively evaluate an [abstract syntax tree](abstract-syntax-tree.md), or follow an instruction sequence using an execution state such as a [stack](stack-data-structure.md) and an [instruction pointer](instruction-pointer.md). It need not repeatedly read [source code](source-code.md) characters, and it need not use an [abstract syntax tree](abstract-syntax-tree.md) at all.

[Compilation](compilation.md) and interpretation can coexist. In [CPython](cpython.md), [Python](python-programming-language.md) [source code](source-code.md) is compiled into [bytecode](bytecode.md) for execution by an [interpreter](interpreter-computing.md); its [bytecode](bytecode.md) is not promised to remain stable between releases.[Python 3.14 documentation; Python 3.14 glossary: bytecode and virtual machine entries; compilation, execution and release-specific bytecodes](python-3-14-documentation/glossary-python-3-14-documentation.md) The [Python](python-programming-language.md) 3.14 `compile` function accepts text or an [abstract syntax tree](abstract-syntax-tree.md) and can produce a code object, which `eval` or `exec` can execute.[Python 3.14 documentation; Python 3.14 Built-in Functions: compile, accepted source forms, code objects and execution by eval or exec](python-3-14-documentation/built-in-functions-python-3-14-documentation.md) These operations make translation and execution separately accessible without requiring them to live in different applications.

[Just-in-time compilation](just-in-time-compilation.md) gives another combination: an interactive implementation can translate a submitted [program expression](program-expression.md) into [machine code](machine-code.md) and then execute it immediately. The [LLVM](llvm.md) 20.1.0 tutorial demonstrates this by adding an [intermediate representation](intermediate-representation.md) module to its [just-in-time compilation](just-in-time-compilation.md) facility, looking up the generated function, and calling it.[LLVM 20.1.0 documentation; Implementing a language with LLVM, chapter 4, section 4.4: HandleTopLevelExpression, addModule, lookup and calling the generated native function](llvm-20-1-0-documentation/4-kaleidoscope-adding-jit-and-optimizer-support.md) Thus calling a [programming language](programming-language-split.md) permanently "compiled" or "interpreted" hides an implementation choice: ask which representation is translated, which is executed, and when.

**Table of contents**

- [Interpreter arithmetic trace](interpreter-arithmetic-trace.md)

## ↑ Ancestors (3)

1. [Programming language](programming-language-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
