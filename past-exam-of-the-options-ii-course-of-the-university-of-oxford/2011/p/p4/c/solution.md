<h1 id="p/p4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) to the first column of $A$, using the identity if it is already the zero vector. This gives an [orthogonal matrix](../../../../../orthogonal-matrix.md) $H_1$ for which $H_1A$ has zeros below its first diagonal entry. At stage $j$, apply a [Householder transformation](../../../../../householder-transformation.md) to rows $j,\ldots,n$ of column $j$, and extend it by the identity on the first $j-1$ coordinates. If that trailing column is zero, again use the identity. The transformation preserves zeros in earlier columns, since their trailing entries already vanish.

After at most $n-1$ stages,

$$
R=H_{n-1}\cdots H_1A
$$

is an [upper triangular matrix](../../../../../upper-triangular-matrix.md). Each $H_j$ is symmetric and orthogonal, so with

$$
Q=H_1\cdots H_{n-1}
$$

we have $Q^TQ=I$ and

$$
\boxed{A=QR.}
$$

No invertibility assumption was used, so the [Householder QR decomposition](../../../../../householder-qr-decomposition.md) also exists for singular matrices.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
