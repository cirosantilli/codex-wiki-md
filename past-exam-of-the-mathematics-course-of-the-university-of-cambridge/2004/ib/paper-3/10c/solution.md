<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

For velocity $\mathbf u=\nabla\phi$ and a conservative body force $-\nabla\chi$, the unsteady [Bernoulli equation](../../../../../bernoulli-equation.md) is

$$
\boxed{\phi_t+\frac12|\nabla\phi|^2+\frac p\rho+\chi=C(t).}
$$

It follows by integrating the inviscid [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) in space; a purely time-dependent potential gauge can absorb $C(t)$.

Use a coordinate along the thin U-tube from the left surface to the right, and let the right surface rise by $\zeta$ while the left falls by $\zeta$. [Incompressibility](../../../../../incompressible-flow.md) and uniform area give velocity $\dot\zeta$ along the whole fluid column. If its total length is $L$, the velocity-potential difference between the surfaces is $L\dot\zeta$; the column length stays constant as their displacements cancel. Both surfaces have atmospheric pressure and the same speed. Subtracting their Bernoulli balances, with $\chi=gy$, therefore yields

$$
L\ddot\zeta+2g\zeta=0.
$$

In the long-leg approximation underlying the requested formula, the base bend contributes negligible length and $L=2h$. Consequently

$$
\boxed{h\ddot\zeta+g\zeta=0,\qquad\omega=\sqrt{g/h}.}
$$

If the horizontal connector or bend has nonnegligible length, it belongs in $L$ and the general frequency is $\sqrt{2g/L}$; the stated height alone would then not determine the inertia.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
