# Matroid closure exchange property

↑ **Parent:** [Matroid](matroid.md)

The [closure of a matroid](closure-of-a-matroid.md) obeys the displayed exchange rule. This is the finite [pregeometry](pregeometry.md) exchange principle: if adding $x$ newly makes $y$ dependent, then adding $y$ also makes $x$ dependent.

**Proof.** Write $r=r(A)$. The first hypothesis and the one-element bound on the [rank of a matroid](rank-of-a-matroid.md) give $r(A+y)=r+1$. The second gives $r(A+x+y)=r(A+x)\leq r+1$. Inclusion gives $r(A+x+y)\geq r(A+y)$, so equality holds. This is exactly $x\in\operatorname{cl}_M(A+y)$.

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/viii/solution.md)
