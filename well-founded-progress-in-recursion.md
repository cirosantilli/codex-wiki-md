# Well-founded progress in recursion

↑ **Parent:** [Recursion (computer science)](recursion-computer-science.md)

A [base case](base-case.md) and a decreasing [natural number](natural-number.md) measure work together. Check that every invocation satisfies its [precondition](precondition.md), each [base case](base-case.md) finishes with the correct [output](output-computing.md), and every other invocation makes finitely many [recursive calls](recursive-call.md) with strictly smaller measure. All local work must also terminate. By [well-founded induction](well-founded-induction.md), the children finish, so their caller finishes; if their answers are correct and the combination rule preserves the [postcondition](postcondition.md), the caller is correct too. This proves [total correctness](total-correctness.md), not just correctness conditional on return.

Strict decrease without a lower bound is insufficient: subtracting one forever from a negative [integer](integer-split.md) never reaches zero. Even a positive real-valued measure can decrease indefinitely, as $1,1/2,1/4,\ldots$ shows. A [well-founded relation](well-founded-relation.md) rules out that descent. In [structural recursion](structural-recursion.md), a proper child [subtree](subtree.md) of a finite [binary tree](binary-tree.md) supplies progress without numeric arguments. The proof obligation is the relation between parent and child instances, together with terminating local work and complete [base cases](base-case.md).

## ↑ Ancestors (4)

1. [Recursion (computer science)](recursion-computer-science.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Algorithm termination](algorithm-termination.md)
