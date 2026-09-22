# Recursion (computer science)

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Recursion_(computer_science))

[Recursion](recursion-computer-science.md) solves a problem by invoking the same procedure on smaller instances, with base cases answered directly. For [merge sort](merge-sort.md), an empty or one-entry [array](array-data-structure.md) is already sorted, and every larger [array](array-data-structure.md) is split into two shorter parts. The decreasing lengths justify termination; a self-call without a progress rule would not suffice.

A [recursive procedure](recursive-procedure.md) refers to itself, directly or through another procedure. A [recursive call](recursive-call.md) starts another invocation, with its own arguments and local [variables](variable-mathematics.md); the caller can wait for its returned [output](output-computing.md). A [base case](base-case.md) supplies an answer without further [recursive calls](recursive-call.md). To establish [algorithm termination](algorithm-termination.md), also show that every [recursive call](recursive-call.md) progresses in a [well-founded relation](well-founded-relation.md). “Smaller” means smaller in that chosen relation: argument values need not all decrease, and the arguments need not even be numbers.

[Recursion](recursion-computer-science.md) is especially expressive when a [data structure](data-structure-split.md) already decomposes into smaller structures. A [binary tree](binary-tree.md) has two child [subtrees](subtree.md), so [structural recursion](structural-recursion.md) can follow its shape. A short rule for each case can describe an entire traversal or computation. The distinction between a [recursive procedure](recursive-procedure.md) and the [recursive process](recursive-process.md) it generates helps connect that compact description to its resource use.[Structure and Interpretation of Computer Programs, second edition, §1.2.1: procedure versus process; §1.2.2: closing discussion before Counting change, hierarchical data and straightforward definitions](structure-and-interpretation-of-computer-programs-by-harold-abelson-and-others.md)

**Table of contents**

- [McCarthy 91 function](mccarthy-91-function.md)
  - [Generalized McCarthy function](generalized-mccarthy-function.md)
- [Recursive procedure](recursive-procedure.md)
- [Recursive process](recursive-process.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Well-founded progress in recursion](well-founded-progress-in-recursion.md)
- [Base case](base-case.md)
- [Recursive call](recursive-call.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
