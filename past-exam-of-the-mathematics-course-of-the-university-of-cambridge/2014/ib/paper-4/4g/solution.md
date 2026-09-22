<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

For an [entire function](../../../../../entire-function.md), the [Cauchy derivative formula](../../../../../cauchy-derivative-formula.md) on a positively oriented circle of radius $R$ about $z_0$ is

$$
 \boxed{f^{(n)}(z_0)=\frac{n!}{2\pi i}\oint_{|\zeta-z_0|=R}
 \frac{f(\zeta)}{(\zeta-z_0)^{n+1}}\,d\zeta,\qquad n=0,1,\ldots.}
$$

The resulting [Cauchy estimate](../../../../../cauchy-estimate.md) is $|f^{(n)}(z_0)|\leq n!M_R/R^n$, where $M_R$ is the maximum of $|f|$ on that circle.

The [Liouville theorem](../../../../../liouville-theorem.md) says that a bounded [entire function](../../../../../entire-function.md) is constant. Indeed, if $|f|\leq M$ on the plane, the [Cauchy estimate](../../../../../cauchy-estimate.md) with $n=1$ gives $|f'(z_0)|\leq M/R$. Sending $R$ to infinity gives $f'(z_0)=0$ at every point, hence $f$ is constant.

For the growth assumption, apply the [Cauchy estimate](../../../../../cauchy-estimate.md) on circles centred at zero. For every integer $n>k$,

$$
 |f^{(n)}(0)|\leq n!R^{k-n}\longrightarrow0\quad(R\longrightarrow\infty).
$$

All sufficiently high [Taylor series](../../../../../taylor-series.md) vanish. Since the [Taylor series](../../../../../taylor-series.md) of an [entire function](../../../../../entire-function.md) converges everywhere, **$f$ is a polynomial**, of degree at most $\lfloor k\rfloor$ when $k\geq0$. If a negative finite exponent is interpreted for nonzero $z$, the same estimate forces every coefficient to vanish, giving $f=0$.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
