<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $h=2k_c$ and $D=d/dz$. Taking the [divergence](../../../../../../divergence.md) of the [Stokes flow](../../../../../../stokes-flow-split.md) momentum equation gives $\nabla^2P=R\theta_z$; applying the [Laplacian](../../../../../../laplacian.md) to its vertical component then eliminates [pressure](../../../../../../pressure.md) and gives $\nabla^4w=-R\theta_{xx}$. The forced [velocity](../../../../../../velocity.md) and [temperature](../../../../../../temperature.md) are $O(\epsilon^2)$, so their [advection](../../../../../../advection.md) product is $O(\epsilon^4)$ and drops out at leading order. The steady [heat equation](../../../../../../heat-equation.md) reduces to $w_0+\nabla^2\theta_0=0$.

Consequently the [boundary value problem](../../../../../../boundary-value-problem.md) for the forced profiles is

$$
\boxed{(D^2-h^2)^2w_\epsilon=R h^2\theta_\epsilon,\qquad (D^2-h^2)\theta_\epsilon=-w_\epsilon.}
$$

Its six [boundary conditions](../../../../../../boundary-condition.md) are

$$
\boxed{w_\epsilon(0)=w_\epsilon(1)=w_\epsilon''(0)=w_\epsilon''(1)=0,\qquad \theta_\epsilon(0)=\gamma,\quad\theta_\epsilon(1)=0.}
$$

The horizontal [velocity field](../../../../../../velocity-field.md) is $u_0=-\epsilon^2w_\epsilon'(z)\sin(hx)/h$, which directly verifies the [incompressible flow](../../../../../../incompressible-flow.md) and [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md). In the detuning used subsequently, $R$ may be replaced by $R_c$ in this leading problem, since its correction enters at order $\epsilon^4$. The vertical profiles depend linearly on $\gamma$.

For reference, the unforced [free-slip convection neutral curve](../../../../../../free-slip-convection-neutral-curve.md) is $R_0(k)=(k^2+\pi^2)^3/k^2$, with $k_c=\pi/\sqrt2$ and $R_c=27\pi^4/4$. At $h=2k_c$ the neutral curve has $R_0(h)=2R_c$, so the forced second horizontal harmonic is noncritical at $R_c$, and the stated linear problem has no critical-mode resonance.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
