<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [elementary row operation](../../../../../../elementary-row-operation.md) is one of three operations: interchange two rows, multiply one row by a nonzero [scalar](../../../../../../scalar.md), or add a scalar multiple of one row to a different row. Each operation is reversed by another operation of the same kind.

Performing such an operation on an $m\times n$ [matrix](../../../../../../matrix.md) $A$ is equivalent to left multiplication by the $m\times m$ [elementary matrix](../../../../../../elementary-matrix.md) obtained by applying that operation to the [identity matrix](../../../../../../identity-matrix.md). Each [elementary matrix](../../../../../../elementary-matrix.md) is invertible, with inverse corresponding to the reverse operation. Thus a sequence of operations gives

$$
B=E_kE_{k-1}\cdots E_1A,
\qquad
\boxed{B=PA,\quad P=E_k\cdots E_1\text{ invertible}.}
$$

For square [matrices](../../../../../../matrix.md), if $A$ were invertible, then $B=PA$ would have inverse $A^{-1}P^{-1}$. Hence **if $B$ is singular, $A$ must be singular as well**. In fact the two are invertible together, because $A=P^{-1}B$ gives the converse.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
