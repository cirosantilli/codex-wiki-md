<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With sufficiently many [derivatives](../../../../../derivative.md), [Taylor's theorem](../../../../../taylor-s-theorem.md) gives a finite approximation and a controlled remainder. For example, if $f$ is $N+1$ times continuously differentiable between $a$ and $a+\delta$, then

$$
\boxed{f(a+\delta)=\sum_{j=0}^N\frac{f^{(j)}(a)}{j!}\delta^j
+\frac{f^{(N+1)}(a+\theta\delta)}{(N+1)!}\delta^{N+1}},\qquad0<\theta<1.
$$

Thus [derivatives](../../../../../derivative.md) at the nearby base point determine the [polynomial](../../../../../polynomial-split.md) approximation; a bound on the next [derivative](../../../../../derivative.md) bounds its error. The smallness of $\delta$ makes this useful, provided the [derivatives](../../../../../derivative.md) remain controlled.

The statement's bare assumption of differentiability alone guarantees only $f(a+\delta)=f(a)+f'(a)\delta+o(\delta)$. Higher-order formulas need higher regularity. Even smoothness does not by itself guarantee equality with an infinite [Taylor series](../../../../../taylor-series.md); that stronger conclusion requires the remainder to tend to zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
