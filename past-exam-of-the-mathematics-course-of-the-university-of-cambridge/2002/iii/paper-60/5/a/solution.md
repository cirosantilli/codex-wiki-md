<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=\Delta x$, $k=\Delta t=\mu h$. Every smooth exact solution of the [advection equation](../../../../../../transport-equation.md) here is $u(x,t)=F(x+t)$. At $s=x+t$, substitution into the scheme gives the unscaled residual

$$
\mathcal R=F(s+\mu h)-(1-2\mu)[F(s)-F(s+h)]-F(s+(1-\mu)h).
$$

The constant, linear and quadratic Taylor coefficients vanish. Its cubic coefficient is

$$
\frac{h^3}{6}\{\mu^3+1-2\mu-(1-\mu)^3\}F'''(s)
=\frac{\mu(1-\mu)(1-2\mu)}6h^3u_{xxx}.
$$

For a general smooth function the first-order residual is $2k(u_t-u_x)$, so the proper normalized [local truncation error](../../../../../../local-truncation-error.md) on an exact solution is

$$
\boxed{\frac{\mathcal R}{2k}=\frac{(1-\mu)(1-2\mu)}{12}h^2u_{xxx}+O(h^3).}
$$

Hence **the scheme has formal order two for fixed general positive $\mu$**. At $\mu=1/2$ and $\mu=1$, the displayed residual vanishes identically for every $F$, not just to one higher Taylor order: the recurrence transports exactly sampled characteristics when both starting levels are compatible with the exact solution. This formal exactness does not imply [stability](../../../../../../stability-of-a-numerical-method.md). At $\mu=0$ there is no positive time step. The two-level recurrence also requires a starting procedure for $U^1$; one initial solution profile alone is not two independent starting levels.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
