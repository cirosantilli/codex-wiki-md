# Transform-sensitive trait frequency counter

↑ **Parent:** [Stackable trait modification](stackable-trait-modification.md)

A counting [trait](trait.md) that increments the original argument to insertion assumes that subsequent [traits](trait.md) store that argument unchanged. A later capitalization [trait](trait.md) breaks the assumption: the counter can record lowercase `a` while the document stores uppercase `A`. To maintain counts of actual document contents across such a composition, inspect the stored character after delegation or constrain the legal mixin order. Correctness for one base implementation does not establish correctness under every [trait](trait.md) combination.

## ↑ Ancestors (6)

1. [Stackable trait modification](stackable-trait-modification.md)
2. [Mixin](mixin.md)
3. [Object-oriented programming](object-oriented-programming.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/imperative-programming/7/b/solution.md)
