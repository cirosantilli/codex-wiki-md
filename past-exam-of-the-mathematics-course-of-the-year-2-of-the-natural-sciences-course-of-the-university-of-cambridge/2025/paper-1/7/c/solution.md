<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the first function, the complex exponential has no [zeros](../../../../../zero-of-a-function.md), while the denominator has three distinct simple [zeros](../../../../../zero-of-a-function.md). Thus there are $\boxed{\text{simple poles at }z=0,\,2i,\,-2i;\ \text{no finite zeros}}$. To examine infinity, substitute $z=1/w$:

$$
\frac{e^{1/w}}{[(1/w)^2+4]/w}=\frac{w^3e^{1/w}}{1+4w^2}.
$$

The factor $e^{1/w}$ has an [essential singularity](../../../../../essential-singularity.md) at zero, and multiplication by a nonzero finite-order factor cannot remove it. Therefore $\boxed{\infty\text{ is an isolated essential singularity}}$ of the first function.

For the second function, $\sin z$ has simple [zeros](../../../../../zero-of-a-function.md) at $z=n\pi$. At zero, its [Taylor series](../../../../../taylor-series.md) gives

$$
\frac{z^2}{\sin^2z}=\left(\frac{z}{z-z^3/6+O(z^5)}\right)^2=1+\frac{z^2}{3}+O(z^4),
$$

so $\boxed{z=0\text{ is removable, with extended value }1}$. Every other $z=n\pi$ is a double [pole](../../../../../pole.md), since the numerator is nonzero there. There are no finite [zeros](../../../../../zero-of-a-function.md), including after removal at zero.

At infinity the double [poles](../../../../../pole.md) $n\pi$ accumulate. Equivalently, after $z=1/w$, the function $1/[w^2\sin^2(1/w)]$ has double [poles](../../../../../pole.md) at $w=1/(n\pi)$ tending to zero. Hence $\boxed{\infty\text{ is a non-isolated singularity}}$. The removable/pole/essential trichotomy for [isolated singularities](../../../../../isolated-singularity-split.md) does not apply there; calling this an isolated [essential singularity](../../../../../essential-singularity.md) would be incorrect.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
