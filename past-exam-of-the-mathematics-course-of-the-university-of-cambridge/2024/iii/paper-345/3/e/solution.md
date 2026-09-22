<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let

$$
g'_H=\frac{g(\rho_1-\rho_H)}{\rho_0},
\qquad
g'_L=\frac{g(\rho_1-\rho_L)}{\rho_0}.
$$

The global steady heat, or [buoyancy flux](../../../../../../buoyancy-flux.md), balance equates the floor-source input to the buoyancy carried out by the one-way upper-layer exhaust:

$$
B=Q_Vg'_H.
$$

The corresponding upper-to-lower density jump is fixed by the warm plume crossing the interface,

$$
B=Q_B(h)(g'_H-g'_L).
$$

The first balance also shows that the descending cold plume has buoyancy-flux magnitude per unit wall length

$$
\mathcal B=\frac{Q_Vg'_H}{L}=\frac BL.
$$

At a steady interface, the upward axisymmetric-plume volume flux equals the total downward wall-plume volume flux. Using parts (c) and (d),

$$
C_PB^{1/3}h^{5/3}
=L\alpha(z_o-h)
\left(\frac{B}{\alpha L}\right)^{1/3}.
$$

After cancellation of $B^{1/3}$, the required implicit geometric relation is

$$
\boxed{
C_Ph^{5/3}
=\alpha^{2/3}L^{2/3}(z_o-h),
\qquad
z_o=z_V+\frac{H'}{2\alpha}
}.
$$

Thus the ideal steady interface fraction is independent of the source strength: increasing $B$ multiplies both opposing plume volume fluxes by $B^{1/3}$. The floor area $A$ and room height $H$ affect the transient filling time and admissibility of the assumed ordering, but not this steady integral balance, provided $0<h<z_V$ and the plumes remain separated.

Set

$$
K_V=\frac{C_d}{3}LH'^{3/2}.
$$

Combining the [single-opening exchange flow](../../../../../../single-opening-exchange-flow.md) relation $Q_V=K_V\sqrt{g'_H}$ with $B=Q_Vg'_H$ gives

$$
\boxed{
Q_V=(K_V^2B)^{1/3}
=\left(\frac{C_d^2L^2H'^3B}{9}\right)^{1/3}
}.
$$

It also gives $g'_H=(B/K_V)^{2/3}$, after which the second density balance determines $g'_L$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
