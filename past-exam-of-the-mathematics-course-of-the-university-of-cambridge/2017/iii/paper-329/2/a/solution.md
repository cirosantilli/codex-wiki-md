<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $z$ positive downwards. The leading axial [velocity](../../../../../../velocity.md) of a [slender viscous thread](../../../../../../slender-viscous-thread.md) is independent of radius. [Incompressible flow](../../../../../../incompressible-flow.md) then gives $u_r=-rw'/2$, while steady [mass conservation](../../../../../../mass-conservation.md) gives $(a^2w)'=0$. The [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) has $\sigma_{rr}=-p-\mu w'$ and $\sigma_{zz}=-p+2\mu w'$. The [Young–Laplace equation](../../../../../../young-laplace-equation.md), neglecting axial curvature at slender order, gives $\sigma_{rr}=-p_e-\gamma/a$ and hence $p=p_e+\gamma/a-\mu w'$.

The axial cut transmits both the integrated [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) and the circumferential [surface tension](../../../../../../surface-tension.md). After subtracting the ambient [pressure](../../../../../../pressure.md), its tensile [force](../../../../../../force.md) is

$$
T=\pi a^2(3\mu w'-\gamma/a)+2\pi\gamma a
=3\pi\mu a^2w'+\pi\gamma a.
$$

The coefficient three is the [Trouton ratio](../../../../../../trouton-ratio.md) for axial extension. The last term is essential: the [capillary tensile force of a slender thread](../../../../../../capillary-tensile-force-of-a-slender-thread.md) is $\pi\gamma a$, not $2\pi\gamma a$, because the [capillary pressure](../../../../../../capillary-pressure.md) subtracts half the interfacial line contribution. Axial [force](../../../../../../force.md) balance is $T'+\pi\rho ga^2=0$. Together the governing equations are

$$
\boxed{(a^2w)'=0,\qquad 3\mu(a^2w')'+\rho ga^2+\gamma a'=0.}
$$

Define the [dimensionless variables](../../../../../../dimensionless-variable.md)

$$
\ell=\sqrt{\frac{\mu w_0}{\rho g}},\quad Z=\frac z\ell,\quad W=\frac w{w_0},\quad
\Gamma=\frac{\gamma\ell}{\mu a_0w_0}=\frac{\gamma}{\rho g a_0\ell}.
$$

Then $a=a_0W^{-1/2}$ and the axial equation becomes

$$
3\frac d{dZ}\left(\frac{W_Z}{W}\right)+\frac1W+\Gamma\frac d{dZ}W^{-1/2}=0.
$$

For the increasing power-law branch, all three terms have the same dependence when $\alpha=2$. Substitution leaves $1-6k^2-\Gamma k=0$. Thus

$$
\boxed{W=(1+kZ)^2,\quad \alpha=2,\quad k=\frac{\sqrt{\Gamma^2+24}-\Gamma}{12}.}
$$

This remains valid at $\Gamma=0$, when $k=1/\sqrt6$. The other root is negative and describes a decreasing local branch up to its singular endpoint, not a thread accelerating downwards indefinitely. Positive [surface tension](../../../../../../surface-tension.md) decreases $k$, so it slows the fall at a given height on this branch. Thinning reduces the capillary tensile [force](../../../../../../force.md) $\pi\gamma a$. Its negative axial derivative supplies an upward capillary [force](../../../../../../force.md) on a thread segment, balancing part of the weight. The viscous tensile [force](../../../../../../force.md) therefore supplies a smaller remaining balance; on the quadratic family this reduces the stretching rate.

The condition $W(0)=1$ alone does not select a unique solution of this second-order [ordinary differential equation](../../../../../../ordinary-differential-equation.md). The boxed power law is the requested verified branch, with tensile [force](../../../../../../force.md) tending to zero at large height; an additional nozzle tension or downstream condition is required to select it physically. The slender, negligible-inertia approximation must remain valid over the height range considered.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
