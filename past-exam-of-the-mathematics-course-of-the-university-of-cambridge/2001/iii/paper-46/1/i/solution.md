<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\sigma_v^2=\langle v(0)^2\rangle$, assumed finite. The displacement is $\Delta X(t)=\int_0^t v(s)\,ds$. By [stationarity](../../../../../../stationary-process.md), its two-time covariance is $\langle v(s)v(r)\rangle=\sigma_v^2\rho(s-r)$, with $\rho$ even for a real scalar process. Integrating over the two triangles of the square gives the [Taylor turbulent dispersion](../../../../../../taylor-turbulent-dispersion.md) identity

$$
\boxed{\langle\Delta X(t)^2\rangle=2\sigma_v^2\int_0^t(t-s)\rho(s)\,ds.}
$$

A sufficient condition for ordinary long-time variance growth is $\int_0^\infty|\rho(s)|\,ds<\infty$ with $\int_0^\infty\rho(s)\,ds>0$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) then gives

$$
\frac{\langle\Delta X(t)^2\rangle}{2t}\longrightarrow D,
\qquad \boxed{D=\sigma_v^2\int_0^\infty\rho(s)\,ds.}
$$

More generally the necessary asymptotic condition for a finite positive variance-based [diffusion coefficient](../../../../../../diffusion-coefficient.md) is convergence of $\sigma_v^2\int_0^t(1-s/t)\rho(s)\,ds$ to that coefficient. Absolute integrability is sufficient, not necessary. A zero integral does not give nondegenerate ordinary [diffusion](../../../../../../diffusion.md). Moreover a second-moment calculation alone does not establish a [normal distribution](../../../../../../normal-distribution.md) or an entire diffusive scaling limit; those require additional probabilistic assumptions.

For the specified positive [autocorrelation](../../../../../../autocorrelation.md), direct integration gives, when $\alpha\ne1,2$,

$$
\langle\Delta X^2\rangle=2\sigma_v^2\left[\frac{(1+t)^{2-\alpha}-1}{(1-\alpha)(2-\alpha)}-\frac t{1-\alpha}\right].
$$

Thus the [power-law velocity-correlation dispersion](../../../../../../power-law-velocity-correlation-dispersion.md) has the following regimes. If $\alpha>1$, the [Lagrangian integral time](../../../../../../lagrangian-integral-time.md) is $1/(\alpha-1)$ and **ordinary variance growth holds**, with $D=\sigma_v^2/(\alpha-1)$. At $\alpha=2$ the exact expression is $2\sigma_v^2[t-\log(1+t)]$. If $\alpha=1$,

$$
\langle\Delta X^2\rangle=2\sigma_v^2[(1+t)\log(1+t)-t]\sim2\sigma_v^2t\log t.
$$

For $0<\alpha<1$,

$$
\boxed{\langle\Delta X^2\rangle\sim\frac{2\sigma_v^2}{(1-\alpha)(2-\alpha)}t^{2-\alpha}.}
$$

The last two regimes spread faster than ordinary [diffusion](../../../../../../diffusion.md) and have no finite long-time [diffusion coefficient](../../../../../../diffusion-coefficient.md). Their slowly decaying velocity memory is responsible. At short times all these correlations instead give the ballistic law $\langle\Delta X^2\rangle\sim\sigma_v^2t^2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
