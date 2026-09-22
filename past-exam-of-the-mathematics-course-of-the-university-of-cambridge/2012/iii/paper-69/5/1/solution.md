<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the endpoint values $u_0=u_M=0$ and evolve the interior indices $1,\ldots,M-1$. This matches $\Delta x=1/M$ on $[0,1]$. If the printed upper index $m=M$ is retained, the odd ghost extension $u_{M+1}=-u_{M-1}$ makes its boundary equation identically compatible; it does not add an interior unknown.

Writing $h=\Delta x$ and $\tau=\Delta t$, this is the [theta method](../../../../../../theta-method.md) with parameter $a$:

$$
\frac{U^{n+1}-U^n}{\tau}=aD_{xx}U^{n+1}+(1-a)D_{xx}U^n.
$$

For a smooth exact heat solution, its normalized residual at $t_n$ is

$$
\mathcal R=(\tfrac12-a)\tau u_{xxxx}-\frac{h^2}{12}u_{xxxx}
 +O(\tau^2+\tau h^2+h^4).
$$

Thus the generic consistency orders are **first in time and second in space for $a\ne1/2$**, and **second in both time and space for $a=1/2$**, the [Crank-Nicolson method](../../../../../../crank-nicolson-method.md). These are independent-step orders. Along the special parabolic refinement $\tau=\mu h^2$, the leading combined residual cancels if $a=1/2-1/(12\mu)$, giving a higher combined smooth-data order; it does not change the generic temporal order at independently varied meshes.

The given [L2 initial condition](../../../../../../l2-initial-condition.md) need not have pointwise values or four derivatives. Initialize by a bounded cell-average or projection operator, as in [L2-compatible initialization of grid data](../../../../../../l2-compatible-initialization-of-grid-data.md). The Taylor estimate applies to smooth data or sufficiently positive times after heat smoothing, rather than an unqualified uniform high-order estimate at the initial instant for arbitrary rough data. Stability and convergence for rough data are distinct from this consistency order.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [5](../../5.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
