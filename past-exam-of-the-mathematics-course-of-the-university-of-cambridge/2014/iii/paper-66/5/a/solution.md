<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a smooth exact solution of the [advection equation](../../../../../../transport-equation.md), $u(x,t)=g(x+t)$, since the transport velocity in the convention $u_t=u_x$ is minus one. Put $d=\Delta x$, $k=\mu d$ and move the scheme's right side to the left. Substitution gives the exact-solution residual

$$
\mathcal R=g(s+k)-g(s+d-k)
-(2\mu-1)[g(s+d)-g(s)],\qquad s=x+t.
$$

Its constant, linear and quadratic [Taylor expansion](../../../../../../taylor-expansion.md) terms cancel. The cubic term is

$$
\mathcal R
=\frac{d^3}{6}\mu(2\mu-1)(\mu-1)g^{(3)}(s)+O(d^4).
$$

The un-substituted leading term is $2k(u_t-u_x)$, so divide by $2k$ to use a normalized [local truncation error](../../../../../../local-truncation-error.md). For a fixed positive Courant ratio,

$$
\boxed{\frac{\mathcal R}{2k}
=\frac{d^2}{12}(2\mu-1)(\mu-1)u_{xxx}+O(d^3).}
$$

Thus **the generic method is second order**, provided stability and a compatible second-order starter are supplied.

There are two special ratios rather than an unnoticed higher generic order. At $\mu=1/2$, the scheme is $u_m^{n+1}=u_{m+1}^{n-1}$; both sides lie on the same exact characteristic, and the residual vanishes identically. At $\mu=1$ the previous-level term cancels the unshifted current term for exact data, again producing zero residual on every exact characteristic solution. The first special case is stable, while the second is not stable for arbitrary two-level perturbations, as part (b) shows. **Exact propagation of specially initialized data is not a substitute for stability.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
