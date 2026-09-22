<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

A complex [power series](../../../../../power-series.md) with [radius of convergence](../../../../../radius-of-convergence.md) $R$ converges absolutely at every $z$ with $|z|<R$ and diverges at every $z$ with $|z|>R$. This makes no general assertion at $|z|=R$: boundary points must be examined separately. The series always converges at $z=0$. If $R=0$, no nonzero point lies in the convergence disk; if $R=\infty$, the series converges absolutely throughout the [complex plane](../../../../../complex-plane.md).

If $p$ is the zero polynomial, every coefficient vanishes, so **$R=\infty$**. Otherwise let $d$ be its degree and $c\ne0$ its leading coefficient. Since $p(n)=cn^d(1+o(1))$,

$$
\left|\frac{p(n+1)}{p(n)}\right|\longrightarrow1.
$$

The [ratio test](../../../../../ratio-test.md) therefore proves absolute convergence when $|z|<1$. For $|z|>1$, the terms $p(n)z^n$ do not tend to zero, so the series diverges. Thus the [polynomial-coefficient power series](../../../../../polynomial-coefficient-power-series.md) has **$R=1$ for every nonzero polynomial**. In fact, it also diverges at every $|z|=1$, because $|p(n)z^n|=|p(n)|$ does not tend to zero, whether $d=0$ or $d>0$.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
