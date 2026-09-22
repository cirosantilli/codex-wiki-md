<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [induced metric](../../../../../../induced-metric.md) is obtained from the ambient [Euclidean metric](../../../../../../euclidean-metric.md) by the [pullback of a Riemannian metric](../../../../../../pullback-of-a-riemannian-metric.md) operation. Differentiating $x^2+a^2\rho^2=1$ on a branch with $x\ne0$ gives $dx=-a^2\rho\,d\rho/x$. Also $dy^2+dz^2=d\rho^2+\rho^2d\phi^2$. Consequently

$$
\boxed{g=E(\rho)d\rho^2+\rho^2d\phi^2,\qquad E(\rho)=1+\frac{a^4\rho^2}{1-a^2\rho^2}=\frac{1+a^2(a^2-1)\rho^2}{1-a^2\rho^2}.}
$$

The assumption that $(\rho,\phi)$ are coordinates already excludes the equator $x=0$ as well as the poles $\rho=0$. On such a chart, $0<\rho<1/|a|$ and $E>0$.

The [conformal flattening of a surface of revolution](../../../../../../conformal-flattening-of-a-surface-of-revolution.md) supplies the particularly simple [conformal factor](../../../../../../conformal-factor.md)

$$
\boxed{\Omega=\rho^{-1},\qquad \Omega^2g=\frac{E(\rho)}{\rho^2}d\rho^2+d\phi^2=d\sigma^2+d\phi^2,\quad \sigma(\rho)=\int_{\rho_*}^{\rho}\frac{\sqrt{E(r)}}r\,dr.}
$$

Since $\sigma'>0$, these are [isothermal coordinates](../../../../../../isothermal-coordinates.md) with a flat rescaled metric. An angular coordinate is understood on a local branch; the flat metric may equally be viewed locally as a cylinder metric. The apparent divergence of $E$ at the equator is a coordinate failure, not a singularity of the [induced metric](../../../../../../induced-metric.md). For example, $(x,\phi)$ give $g=[1+x^2/(a^2(1-x^2))]dx^2+(1-x^2)d\phi^2/a^2$, regular at $x=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
