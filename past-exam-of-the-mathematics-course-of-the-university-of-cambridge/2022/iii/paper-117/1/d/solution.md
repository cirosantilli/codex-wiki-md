<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $L=\log D$. By the [Prime number theorem](../../../../../../prime-number-theorem.md) and [partial summation](../../../../../../abel-s-summation-formula.md), the sum is at most a constant times

$$
\int_2^z
\frac1{t(\log t)^4}
\exp\left(-\frac{L}{2\log t}\right)dt.
$$

Make the substitution $v=L/\log t$. Since $dt/t=-L v^{-2}dv$, this becomes

$$
\frac1{L^3}
\int_{L/\log z}^{L/\log2}v^2e^{-v/2}\,dv
\leq
\frac1{L^3}
\int_{L/\log z}^{\infty}v^2e^{-v/2}\,dv.
$$

For $u>0$, the final integral is $O(e^{-cu})$ after decreasing the absolute constant $c>0$; any polynomial factor in $u$ is absorbed by the exponential, and bounded $u$ causes no problem. Taking $u=L/\log z$ proves

$$
\sum_{p\leq z}\frac1{p(\log p)^3}
\exp\left(-\frac12\frac{\log D}{\log p}\right)
\ll\frac1{(\log D)^3}
\exp\left(-c\frac{\log D}{\log z}\right),
$$

the [exponentially damped reciprocal-prime sum](../../../../../../exponentially-damped-reciprocal-prime-sum.md) estimate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
