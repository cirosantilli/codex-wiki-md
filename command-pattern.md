# Command pattern

↑ **Parent:** [Software design pattern](software-design-pattern.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Command_pattern)

Represent a request and the information needed to execute it as a [software object](software-object.md) with a common command interface. Undoable commands additionally retain enough information to invert their change: an insertion retains its position and value, a deletion retains the removed value, and a positional move retains the source and final destination indices.

For sequential undo/redo, a history manager stores applied commands on one [stack](stack-data-structure.md) and undone commands on another. Undo transfers the most recent applied command to the redo [stack](stack-data-structure.md); redo transfers its head back after reapplying it. A fresh edit clears the redo branch. Command inverses are valid under this chronological protocol, not generally after unrelated intervening edits. Saving complete immutable versions instead gives a [Memento pattern](memento-pattern.md) implementation of the same undo/redo interface.

**Table of contents**

- [Inverse command correctness](inverse-command-correctness.md)

## ↑ Ancestors (5)

1. [Software design pattern](software-design-pattern.md)
2. [Object-oriented programming](object-oriented-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Behavioral pattern](behavioral-pattern.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/8/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/7/a/ii/solution.md)
