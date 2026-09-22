<h1 id="8b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The determinant factors as

$$
\det A=-2(\mu-1)(\mu+1).
$$

Thus for $\mu\ne\pm1$, the [kernel](../../../../../../kernel-of-a-linear-map.md) is $\{0\}$ and the inhomogeneous system has exactly one solution.

At $\mu=-1$, row reduction gives

$$
\ker A=\operatorname{span}\{(1,-2,3)^T\},
$$

and the augmented matrix has the same rank two as $A$, so there are infinitely many solutions. At $\mu=1$,

$$
\ker A=\operatorname{span}\{(-1,-2,3)^T\},
$$

but the augmented matrix has rank three while $A$ has rank two, so there is no solution. Therefore the number of solutions is

$$
\boxed{
\begin{cases}
1,&\mu\ne\pm1,\\
\infty,&\mu=-1,\\
0,&\mu=1.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
