<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Orient both [spheres](../../../../../sphere.md) in the standard way and normalize their [area forms](../../../../../area-form.md) to total area $4\pi$. The [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) can be obtained in two ways. For a [regular value](../../../../../regular-value.md) $y$, use the [degree as a sum of local degrees](../../../../../degree-as-a-sum-of-local-degrees.md):

$$
\boxed{\deg g=\sum_{x\in g^{-1}(y)}\operatorname{sign}\det Dg_x.}
$$

Each inverse image is isolated by the [inverse function theorem](../../../../../inverse-function-theorem.md), and compactness makes the set finite. The determinant is computed in consistently oriented local coordinates. A second method is [spherical degree by area pullback](../../../../../spherical-degree-by-area-pullback.md):

$$
\boxed{\deg g=\frac1{4\pi}\int_{S^2}g^*\omega
=\frac1{4\pi}\int_0^{2\pi}\!\int_0^\pi
g\cdot(\partial_\theta g\times\partial_\varphi g)\,d\theta\,d\varphi,}
$$

where the last formula represents $g$ as a unit vector in $\mathbb R^3$. The [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) already contains the signed [Jacobian determinant](../../../../../jacobian-determinant.md); no extra $\sin\theta$ is to be inserted in that last coordinate expression.

To relate the methods, replace $\omega$ by a smooth top-degree [differential form](../../../../../differential-form-split.md) with the same total integral supported in a small neighbourhood of a [regular value](../../../../../regular-value.md). Two such top-degree forms with equal integral differ by an [exact differential form](../../../../../exact-differential-form.md) on $S^2$, by its top-degree [de Rham cohomology](../../../../../de-rham-cohomology.md). Their pullbacks therefore have the same integral by [Stokes theorem](../../../../../stokes-theorem.md). Over the chosen neighbourhood, $g$ splits into local inverse branches; the [change of variables formula](../../../../../change-of-variables-formula.md) makes the contribution of each branch its [orientation](../../../../../orientation-of-a-simplex.md) sign times $4\pi$. Their sum is precisely the first formula. Thus the area integral is an integer and agrees with the signed inverse-image count.

For a nonconstant [rational map](../../../../../rational-map-complex-analysis.md), first use [common-factor reduction of a rational map](../../../../../common-factor-reduction-of-a-rational-map.md) so $p$ and $q$ are coprime. Write $k=\max(\deg p,\deg q)$ for these reduced polynomials. A generic finite target value $w$ has inverse images at the roots of $p-wq$: avoiding exceptional values makes its degree $k$ and its roots simple. The [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) supplies $k$ roots. A [holomorphic map](../../../../../holomorphic-map.md) has positive real [Jacobian determinant](../../../../../jacobian-determinant.md) $|R'|^2$ at a regular point, so every local sign is $+1$. **Hence**

$$
\boxed{\deg R=k\quad\text{for a coprime representation}.}
$$

The source leaves coprimality implicit. In an unreduced representation the answer is $\max(\deg p,\deg q)-\deg\gcd(p,q)$, including degree zero for a constant reduced map. For example $(z^2-1)/(z-1)$ extends to $z+1$ and has degree one, although the unreduced maximum degree is two. Exceptional inverse images at infinity or multiple roots do not change the [degree of a rational map of the Riemann sphere](../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md).

For the [rational map approximation for Skyrmions](../../../../../rational-map-approximation-for-skyrmions.md), use [stereographic projection](../../../../../stereographic-projection.md) $z=\tan(\theta/2)e^{i\varphi}$ and the unit target vector

$$
\mathbf n_R=\frac{(2\operatorname{Re}R,\,2\operatorname{Im}R,\,1-|R|^2)}{1+|R|^2}.
$$

Combine this [rational map](../../../../../rational-map-complex-analysis.md) with a radial profile to form a [special unitary group](../../../../../special-unitary-group.md) field:

$$
U(r,z)=\cos f(r)\,\mathbf1+i\sin f(r)\,\mathbf n_R(z)\cdot\boldsymbol\sigma,
\qquad f(0)=\pi,\quad f(\infty)=0,
$$

where $\boldsymbol\sigma$ are the [Pauli matrices](../../../../../pauli-matrices.md). The endpoint values make $U(0)=-\mathbf1$ independent of angle and $U(\infty)=\mathbf1$. Appropriate radial behaviour gives an admissible [finite-energy field configuration](../../../../../finite-energy-field-configuration.md). With $L_i=U^\dagger\partial_iU$, choose the [topological baryon number in the Skyrme model](../../../../../topological-baryon-number-in-the-skyrme-model.md) convention

$$
B=-\frac1{24\pi^2}\int\epsilon_{ijk}\operatorname{tr}(L_iL_jL_k)\,d^3x.
$$

Separating the radial and angular factors gives

$$
\boxed{B=-\frac{2k}{\pi}\int_0^\infty f'(r)\sin^2f(r)\,dr=k.}
$$

Thus the [degree of a rational map of the Riemann sphere](../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md) supplies the [Skyrmion](../../../../../skyrmion.md) charge.

In conventional dimensionless massless [Skyrme model](../../../../../skyrme-model.md) units, its static energy reduces to

$$
E=4\pi\int_0^\infty\left[r^2f'^2+2k(1+f'^2)\sin^2f+\mathcal I[R]\frac{\sin^4f}{r^2}\right]dr,
\qquad\mathcal I[R]=\frac1{4\pi}\int_{S^2}J_R^2\,d\Omega,
$$

with the [angular Jacobian of a rational map](../../../../../angular-jacobian-of-a-rational-map.md)

$$
J_R=\left[\frac{1+|z|^2}{1+|R|^2}|R'|\right]^2,
\qquad\frac1{4\pi}\int J_R\,d\Omega=k.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\mathcal I\geq k^2$. These formulas follow from the radial strain $|f'|$ and the two equal angular strains $\sin f\sqrt{J_R}/r$: the quadratic energy sums their squares and the quartic [Skyrme term](../../../../../skyrme-term.md) sums their pairwise products of squares. Minimize the [angular integral in the rational map approximation](../../../../../angular-integral-in-the-rational-map-approximation.md) over degree-$k$ maps, then minimize the remaining radial energy with the stated endpoints. This replaces a three-dimensional field minimization by finitely many map coefficients and an [ordinary differential equation](../../../../../ordinary-differential-equation.md) for $f$.

**The method constructs a charge-$k$ variational approximation**, with topology built in and with [rotational symmetry of a rational map](../../../../../rotational-symmetry-of-a-rational-map.md) translated into combined spatial and [isospin rotations](../../../../../isorotation.md). It is efficient for identifying shapes and providing initial data for unrestricted numerical relaxation. Its restrictions are equally concrete: it uses one radial profile and a holomorphic angular map independent of radius, so it cannot represent arbitrary radial-angular correlations, separated clusters, or all deformations. Apart from the degree-one [Skyrmion hedgehog ansatz](../../../../../skyrmion-hedgehog-ansatz.md), it generally does not solve the full field equation exactly. Massive-pion terms can be included in the radial functional but do not remove these restrictions, and multi-shell or unrestricted fields may be needed for larger charges. Approximate energy minima and a final [collective-coordinate quantization](../../../../../collective-coordinate-quantization.md) are distinct steps.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
