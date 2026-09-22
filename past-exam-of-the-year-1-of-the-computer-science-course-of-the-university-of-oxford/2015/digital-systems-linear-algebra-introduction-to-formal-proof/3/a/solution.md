<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $U,V$ be $n\times n$ [upper triangular matrices](../../../../../upper-triangular-matrix.md). For an entry below the diagonal, $i>j$, [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
(UV)_{ij}=\sum_{k=1}^nU_{ik}V_{kj}.
$$

If $k<i$, then $U_{ik}=0$. If $k\geq i$, then $k>j$, so $V_{kj}=0$. Every summand is zero, giving

$$
\boxed{i>j\implies(UV)_{ij}=0.}
$$

Thus $UV$ is an [upper triangular matrix](../../../../../upper-triangular-matrix.md). Equivalently, a potentially nonzero summand would require $i\leq k\leq j$, impossible below the diagonal.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
