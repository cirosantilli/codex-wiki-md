# Alias analysis

↑ **Parent:** [Compiler](compiler.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alias_analysis)

Analysis of whether two accesses may designate the same storage location. [Common subexpression elimination](common-subexpression-elimination.md) must not reuse a previously loaded value after a store that might change that location, unless an additional argument justifies it. A saved [memory address](memory-address.md) can remain valid even though a value previously loaded at that address is invalidated.

## ↑ Ancestors (4)

1. [Compiler](compiler.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Common subexpression elimination](common-subexpression-elimination.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/e/solution.md)
