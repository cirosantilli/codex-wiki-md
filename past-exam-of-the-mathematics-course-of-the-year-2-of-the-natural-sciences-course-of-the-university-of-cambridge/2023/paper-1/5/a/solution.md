<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $M^T=-M$, $(M^2)^T=(M^T)^2=M^2$, so $M^2$ is a real [symmetric matrix](../../../../../symmetric-matrix.md). Moreover,

$$
\boxed{x^TM^2x=-x^TM^TMx=-\|Mx\|^2\leq0,}
$$

proving that it is a [negative semidefinite matrix](../../../../../negative-semidefinite-matrix.md).

For odd $n$, [determinant](../../../../../determinant.md) invariance under transpose gives

$$
\det M=\det M^T=\det(-M)=(-1)^n\det M=-\det M,
$$

so $\det M=0$. Hence $M$ and $M^2$ have a zero [eigenvalue](../../../../../eigenvalue.md). Finally, if $M^2w=0$, then $0=w^TM^2w=-\|Mw\|^2$, so $Mw=0$. Thus

$$
\boxed{\ker M^2=\ker M,}
$$

where equality of these [kernels](../../../../../kernel-of-a-linear-map-split.md) includes the reverse implication, which is immediate.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
