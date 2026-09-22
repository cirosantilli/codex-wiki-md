<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Because $|h^2|=|h|^2$, the [Parseval identity](../../../../../parseval-identity.md) for the [Taylor series](../../../../../taylor-series.md) gives

$$
M(r):=\frac1{2\pi}\int_0^{2\pi}|h^2(re^{i\theta})|d\theta=\boxed{\sum_{n\geq1}|c_n|^2r^{2n}}.
$$

Differentiate this [power series](../../../../../power-series.md) for $r<1$ and use [iii](../iii.md):

$$
M'(r)=\frac2r\sum_{n\geq1}n|c_n|^2r^{2n}=\frac{2\operatorname{Area}(h(r\mathbb D))}{\pi r}\leq\frac{2r}{(1-r^2)^2}.
$$

Since $M(0)=0$, integration yields the [integral mean bound for an odd square-root transform](../../../../../integral-mean-bound-for-an-odd-square-root-transform.md),

$$
\boxed{M(r)\leq\int_0^r\frac{2s}{(1-s^2)^2}ds=\frac{r^2}{1-r^2}}.
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../../split.md)
6. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
