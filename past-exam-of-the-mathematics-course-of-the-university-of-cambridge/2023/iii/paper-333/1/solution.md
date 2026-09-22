<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume a small [Rossby number](../../../../../rossby-number.md), a [beta plane](../../../../../beta-plane.md), and small fractional changes

$$
\frac{|\beta y|}{f_0},\quad
\frac{|\zeta|}{f_0},\quad
\frac{|h_b|}{H_0},\quad
\frac{|\eta|}{H_0}\ll1.
$$

At leading order, [geostrophic balance](../../../../../geostrophic-balance.md) gives

$$
\mathbf u_g=(-\psi_y,\psi_x),
\qquad
\zeta=\nabla^2\psi,
\qquad
\eta=\frac{f_0}{g}\psi.
$$

Expanding the reciprocal depth in the [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) gives

$$
q=\frac{f_0+\beta y+\zeta}{H_0-h_b+\eta}
\simeq\frac{f_0}{H_0}
\left(1+\frac{\beta y}{f_0}
+\frac{\nabla^2\psi}{f_0}
+\frac{h_b}{H_0}
-\frac{f_0\psi}{gH_0}
\right).
$$

This is the stated [shallow-water quasi-geostrophic potential vorticity](../../../../../shallow-water-quasi-geostrophic-potential-vorticity.md) $P_g$. The term $\nabla^2\psi$ is the parcel's relative vorticity, while $-f_0^2\psi/(gH_0)=-\psi/L_D^2$ is vortex stretching caused by free-surface displacement, where

$$
L_D=\frac{\sqrt{gH_0}}{f_0}
$$

is the [barotropic deformation radius](../../../../../barotropic-deformation-radius.md).

For $h_b=\alpha y$, omit the irrelevant constant factor $f_0/H_0$. The active PV anomaly is

$$
Q=\nabla^2\psi-\frac{\psi}{L_D^2}
+\left(\beta+\frac{f_0\alpha}{H_0}\right)y.
$$

Linearizing $Q_t+J(\psi,Q)=0$ about rest and using $\psi\propto e^{i(kx+ly-\omega t)}$ gives the [Topographic Rossby-wave dispersion relation](../../../../../topographic-rossby-wave-dispersion-relation.md)

$$
\boxed{
\omega=-\frac{(\beta+f_0\alpha/H_0)k}
{k^2+l^2+L_D^{-2}}}.
$$

A northward displacement raises planetary PV when $\beta>0$ and raises topographic PV when the bottom rises northward, $\alpha>0$. PV conservation then requires anticyclonic relative vorticity, producing westward phase propagation. A negative slope opposes $\beta$ and reverses propagation when $f_0\alpha/H_0<-\beta$.

Under a rigid lid, $h=H_0-h_b$ is fixed but need not be close to $H_0$. With $q=(f+\nabla^2\psi)/h(y)$, linearization of $Dq/Dt=0$ gives

$$
\boxed{
\partial_t\nabla^2\psi
+\left(\beta-f\frac{h_y}{h}\right)\psi_x=0}.
$$

For $h=H_0e^{\gamma y}$ and over a region where $f\simeq f_0$, plane waves obey

$$
\boxed{
\omega=-\frac{(\beta-f_0\gamma)k}{k^2+l^2}}.
$$

The planetary-vorticity gradient dominates when $|\beta|\gg|f_0\gamma|$, while exponential depth variation dominates when $|f_0\gamma|\gg|\beta|$. If the variation of $f=f_0+\beta y$ across the region is retained, this is the corresponding local [WKB approximation](../../../../../wkb-approximation.md) with effective gradient $\beta-f\gamma$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
