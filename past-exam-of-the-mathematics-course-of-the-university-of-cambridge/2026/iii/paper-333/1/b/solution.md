<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Initially $\zeta=0$, so conservation of the linear [potential vorticity](../../../../../../potential-vorticity.md) gives

$$
\zeta_f-\frac f{H_0}\eta_f
=-\frac f{H_0}\eta_i.
$$

The final flow is in [geostrophic balance](../../../../../../geostrophic-balance.md), hence

$$
\zeta_f=\frac gf\nabla^2\eta_f.
$$

Consequently the adjusted height solves the modified Helmholtz equation

$$
\boxed{
\left(\nabla^2-\frac1{L_R^2}\right)\eta_f
=-\frac{\eta_i}{L_R^2}},
\qquad
\boxed{L_R=\frac{\sqrt{gH_0}}{|f|}},
$$

where $L_R$ is the [Rossby deformation radius](../../../../../../rossby-deformation-radius.md).

The initial condition is independent of $x$ and odd in $y$. The bounded solution that is continuously differentiable at $y=0$ is

$$
\boxed{
\eta_f(y)=\eta_0\operatorname{sgn}(y)
\left(1-e^{-|y|/L_R}\right)}.
$$

It gives

$$
\boxed{
u_f(y)=-\frac{g\eta_0}{fL_R}e^{-|y|/L_R}},
\qquad
\boxed{v_f=0}.
$$

During [geostrophic adjustment](../../../../../../geostrophic-adjustment.md), the part of the initial energy incompatible with the conserved potential-vorticity distribution radiates away as [inertia-gravity waves](../../../../../../inertia-gravity-wave.md). The remaining current has width $O(L_R)$ and is geostrophically balanced.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
