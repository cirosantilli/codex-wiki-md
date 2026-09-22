<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $B^k=0$ with $k\geq1$, put $S=I+B+\cdots+B^{k-1}$. The [matrix geometric series](../../../../../../matrix-geometric-series.md) telescopes on both sides:

$$
(I-B)S=S(I-B)=I-B^k=I.
$$

Thus **$I-B$ is nonsingular**, and

$$
\boxed{(I-B)^{-1}=\sum_{j=0}^{k-1}B^j.}
$$

This is a finite polynomial identity for a [nilpotent matrix](../../../../../../nilpotent-matrix.md); no convergence argument or bound $\|B\|<1$ is required.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
