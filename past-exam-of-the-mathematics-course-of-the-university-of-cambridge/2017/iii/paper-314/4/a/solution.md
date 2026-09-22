<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the free surface be at $r=R_1$ and take the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) to vanish at infinity. [Mass conservation](../../../../../../mass-conservation.md) fixes $R_1=(3M_1/(4\pi\rho_1))^{1/3}$. The enclosed mass is $m(r)=4\pi\rho_1r^3/3$, and [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) requires $dp_0/dr=-\rho_1Gm(r)/r^2$. With vacuum outside, $p_0(R_1)=0$, giving

$$
\boxed{p_0(r)=\frac{2\pi G\rho_1^2}{3}(R_1^2-r^2),\qquad
\Phi_0(r)=
\begin{cases}
-\dfrac{GM_1}{2R_1}\left(3-\dfrac{r^2}{R_1^2}\right),&r\leq R_1,\\
-\dfrac{GM_1}{r},&r\geq R_1.
\end{cases}}
$$

The [pressure](../../../../../../pressure.md) is zero outside. A prescribed constant external [pressure](../../../../../../pressure.md) would simply add that constant to $p_0$.

The bulk [Eulerian and Lagrangian fluid perturbations](../../../../../../eulerian-and-lagrangian-fluid-perturbations.md) obey $\delta\rho=0$ because the [mass density](../../../../../../density.md) is uniform and the [Lagrangian displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) has zero [divergence](../../../../../../divergence.md). The linearized [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) in the interior is

$$
-\omega^2\boldsymbol\xi=-\nabla\left(\frac{\delta p}{\rho_1}+\delta\Phi\right).
$$

Taking the [curl](../../../../../../curl.md) gives $\omega^2\nabla\times\boldsymbol\xi=0$. Thus every nonzero-frequency [normal mode](../../../../../../normal-mode.md) has an [irrotational flow](../../../../../../irrotational-flow.md) displacement; the [simply connected space](../../../../../../simply-connected-space.md) formed by the interior admits $\boldsymbol\xi=\nabla U$ and [incompressibility](../../../../../../incompressible-flow.md) gives the [Laplace equation](../../../../../../laplace-equation.md) $\nabla^2U=0$. For a regular center, one [spherical harmonic](../../../../../../spherical-harmonic.md) component is $U=A_l r^lY_l^m$, with $|m|\leq l$.

It is essential to retain the [surface gravity perturbation of a uniform-density sphere](../../../../../../surface-gravity-perturbation-of-a-uniform-density-sphere.md). Although the bulk [mass density](../../../../../../density.md) perturbation is zero, the displaced density discontinuity gives

$$
\delta\rho=\rho_1\xi_r(R_1)\delta(r-R_1),\qquad
\xi_r(R_1)=lA_lR_1^{l-1}Y_l^m.
$$

The [Poisson equation](../../../../../../poisson-equation.md) implies that $\delta\Phi$ is continuous and its outward radial derivative has the jump

$$
\left[\partial_r\delta\Phi\right]_{\mathrm{out}-\mathrm{in}}=4\pi G\rho_1\xi_r(R_1).
$$

Using regularity at the center and decay at infinity, write

$$
\delta\Phi_{\mathrm{in}}=C_l r^lY_l^m,\qquad
\delta\Phi_{\mathrm{out}}=C_l R_1^{2l+1}r^{-l-1}Y_l^m.
$$

The derivative jump is $-(2l+1)C_lR_1^{l-1}Y_l^m$, so $C_l=-4\pi G\rho_1lA_l/(2l+1)$.

Integrating the bulk [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) gives $\delta p/\rho_1=\omega^2U-\delta\Phi$ for $l\geq1$. At the free surface the [Lagrangian pressure perturbation](../../../../../../lagrangian-pressure-perturbation.md) vanishes:

$$
0=\delta p+\xi_r p_0'(R_1),\qquad
\frac{\delta p}{\rho_1}=\frac{GM_1}{R_1^2}\xi_r.
$$

Combining these relations yields the [Kelvin stellar mode](../../../../../../kelvin-stellar-mode.md) frequency

$$
\omega_l^2=l\frac{GM_1}{R_1^3}-\frac{4\pi G\rho_1l}{2l+1}
=\boxed{\frac{2l(l-1)}{2l+1}\frac{GM_1}{R_1^3}},\qquad l\geq1.
$$

The $2l+1$ choices of $m$ are degenerate because of [spherical symmetry](../../../../../../spherical-symmetry.md). For $l=1$, $rY_1^m$ is a [linear combination](../../../../../../linear-combination.md) of coordinates in a [Cartesian coordinate system](../../../../../../cartesian-coordinate-system.md), so $\nabla U$ is a constant [displacement](../../../../../../displacement.md): **the zero frequency is rigid translation of the whole isolated body**. Such a translation has no restoring force. The constant $l=0$ potential generates no displacement; a radial breathing motion is excluded by [incompressibility](../../../../../../incompressible-flow.md) and a regular center.

The printed irrotational assertion needs the nonzero-frequency qualification, or restriction to the potential [incompressible stellar surface modes](../../../../../../incompressible-stellar-surface-mode.md). It is false for all neutral displacements: $\boldsymbol\xi=\boldsymbol\Omega\times\mathbf r$ has zero [divergence](../../../../../../divergence.md), zero normal displacement at the surface, and $\delta p=\delta\Phi=0$, so it is a zero-frequency displacement, but $\nabla\times\boldsymbol\xi=2\boldsymbol\Omega\ne0$. This does not change the [Kelvin stellar mode](../../../../../../kelvin-stellar-mode.md) spectrum just derived.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
