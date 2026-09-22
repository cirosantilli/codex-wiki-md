<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use metric compatibility and a torsion-free connection. The coordinate formula for the [Lie derivative](../../../../../lie-derivative-of-a-differential-form.md) of the [metric tensor](../../../../../metric-tensor.md) is

$$
(\mathcal L_\xi g)_{ab}=\xi^c\partial_cg_{ab}+g_{cb}\partial_a\xi^c+g_{ac}\partial_b\xi^c.
$$

Substituting $\partial_ag_{bc}=\Gamma^d{}_{ab}g_{dc}+\Gamma^d{}_{ac}g_{bd}$ and collecting connection terms gives $(\mathcal L_\xi g)_{ab}=\nabla_a\xi_b+\nabla_b\xi_a$. Thus **a Killing vector obeys $\nabla_{(a}\xi_{b)}=0$**, and conversely this [Killing equation](../../../../../killing-equation.md) makes its flow preserve the metric. Its contraction gives $\nabla_a\xi^a=0$.

With the curvature convention fixed in Q1, contract the vector [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) to obtain

$$
\nabla_b\nabla_a\xi^b-\nabla_a\nabla_b\xi^b
=R^b{}_{cba}\xi^c=R_{ca}\xi^c.
$$

The second term vanishes because the Killing divergence is zero. Metric compatibility converts the first term to $\nabla^b\nabla_a\xi_b$, and the [Killing equation](../../../../../killing-equation.md) changes this to $-\nabla^b\nabla_b\xi_a$. Therefore the [second covariant derivative of a Killing vector](../../../../../second-covariant-derivative-of-a-killing-vector.md) satisfies

$$
\boxed{\nabla^b\nabla_b\xi_a+R_{ab}\xi^b=0.}
$$

This derivation fixes the sign by the stated Ricci identity rather than by an unspecified convention for curvature.

For the axial [Killing vector](../../../../../killing-vector-field.md) set $F^{ab}=\nabla^b\xi^a$. It is antisymmetric and its divergence is $\nabla_bF^{ab}=-R^a{}_b\xi^b$. Work in geometrized units $G=c=1$ and with zero cosmological constant, as required by the asymptotically flat setting. If a spatial shell $\Omega$ has oriented boundary $S_2-S_1$, the given form of [Stokes theorem](../../../../../stokes-theorem.md) applied to the [Komar angular momentum](../../../../../komar-angular-momentum.md) gives

$$
J_{S_2}-J_{S_1}
=-\frac1{8\pi}\int_\Omega\nabla_bF^{ab}\,d^3\Sigma_a
=\frac1{8\pi}\int_\Omega R^a{}_b\xi^b\,d^3\Sigma_a.
$$

The vacuum [Einstein field equations](../../../../../einstein-field-equations.md) give $R_{ab}=0$ everywhere in the shell outside the matter source. The shell can still contain [gravitational waves](../../../../../gravitational-wave.md), since those have nonzero Weyl curvature rather than a nonzero [Ricci tensor](../../../../../ricci-tensor.md). Hence

$$
\boxed{J_{S_2}=J_{S_1}.}
$$

This is [angular momentum conservation in an axisymmetric vacuum region](../../../../../angular-momentum-conservation-in-an-axisymmetric-vacuum-region.md). Moving the outer surface through the radiative region adds no angular momentum. In an exactly axisymmetric spacetime there is no outward transport of the axial angular momentum by the waves. Axisymmetry does not imply stationarity, so this conclusion does not exclude radiation of energy.

For completeness the Einstein equations express the bulk current as

$$
Y^a=R^a{}_b\xi^b=8\pi\left(T^a{}_b-\frac12T\delta^a{}_b\right)\xi^b.
$$

On an axisymmetric spacelike slice, $\xi$ is tangent to the slice and its contraction with $d^3\Sigma_a$ vanishes; there the trace contribution to the angular-momentum volume integral drops out. One must retain any inner surface charges if the integration region has inner boundaries. The vacuum shell argument itself does not require a matter-only representation of the total charge.

The current $Y$ is conserved on arbitrary slices, not just those to which $\xi$ is tangent. Indeed symmetry of the [Ricci tensor](../../../../../ricci-tensor.md) and antisymmetry of $\nabla_a\xi_b$ give

$$
\nabla_aY^a=(\nabla_aR^a{}_b)\xi^b+R^{ab}\nabla_a\xi_b
=\frac12\xi^b\nabla_bR=0.
$$

The last equality follows because a metric-preserving Killing flow also preserves the [scalar curvature](../../../../../scalar-curvature.md). Equivalently, the [stress-energy conservation](../../../../../stress-energy-conservation.md) law and invariance of the stress trace give the same conserved current.

Let two spacelike hypersurfaces terminate on large enclosing spheres $S_1,S_2$ at the same asymptotic end. Join the spheres by a timelike tube lying wholly in the vacuum exterior. On this tube $\nabla_bF^{ab}=0$, so [Stokes theorem](../../../../../stokes-theorem.md) gives zero difference of their Komar surface integrals, independently of the tube's shape. Alternatively, use the given [Gauss theorem](../../../../../divergence-theorem.md) on a spacetime volume between the slices: $\nabla_aY^a=0$, and the lateral flux is zero because $Y=0$ in the exterior vacuum tube. Taking the enclosing spheres to infinity with the usual asymptotic falloff therefore proves

$$
\boxed{J_\infty\text{ is independent of the chosen spacelike hypersurface}.}
$$

All surface orientations in these equations use the same convention as the stated Komar integral. The argument concerns enclosing surfaces at the same asymptotic end, so it does not discard additional charges from other ends or inner boundaries.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
