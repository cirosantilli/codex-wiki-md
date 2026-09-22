# Abstract syntax tree traversal

↑ **Parent:** [Abstract syntax tree](abstract-syntax-tree.md)

An [abstract syntax tree](abstract-syntax-tree.md) traversal systematically visits its nodes. A [depth-first traversal of a tree](depth-first-traversal-of-a-tree.md) that processes each child before its parent is called postorder. For the [program expression](program-expression.md) `2+3*4`, the schematic postorder is `2, 3, 4, Mult, Add`. This order lets an evaluator obtain each operand value before applying its operation. A traversal of the entire [Python](python-programming-language.md) schema additionally visits marker nodes such as `Add` and `Store`; this shorter list concerns only the expression nodes drawn in the figures. Visiting an [abstract syntax tree](abstract-syntax-tree.md) is a structural operation, and is not a general model of execution: a conditional may select only one branch, while a structural visitor examines both.

## ↑ Ancestors (4)

1. [Abstract syntax tree](abstract-syntax-tree.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Constant folding](constant-folding.md)
