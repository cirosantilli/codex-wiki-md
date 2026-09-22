# Optimal stack evaluation of a binary expression tree

↑ **Parent:** [Stack machine](stack-machine.md)

Suppose each subtree of a [binary expression tree](binary-expression-tree.md) is evaluated completely before its sibling, leaves one result on an operand [stack](stack-data-structure.md), and is not spilled or interleaved. If the child depths are $p,q$, evaluating the first child needs $p$ slots and keeping its result while evaluating the second needs $1+q$. Reversing the order gives $\max(q,1+p)$. If either order preserves the expression's meaning, the minimum is $\max(p,q)$ when $p\ne q$ and $p+1$ when $p=q$. For example, if $p>q$, integrality gives $p\geq q+1$, so evaluating the deeper child first attains the lower bound $p$. If $p=q$, the second child needs its own $p$ slots plus one saved result regardless of order. Induction over the [binary expression tree](binary-expression-tree.md) proves optimality in this evaluation model.

For a noncommutative operator, an instruction swapping the top two [stack](stack-data-structure.md) entries or a reverse-operand opcode permits the same ordering while preserving operand positions. Reordering still requires absence of order-sensitive [side effects](side-effect-computer-science.md). Reassociation and interleaving are separate transformations and are not part of this optimality claim.

## ↑ Ancestors (5)

1. [Stack machine](stack-machine.md)
2. [Abstract machine](abstract-machine.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof/6/d/solution.md)
