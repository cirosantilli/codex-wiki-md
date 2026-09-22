<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Von Mangoldt function](../../../../../../von-mangoldt-function.md) is nonnegative and satisfies $\Lambda(m)\leq\log m$. Using the [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md),

$$
(\Lambda*\Lambda)(n)
=\sum_{d\mid n}\Lambda(d)\Lambda(n/d)
\leq\sum_{d\mid n}\Lambda(d)\log(n/d)
\leq\log n\sum_{d\mid n}\Lambda(d)
=(\log n)^2.
$$

For $0<u\leq1$, a comparison with an [improper integral](../../../../../../improper-integral.md) gives

$$
\boxed{\sum_{n=1}^{\infty}\frac{(\log n)^2}{n^{1+u}}
\ll1+\int_1^\infty\frac{(\log t)^2}{t^{1+u}}\,dt
=1+\frac2{u^3}
\ll u^{-3}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
