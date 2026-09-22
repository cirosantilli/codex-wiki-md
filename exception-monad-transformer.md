# Exception monad transformer

↑ **Parent:** [Monad transformer](monad-transformer.md)

An unlabelled exception can be represented by an [algebraic data type](algebraic-data-type.md) with successful and failed alternatives, sequenced inside a base [computational monad](computational-monad.md). Sequencing skips the next computation after failure; a handler runs an alternative computation. The base effects already performed need not be undone.

## ↑ Ancestors (6)

1. [Monad transformer](monad-transformer.md)
2. [Computational monad](computational-monad.md)
3. [Functional programming](functional-programming.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/d/solution.md)
- [State monad transformer](state-monad-transformer.md)
