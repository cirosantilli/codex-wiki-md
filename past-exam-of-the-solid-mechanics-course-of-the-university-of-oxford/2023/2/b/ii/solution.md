<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $W_r,W_\theta,W_\phi$ denote derivatives of the [strain energy density](../../../../../strain-energy-density.md) with respect to its three [principal stretches](../../../../../principal-stretch.md). The [principal stress formula for incompressible hyperelasticity](../../../../../principal-stress-formula-for-incompressible-hyperelasticity.md) is

$$
t_r=\lambda_rW_r-p,\qquad
t_\theta=\lambda_\theta W_\theta-p,\qquad
t_\phi=\lambda_\phi W_\phi-p.
$$

It follows by applying $\mathbf T=\mathbf F(\partial_{\mathbf F}W)^T-p\mathbf1$ in principal axes. Equal tangential [principal stretches](../../../../../principal-stretch.md) and [material isotropy](../../../../../material-isotropy.md) give $W_\theta=W_\phi$ at $(\lambda^{-2},\lambda,\lambda)$. Differentiating the reduced [strain energy density](../../../../../strain-energy-density.md) by the [chain rule](../../../../../chain-rule.md) gives

$$
\begin{aligned}
h'(\lambda)&=-2\lambda^{-3}W_r+W_\theta+W_\phi\\
&=2\left(W_\theta-\lambda^{-3}W_r\right)
=\frac2\lambda(t_\theta-t_r).
\end{aligned}
$$

The unknown [pressure](../../../../../pressure-split.md) cancels in this difference. Substituting in part (i), and then using the supplied derivative of $\lambda$, gives

$$
\frac{dt_r}{dr}=\frac{\lambda h'(\lambda)}r=\frac{h'(\lambda)}R,
\qquad
\frac{d\lambda}{dr}=\frac{1-\lambda^3}{R}.
$$

Consequently the desired [ordinary differential equation](../../../../../ordinary-differential-equation.md) is

$$
\boxed{\frac{dt_r}{d\lambda}=\frac{h'(\lambda)}{1-\lambda^3}.}
$$

For completeness, the supplied derivative follows from $R^3=r^3-(a^3-A^3)$: $dR/dr=r^2/R^2=\lambda^2$, and differentiating $\lambda=r/R$ gives $(1-\lambda^3)/R$. At the undeformed value $\lambda=1$ the division must be interpreted by a limit; the [spherically symmetric deformation](../../../../../spherically-symmetric-deformation.md) with $a=A$ has $\lambda\equiv1$ and should be handled directly by the radial equilibrium equation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
