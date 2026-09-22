<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Use the ideal steady incompressible-flow model, neglecting height change across the smooth nozzle. [Flow conservation](../../../../../flow-conservation.md) gives inlet and outlet speeds $u_0=Q/A_0$ and $u_1=Q/A_1$. Set atmospheric pressure to zero. The [Bernoulli equation](../../../../../bernoulli-equation.md) between inlet and outlet gives

$$
\boxed{p_0=\frac\rho2(u_1^2-u_0^2)=\frac{\rho Q^2}{2}\left(\frac1{A_1^2}-\frac1{A_0^2}\right).}
$$

Choose a control volume containing the fluid in the nozzle, with the positive axis pointing toward the outlet. The [integral momentum equation](../../../../../integral-momentum-equation.md) gives

$$
p_0A_0+F_{\mathrm{wall\ on\ fluid}}=\rho Q(u_1-u_0).
$$

Thus the fluid's force on the nozzle is $p_0A_0-\rho Q(u_1-u_0)$, in the outlet direction. Substitute the pressure and velocities:

$$
\begin{aligned}
F_{\mathrm{fluid\ on\ nozzle}}
&=\rho Q^2\left[\frac{A_0}{2A_1^2}-\frac1{A_1}+\frac1{2A_0}\right]\\
&=\frac{\rho Q^2}{2A_0}\left(\frac{A_0}{A_1}-1\right)^2.
\end{aligned}
$$

The fireman's holding force is equal and opposite. Therefore **the required force points upstream and has magnitude**

$$
\boxed{F=\frac{\rho Q^2}{2A_0}\left(\frac{A_0}{A_1}-1\right)^2.}
$$

This is the [holding force on a contracting nozzle](../../../../../holding-force-on-a-contracting-nozzle.md); retaining the inlet pressure force is essential to its sign and value.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
