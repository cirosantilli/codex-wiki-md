<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use small [Rossby number](../../../../../../rossby-number.md) $U/(f_0l)\ll1$, slow evolution on the advective time scale, small interface displacements relative to each layer depth, shallow hydrostatic layers, stable [reduced gravity](../../../../../../reduced-gravity-split.md) $g'>0$, and inviscid unforced flow. On a [beta plane](../../../../../../beta-plane.md), take $\beta l/f_0$ of the same small order as the [Rossby number](../../../../../../rossby-number.md). The internal [Burger number](../../../../../../burger-number.md) is retained at order unity so stratification and relative-vorticity effects can both enter the leading potential-vorticity anomaly.

The [rigid-lid pressure in two-layer flow](../../../../../../rigid-lid-pressure-in-two-layer-flow.md) comes from neglecting the free-surface volume displacement in the [rigid-lid approximation](../../../../../../rigid-lid-approximation.md); it does not permit setting the common horizontal pressure gradient to zero. The small surface displacement multiplied by $g$ retains a finite lid-pressure multiplier. Write $h_1=H_1+\chi$, $h_2=H_2-\chi$, and let $\Pi$ denote this common pressure potential. Leading [geostrophic balance](../../../../../../geostrophic-balance.md) gives

$$
f_0\psi_1=\Pi,\qquad f_0\psi_2=\Pi-g'\chi,\qquad
\boxed{\chi=\frac{f_0}{g'}(\psi_1-\psi_2),}
$$

with $\mathbf u_i=(-\psi_{iy},\psi_{ix})$ at leading order. Literally setting $h_1+h_2$ to a spatial constant in the momentum gradients before taking the rigid-lid limit would suppress the upper-layer pressure field and fail to produce general two-layer QG dynamics.

Taking curl of each shallow-water momentum equation and using layer continuity gives material conservation of $(f+\zeta_i)/h_i$. Expanding it to first order and advecting the anomaly by the leading geostrophic velocity yields

$$
\boxed{q_1=\nabla_h^2\psi_1+F_1(\psi_2-\psi_1)+\beta y,\qquad
q_2=\nabla_h^2\psi_2+F_2(\psi_1-\psi_2)+\beta y,\qquad
F_i=\frac{f_0^2}{g'H_i}.}
$$

The [two-layer quasi-geostrophic potential vorticity](../../../../../../two-layer-quasi-geostrophic-potential-vorticity.md) equations are

$$
\boxed{\partial_tq_i+J(\psi_i,q_i)=0,\qquad
J(A,B)=A_xB_y-A_yB_x,\quad i=1,2.}
$$

Here the common background $f_0/H_i$ has been removed and the anomaly multiplied by $H_i$. The advection term is retained at the same slow order as the time derivative even though the leading velocity/pressure balance was linear geostrophy. On an $f$ plane simply set $\beta=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
