# Common subexpression elimination

↑ **Parent:** [Compiler](compiler.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Common_subexpression_elimination)

A transformation that computes a repeated [program expression](program-expression.md) once and reuses its saved result when the value is known not to have changed. A repeated load can be reused only when intervening stores, calls or other changes cannot alter the relevant location. [Alias analysis](alias-analysis.md) helps establish that fact. Maximal address sharing can be counterproductive if [instruction selection](instruction-selection.md) could otherwise fold an address [addition](addition.md) into [register-offset addressing](register-offset-addressing.md).

## ↑ Ancestors (4)

1. [Compiler](compiler.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Alias analysis](alias-analysis.md)
- [Oxford Compilers examination paper (2015)](oxford-compilers-examination-paper-2015.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/e/solution.md)
