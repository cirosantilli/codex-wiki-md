# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_311.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Use $G=c=1$, the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) with zero [cosmological constant](../../../cosmology.md#cosmological-constant), and [metric signature](../../../topology.md#metric-signature) $(-,+,+,+)$. Write $m=m_a\,dx^a$ for the [differential one-form](../../../differential-form.md#one-form) dual to the axial [Killing vector field](../../../general-relativity.md#killing-vector-field). To fix the sign of the volume formula, use the component [Hodge star operator](../../../differential-form.md#hodge-star-operator) convention $(\star j)_{abc}=\epsilon_{abcd}j^d$ and $(\star F)_{ab}=\tfrac12\epsilon_{abcd}F^{cd}$. The [Killing equation](../../../general-relativity.md#killing-equation) gives $(dm)_{ab}=2\nabla_am_b$, and its contracted curvature identity gives

$$
\nabla^b(dm)_{ab}=2R_{ab}m^b,\qquad
d\star dm=-2\star(R_{ab}m^b\,dx^a).
$$

To see the curvature step, tracing the [Killing equation](../../../general-relativity.md#killing-equation) gives $\nabla_bm^b=0$. The [second covariant derivative of a Killing vector](../../../general-relativity.md#second-covariant-derivative-of-a-killing-vector) then gives $\nabla^b\nabla_bm_a=-R_{ab}m^b$, while commuting the [covariant derivatives](../../../general-relativity.md#covariant-derivative) gives $\nabla^b\nabla_am_b=R_{ab}m^b$. Subtracting these two terms is precisely $\nabla^b(dm)_{ab}$ above. The component [Hodge star operator](../../../differential-form.md#hodge-star-operator) converts this divergence to $d\star dm$ with the displayed minus sign.

In a [vacuum spacetime](../../../general-relativity.md#vacuum-spacetime) region $R_{ab}=0$, so $d\star dm=0$. If $S_1$ and $S_2$ are enclosing [spacelike submanifolds](../../../topology.md#spacelike-submanifold) in the same [homology class](../../../homology.md#homology-class) bounding a vacuum three-dimensional region $W$, [Stokes theorem](../../../calculus.md#stokes-theorem) yields

$$
\int_{S_2}\star dm-\int_{S_1}\star dm=\int_Wd\star dm=0.
$$

Thus **the [Komar angular momentum](../../../general-relativity.md#komar-angular-momentum) is independent of the enclosing vacuum spacelike two-manifold**, provided the surfaces have the same [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) and enclose the same sources and inner boundaries. The vacuum region need not be stationary: an axial [Killing vector field](../../../general-relativity.md#killing-vector-field) suffices.

For a regular filling [hypersurface](../../../differential-geometry.md#hypersurface) $\Sigma$ with $\partial\Sigma=S$, the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) give

$$
d\star dm=-16\pi\star\left[J'-\frac12Tm\right],\qquad
J'_a=T_{ab}m^b.
$$

The pullback of $\star m$ to $\Sigma$ vanishes because $m^a$ is tangent to $\Sigma$: the dual three-form measures the normal component, which is zero. Therefore

$$
\boxed{J=-\int_\Sigma\star J'.}
$$

This is the [stress-energy current from a Killing vector](../../../general-relativity.md#stress-energy-current-from-a-killing-vector) integrated over the slice, with the signs fixed by the stated [Hodge star operator](../../../differential-form.md#hodge-star-operator) convention.

There is a necessary boundary qualification omitted from the printed formulation. If the slice has inner boundaries $S_i$, orient them so $\partial\Sigma=S-\bigcup_iS_i$. The actual [Komar angular momentum with inner boundaries](../../../general-relativity.md#komar-angular-momentum-with-inner-boundaries) identity is

$$
J-\sum_iJ_i=-\int_\Sigma\star J',\qquad
J_i=\frac1{16\pi}\int_{S_i}\star dm.
$$

For a vacuum [Kerr black hole](../../../general-relativity.md#kerr-black-hole), $T_{ab}=0$ on the exterior slice but $J\ne0$; its horizon supplies precisely the inner boundary contribution. Thus the matter-only formula is false for arbitrary exterior slices. It is valid when a nonsingular filling with no inner boundaries exists, or when all omitted inner charges vanish. The [Komar angular momentum](../../../general-relativity.md#komar-angular-momentum) independence likewise concerns homologous surfaces in the same vacuum region, not an unrestricted comparison of differently enclosed objects.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

A [gravitational wave](../../../general-relativity.md#gravitational-wave) can propagate through a region with vanishing [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor); its gravitational field is not a matter current $T_{ab}m^b$. Nevertheless, exact [axisymmetry](../../../calculus.md#axisymmetric-vector-field) gives an axial [Killing vector field](../../../general-relativity.md#killing-vector-field), and the vacuum identity $d\star dm=0$ makes the [Komar angular momentum](../../../general-relativity.md#komar-angular-momentum) equal on enclosing [spacelike submanifolds](../../../topology.md#spacelike-submanifold) in the same [homology class](../../../homology.md#homology-class). Applying the same identity to the [spacetime](../../../special-relativity.md#spacetime) tube between surrounding [spacelike submanifolds](../../../topology.md#spacelike-submanifold) at different times gives zero net flux of this charge through the tube.

Consequently **[gravitational waves](../../../general-relativity.md#gravitational-wave) in exact [axisymmetry](../../../calculus.md#axisymmetric-vector-field) carry no net [angular momentum](../../../classical-mechanics.md#angular-momentum) about the symmetry axis**. They can still carry [energy](../../../classical-mechanics.md#energy) and decrease the total [mass](../../../classical-mechanics.md#mass). In a mode description, rotationally invariant radiative data have zero azimuthal mode number; exact [axisymmetry](../../../calculus.md#axisymmetric-vector-field) therefore excludes the axial [angular momentum](../../../classical-mechanics.md#angular-momentum) flux present in nonaxisymmetric merger radiation. This does not mean there are no [gravitational waves](../../../general-relativity.md#gravitational-wave), or that radiation cannot transport [angular momentum](../../../classical-mechanics.md#angular-momentum) when the exact symmetry is absent. The relevant conserved charge includes any horizon contributions identified in the preceding [Komar angular momentum with inner boundaries](../../../general-relativity.md#komar-angular-momentum-with-inner-boundaries) identity.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The common axial [Killing vector field](../../../general-relativity.md#killing-vector-field) fixes the same sign convention for both spins. Initial rest and alignment of the separation with the symmetry axis give no orbital [angular momentum](../../../classical-mechanics.md#angular-momentum). At large separation, the total axial charge is therefore $J_1+J_2$. Since [axisymmetric radiation carries no axial angular momentum](../../../general-relativity.md#axisymmetric-radiation-carries-no-axial-angular-momentum), all of this charge remains in the remnant after the radiation has escaped and the exterior has settled:

$$
\boxed{J_f=J_1+J_2.}
$$

Here the spins are signed quantities about the same axis, not their magnitudes. The conclusion assumes the exact [axisymmetry](../../../calculus.md#axisymmetric-vector-field) stipulated throughout the merger and no remaining exterior matter carrying [angular momentum](../../../classical-mechanics.md#angular-momentum); the final stationary vacuum remnant is a [Kerr black hole](../../../general-relativity.md#kerr-black-hole) under the usual uniqueness hypotheses.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Assume the classical [black-hole area theorem](../../../general-relativity.md#hawking-s-area-theorem) applies: the [null energy condition](../../../general-relativity.md#null-energy-condition) and the required global regularity or [strong asymptotic predictability](../../../general-relativity.md#strong-asymptotic-predictability) hypotheses hold. The disconnected initial horizon sections then give $A_f\geq A_1+A_2$. Define

$$
X=\frac{A_1+A_2}{8\pi}
=\sum_{i=1}^2\left(M_i^2+\sqrt{M_i^4-J_i^2}\right),\qquad
J_f=J_1+J_2.
$$

For any regular [Kerr black hole](../../../general-relativity.md#kerr-black-hole), $|J_i|\leq M_i^2$, so $X\geq|J_1|+|J_2|\geq|J_f|$. The [irreducible mass](../../../general-relativity.md#irreducible-mass) identity obtained by inverting the Kerr area relation is

$$
M_f^2=\frac12\left(Y+\frac{J_f^2}{Y}\right),\qquad Y=\frac{A_f}{8\pi}\geq|J_f|.
$$

Indeed, $Y=M_f^2+\sqrt{M_f^4-J_f^2}$ implies $(Y-M_f^2)^2=M_f^4-J_f^2$, which gives this expression. At fixed $J_f$, its [derivative](../../../calculus.md#derivative) with respect to $Y$ is $\tfrac12(1-J_f^2/Y^2)\geq0$ on the physical branch. Therefore the [area bound for an axisymmetric Kerr merger](../../../general-relativity.md#area-bound-for-an-axisymmetric-kerr-merger) is

$$
\boxed{E_{\mathrm{rad}}\leq M_1+M_2-
\sqrt{\frac12\left[X+\frac{(J_1+J_2)^2}{X}\right]}.}
$$

This uses the ideal limit of infinite initial separation, in which the initial total [energy](../../../classical-mechanics.md#energy) is $M_1+M_2$. At finite separation it is the initial total gravitational [energy](../../../classical-mechanics.md#energy), including binding [energy](../../../classical-mechanics.md#energy), that replaces this sum. The inequality is an upper limit, not a prediction or a guarantee of saturation; real mergers increase the horizon area.

Changing only a spin sign leaves $X$ unchanged, whereas the square of the final [angular momentum](../../../classical-mechanics.md#angular-momentum) changes. For fixed nonzero $|J_1|,|J_2|$, same-sign spins give $(|J_1|+|J_2|)^2$, and opposite signs give $(|J_1|-|J_2|)^2$. The remnant must retain more rotational [energy](../../../classical-mechanics.md#energy) in the same-sign case, so its minimum allowed [mass](../../../classical-mechanics.md#mass) is larger and the radiated-[energy](../../../classical-mechanics.md#energy) upper limit is smaller. Cancellation of opposite spins permits more of the initial rotational [energy](../../../classical-mechanics.md#energy) to be radiated while respecting the same initial total area.

For example, equal extremal initial holes have $M_1=M_2=M$ and $|J_1|=|J_2|=M^2$. Same-sign spins allow at most $(2-\sqrt2)M$, a fraction $1-1/\sqrt2$ of the initial [energy](../../../classical-mechanics.md#energy); opposite signs allow at most $M$, a fraction $1/2$. These are geometric bounds under exact [axisymmetry](../../../calculus.md#axisymmetric-vector-field), not achievable-efficiency claims.

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) is a smooth family of [null geodesics](../../../special-relativity.md#null-geodesic) filling a region without crossings there. Choose a smooth future-directed tangent $U^a$ and an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$, so

$$
U^aU_a=0,\qquad U^b\nabla_bU^a=0.
$$

The space orthogonal to $U$ is degenerate because it contains $U$ itself. To measure genuine transverse separation, introduce an auxiliary [null vector](../../../special-relativity.md#null-vector) $N^a$ with $U\cdot N=-1$ and the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector)

$$
q_{ab}=g_{ab}+U_aN_b+N_aU_b.
$$

In four dimensions $q$ has a positive-definite two-dimensional image and annihilates $U$ and $N$. The [optical tensor](../../../geodesic-congruence.md#optical-tensor) is the transverse part of the velocity [derivative](../../../calculus.md#derivative),

$$
\widehat B_{ab}=q_a{}^cq_b{}^d\nabla_dU_c.
$$

Its irreducible decomposition defines the three optical quantities:

$$
\boxed{\theta=q^{ab}\widehat B_{ab},\qquad
\widehat\sigma_{ab}=\widehat B_{(ab)}-\frac12\theta q_{ab},\qquad
\widehat\omega_{ab}=\widehat B_{[ab]}.}
$$

The [null expansion](../../../geodesic-congruence.md#null-expansion) is the fractional rate of change of a small transverse area, $\theta=d\log\delta A/d\lambda$. The symmetric trace-free [null shear](../../../geodesic-congruence.md#null-shear) distorts the shape of the transverse beam without changing its area at first order. The antisymmetric [null twist](../../../geodesic-congruence.md#null-twist), also called rotation of the congruence, describes the rotational part of its transverse deformation. These are properties of the screen quotient $U^\perp/\langle U\rangle$; the auxiliary vector chooses a convenient representative of that quotient. For an affinely parametrized [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence), the contraction constraints also give $\theta=\nabla_aU^a$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[Parallel transport](../../../fiber-bundle.md#parallel-transport) the auxiliary [null vector](../../../special-relativity.md#null-vector) $N$ and a screen basis along each generator of the [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence). This keeps the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) fixed under the corresponding transported [derivative](../../../calculus.md#derivative). Use the curvature convention $[\nabla_c,\nabla_b]V_a=-R^d{}_{acb}V_d$.

With $B_{ab}=\nabla_bU_a$, differentiation of the affine [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) gives

$$
U^c\nabla_cB_{ab}
=-(\nabla_bU^c)(\nabla_cU_a)-R^d{}_{acb}U^cU_d.
$$

Here the first term comes from commuting the [derivative](../../../calculus.md#derivative) past $U^c$, and the second from the curvature commutator. The constraints $B_{ab}U^a=B_{ab}U^b=0$ follow respectively from the null normalization and affine [geodesic equation](../../../riemannian-geometry.md#geodesic-equation). Projecting onto the screen therefore yields the optical [matrix](../../../vector-space.md#matrix) equation

$$
\frac{D\widehat B_{IJ}}{d\lambda}
=-\widehat B_{IK}\widehat B_{KJ}-\mathcal R_{IJ},\qquad
\mathcal R_{IJ}=R_{acbd}e_I^aU^ce_J^bU^d.
$$

The trace of the tidal [matrix](../../../vector-space.md#matrix) is $R_{ab}U^aU^b$; extra terms from replacing the screen trace by the [spacetime](../../../special-relativity.md#spacetime) trace vanish by curvature antisymmetry. Taking the trace gives

$$
\frac{d\theta}{d\lambda}=-\operatorname{tr}(\widehat B^2)-R_{ab}U^aU^b.
$$

Decompose the [optical tensor](../../../geodesic-congruence.md#optical-tensor) as $\widehat B=\tfrac12\theta I+\widehat\sigma+\widehat\omega$. The [null shear](../../../geodesic-congruence.md#null-shear) is symmetric and trace-free and the [null twist](../../../geodesic-congruence.md#null-twist) is antisymmetric. Their cross traces vanish, and

$$
\operatorname{tr}(\widehat B^2)
=\frac12\theta^2+\widehat\sigma^{ab}\widehat\sigma_{ab}
-\widehat\omega^{ab}\widehat\omega_{ab}.
$$

The negative sign in the last term is the identity $\operatorname{tr}(\widehat\omega^2)=-\sum_{I,J}\widehat\omega_{IJ}^2$ on the positive-definite screen. Substitution proves the four-dimensional [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation):

$$
\boxed{\frac{d\theta}{d\lambda}
=-\frac12\theta^2-\widehat\sigma^{ab}\widehat\sigma_{ab}
+\widehat\omega^{ab}\widehat\omega_{ab}-R_{ab}U^aU^b.}
$$

The coefficient is $1/(D-2)$ in $D$ [spacetime](../../../special-relativity.md#spacetime) dimensions; the factor $1/2$ here belongs to the four-dimensional congruence in this question, not the five-dimensional geometry of the next question.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) and the [null energy condition](../../../general-relativity.md#null-energy-condition) imply the [null convergence condition](../../../general-relativity.md#null-convergence-condition):

$$
R_{ab}U^aU^b=8\pi T_{ab}U^aU^b\geq0.
$$

The scalar-curvature and any [cosmological constant](../../../cosmology.md#cosmological-constant) terms vanish because $U^aU_a=0$. For generators of the [null hypersurface](../../../general-relativity.md#null-hypersurface), the supplied twist-free property gives $\widehat\omega=0$. The [null shear](../../../geodesic-congruence.md#null-shear) squared is nonnegative on the screen. Thus the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) implies

$$
\frac{d\theta}{d\lambda}\leq-\frac12\theta^2.
$$

Starting from $\theta(\lambda_0)=\theta_0<0$, the [null expansion](../../../geodesic-congruence.md#null-expansion) remains negative for as long as the regular congruence exists. Hence

$$
\frac{d}{d\lambda}\left(\frac1\theta\right)
=-\frac{\theta'}{\theta^2}\geq\frac12,\qquad
\frac1{\theta(\lambda)}\geq\frac1{\theta_0}+\frac{\lambda-\lambda_0}{2}.
$$

Before the right-hand side reaches zero, inversion of the negative quantities gives

$$
\theta(\lambda)\leq
\frac{\theta_0}{1+\frac12\theta_0(\lambda-\lambda_0)}.
$$

Since the inverse of a finite negative [null expansion](../../../geodesic-congruence.md#null-expansion) cannot be nonnegative, the regular congruence cannot continue through the proposed upper limit. The [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem) therefore gives

$$
\boxed{\lambda_{\mathrm{focus}}-\lambda_0\leq\frac2{|\theta_0|}.}
$$

Provided the [geodesic](../../../riemannian-geometry.md#geodesic) itself extends this far, the transverse area collapses and $\theta\to-\infty$ at or before this bound. An earlier end of the affine [geodesic](../../../riemannian-geometry.md#geodesic) would instead be [geodesic incompleteness](../../../riemannian-geometry.md#geodesic-incompleteness). A divergence of the [null expansion](../../../geodesic-congruence.md#null-expansion) marks a caustic or a [conjugate point to a spacelike surface](../../../geodesic-congruence.md#conjugate-point-to-a-spacelike-surface); it does not by itself establish a [curvature singularity](../../../general-relativity.md#curvature-singularity).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The relevant [Penrose singularity theorem](../../../general-relativity.md#penrose-singularity-theorem) states: a [connected](../../../geometry-and-topology.md#connected-space) time-oriented four-dimensional [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) with a noncompact [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface), a nonempty [compact](../../../topology.md#compact-space) orientable boundaryless [trapped surface](../../../general-relativity.md#trapped-surface), and the [null convergence condition](../../../general-relativity.md#null-convergence-condition) is **future null-geodesically incomplete**. Under the [Einstein field equations](../../../general-relativity.md#einstein-field-equations), the [null energy condition](../../../general-relativity.md#null-energy-condition) supplies the curvature hypothesis. A [trapped surface](../../../general-relativity.md#trapped-surface) here is spacelike and has both future normal [null expansions](../../../geodesic-congruence.md#null-expansion) strictly negative. The conclusion is an incomplete [null geodesic](../../../special-relativity.md#null-geodesic), not necessarily a divergent curvature invariant at an identifiable point.

Suppose, for contradiction, that every future [null geodesic](../../../special-relativity.md#null-geodesic) is complete. Write $S$ for the [trapped surface](../../../general-relativity.md#trapped-surface) and

$$
E^+(S)=J^+(S)\setminus I^+(S)=\partial I^+(S).
$$

The equality follows because the [causal future](../../../general-relativity.md#causal-future) of a [compact](../../../topology.md#compact-space) set is [closed](../../../topology.md#closed-set) in a [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime). This [future horismos](../../../general-relativity.md#future-horismos) is a closed [achronal boundary](../../../general-relativity.md#achronal-boundary). It is nonempty: the restriction of a Cauchy time [function](../../../function.md) to [compact](../../../topology.md#compact-space) $S$ has a minimum, and a point at that minimum cannot be chronologically preceded by another point of $S$.

Normalize the two future null normal directions along $S$ against a smooth future timelike field, fixing the affine scale continuously. Their initial [null expansions](../../../geodesic-congruence.md#null-expansion) are continuous and strictly negative. [Compactness](../../../topology.md#compact-space) of the normalized normal bundle gives a uniform $c>0$ with $\theta_\pm\leq-c$ everywhere on $S$. The preceding [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem) forces a [conjugate point to a spacelike surface](../../../geodesic-congruence.md#conjugate-point-to-a-spacelike-surface) along each normal generator within affine length $L=2/c$.

By the supplied boundary-generator result, every point of $E^+(S)$ is reached by an orthogonal future [null geodesic](../../../special-relativity.md#null-geodesic) which has no earlier conjugate point. No such boundary generator can remain on the boundary beyond its first focal point. Every point of $E^+(S)$ therefore lies in

$$
K=\left\{\exp_p(\lambda U):p\in S,\ U\text{ a normalized future null normal},\ 0\leq\lambda\leq L\right\}.
$$

The parameter set is [compact](../../../topology.md#compact-space). Future null completeness makes its [geodesic](../../../riemannian-geometry.md#geodesic) flow defined throughout this common finite interval, and smooth dependence on initial data makes its image $K$ [compact](../../../topology.md#compact-space). Since $E^+(S)$ is closed and contained in $K$, it is [compact](../../../topology.md#compact-space). This is the [compactness of the future horismos of a trapped surface](../../../general-relativity.md#compactness-of-the-future-horismos-of-a-trapped-surface) step; a merely pointwise finite bound would not suffice without [compactness](../../../topology.md#compact-space) and uniform normalization.

Choose a smooth complete timelike vector field, obtained if necessary by positive rescaling against a complete auxiliary [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Its inextendible [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) meet a chosen smooth [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) $C$ exactly once. Projection along those curves defines a [continuous map](../../../topology.md#continuous-map) $\pi_C:E^+(S)\to C$. The [achronal set](../../../general-relativity.md#achronal-set) property makes this map an [injective function](../../../algebra.md#injective-function): two boundary points on the same timelike [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) would be timelike related.

An [achronal boundary](../../../general-relativity.md#achronal-boundary) is a topological [hypersurface](../../../differential-geometry.md#hypersurface) without boundary, even at nonsmooth generator junctions; the submanifold property allowed in the question supplies this fact. Thus domain and codomain are both three-dimensional [topological manifolds](../../../topology.md#topological-manifold) without boundary. [Invariance of domain](../../../topology.md#invariance-of-domain) makes $\pi_C(E^+(S))$ [open](../../../topology.md#open-set) in $C$. [Compactness](../../../topology.md#compact-space) makes it [closed](../../../topology.md#closed-set) in the [Hausdorff space](../../../topology.md#hausdorff-space) $C$, and it is nonempty. [Connectedness](../../../geometry-and-topology.md#connected-space) of the [spacetime](../../../special-relativity.md#spacetime) gives [connectedness](../../../geometry-and-topology.md#connected-space) of $C$, so this image is all of $C$. That would make $C$ [compact](../../../topology.md#compact-space), contradicting the noncompact [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) hypothesis. The completeness assumption is false, proving the theorem.

The noncompactness hypothesis and strict trapping are essential to this version. [Global hyperbolicity](../../../general-relativity.md#globally-hyperbolic-spacetime) cannot simply be omitted in the [compactness](../../../topology.md#compact-space) and projection steps, and nonpositive initial expansion with zeros does not supply the uniform focusing bound used here.

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $q=r_0^2$ and $\eta=d\psi+\tfrac12\cos\theta\,d\phi$. Expanding the [metric tensor](../../../general-relativity.md#metric-tensor) in the stationary direction gives the useful exact identities

$$
g_{tt}=-1+\frac q{r^2},\qquad g_{t\psi}=-\frac{\alpha q}{r^2},\qquad
k=\left(-1+\frac q{r^2}\right)dt-\frac{\alpha q}{r^2}\eta.
$$

Taking the [exterior derivative](../../../differential-form.md#exterior-derivative) gives

$$
dk=\frac{2q}{r^3}dt\wedge dr
+\frac{2\alpha q}{r^3}dr\wedge\eta
+\frac{\alpha q\sin\theta}{2r^2}d\theta\wedge d\phi.
$$

The fibered form of the [metric tensor](../../../general-relativity.md#metric-tensor) has [determinant](../../../linear-algebra.md#determinant) $\det g=-r^6\sin^2\theta/16$. Its inverse components needed for the flux are

$$
g^{tt}=-\frac h f,\qquad g^{t\psi}=-\frac{h\Omega}f,\qquad g^{rr}=f.
$$

Therefore

$$
(dk)^{tr}=f\left[g^{tt}(dk)_{tr}+g^{t\psi}(dk)_{\psi r}\right]
=-\frac{2q}{r^3}h(1-\alpha\Omega)=-\frac{2q}{r^3},
$$

since $h(1-\alpha\Omega)=1$. This calculation includes the rotational mixed term; dropping it prematurely would miss the exact cancellation.

With the stipulated negative coordinate [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), $\epsilon_{tr\psi\theta\phi}=-r^3\sin\theta/4$. The pullback of the [Hodge star operator](../../../differential-form.md#hodge-star-operator) to the constant-$t,r$ three-dimensional [spacelike submanifold](../../../topology.md#spacelike-submanifold) is consequently

$$
(\star dk)_{\psi\theta\phi}=\epsilon_{\psi\theta\phi tr}(dk)^{tr}
=\frac q2\sin\theta.
$$

The coordinate ranges and standard sphere identifications give

$$
\int\star dk=\frac q2(2\pi)^2\int_0^\pi\sin\theta\,d\theta=4\pi^2q.
$$

Thus the five-dimensional [Komar mass](../../../general-relativity.md#komar-mass), in the normalization given and $G_5=1$, is

$$
\boxed{M=\frac{3\pi r_0^2}{8}.}
$$

The flux is already independent of $r$ in the vacuum region, so its limit at infinity has the same value. The negative orientation in the question is crucial for the positive sign; reversing that orientation reverses the flux.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Consider the discrete map

$$
(t,r,\psi,\theta,\phi)\longmapsto
(t,r,\psi,\pi-\theta,\,2\phi_0-\phi).
$$

It is an [isometry](../../../riemannian-geometry.md#isometry): $\cos\theta$ and $d\phi$ both change sign, leaving $\cos\theta\,d\phi$ unchanged, while $d\theta^2$ and $\sin^2\theta\,d\phi^2$ are also unchanged. A local component of its [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) is $\theta=\pi/2$, $\phi=\phi_0$.

If a [geodesic](../../../riemannian-geometry.md#geodesic) starts tangent to that component, the [isometry](../../../riemannian-geometry.md#isometry) fixes both its initial position and its initial tangent. Applying the [isometry](../../../riemannian-geometry.md#isometry) therefore gives a [geodesic](../../../riemannian-geometry.md#geodesic) with the same initial data. Uniqueness of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) makes it the same curve, so it remains in the fixed component. This proves that the selected submanifold is a [totally geodesic submanifold](../../../second-fundamental-form.md#totally-geodesic-submanifold); it has dimension three, not two. The proof continues through a horizon when expressed in regular coordinates, so coordinate singularities of the original chart do not invalidate it.

The [geodesic conserved quantities from Killing vectors](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector) associated with $\partial_\psi$ and $\partial_\phi$ are

$$
L_\psi=r^2h\left(\dot\psi+\frac12\cos\theta\,\dot\phi-\Omega\dot t\right),\qquad
L_\phi=\frac12\cos\theta\,L_\psi+\frac{r^2\sin^2\theta}{4}\dot\phi.
$$

Dots denote [derivatives](../../../calculus.md#derivative) with respect to an [affine parameter](../../../riemannian-geometry.md#affine-parameter). On the chosen submanifold $\dot\phi=0$ and $\cos\theta=0$, so $L_\phi=0$. Requiring also $L_\psi=0$ gives

$$
\boxed{\dot\psi=\Omega(r)\dot t.}
$$

More generally, away from the polar-coordinate axes, both displayed angular charges being zero imply $\dot\phi=0$ and the same relation. In particular, zero conserved [angular momentum](../../../classical-mechanics.md#angular-momentum) does not imply constant $\psi$: the motion follows the local dragging of the angular coordinate by the rotating geometry.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the zero-angular-momentum curves, the fiber term in the induced [metric tensor](../../../general-relativity.md#metric-tensor) vanishes along the tangent, leaving

$$
0=-\frac f h\dot t^2+\frac{\dot r^2}{f}
$$

for a [null geodesic](../../../special-relativity.md#null-geodesic). In the exterior, a future [geodesic](../../../riemannian-geometry.md#geodesic) has positive conserved [energy](../../../classical-mechanics.md#energy) $E=(f/h)\dot t$. Its equations are

$$
\dot r=\pm E\sqrt h,\qquad \dot t=\frac{Eh}{f},\qquad
\frac{dt}{dr}=\pm\frac{\sqrt h}{f}.
$$

Define the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate), separately on intervals bounded by horizon radii, by

$$
\boxed{r_*(r)=\int^r\frac{\sqrt{h(s)}}{f(s)}\,ds.}
$$

For an outgoing curve $\dot r=+E\sqrt h$,

$$
\frac d{d\lambda}(t-r_*)=\dot t-r_*'\dot r=0;
$$

for an ingoing curve $\dot r=-E\sqrt h$, $d(t+r_*)/d\lambda=0$. Thus $u=t-r_*$ and $v=t+r_*$ are the respective constant labels. The [derivative](../../../calculus.md#derivative) $\sqrt h/f$, with its sign, is required for continuation; taking $\sqrt h/|f|$ would give the wrong labels between the horizons.

For a nonextremal horizon $r=r_H$, the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) has leading behavior

$$
r_*\sim\frac{\sqrt{h(r_H)}}{f'(r_H)}\log|r-r_H|.
$$

At the double root of the [extremal black hole](../../../general-relativity.md#extremal-black-hole) it instead has a pole. These singularities are coordinate effects at a regular [Killing horizon](../../../general-relativity.md#killing-horizon); they are not the [curvature singularity](../../../general-relativity.md#curvature-singularity) at $r=0$. To cross the future horizon, the ingoing coordinates

$$
v=t+r_*,\qquad \psi_+=\psi+\int^r\frac{\Omega(s)\sqrt{h(s)}}{f(s)}\,ds
$$

give the regular induced [metric tensor](../../../general-relativity.md#metric-tensor)

$$
ds_3^2=-\frac f h\,dv^2+\frac2{\sqrt h}\,dv\,dr
+r^2h(d\psi_+-\Omega\,dv)^2.
$$

This also fixes the future branch used in the causal argument below.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Relative to a chosen asymptotically flat end, define the [black hole](../../../general-relativity.md#black-hole) region by

$$
\boxed{\mathcal B=\mathcal M\setminus J^-(\mathcal I^+),}
$$

where $\mathcal I^+$ is that end's [future null infinity](../../../general-relativity.md#future-null-infinity) in a [conformal completion](../../../general-relativity.md#conformal-completion). It consists of events unable to send a future causal signal to that infinity; its boundary is the corresponding future [event horizon](../../../general-relativity.md#event-horizon).

For $0<\alpha<r_0/2$, $h>0$ and $f<0$ on $r_-<r<r_+$. The [gradient](../../../calculus.md#gradient) of $r$ has norm $g^{ab}\nabla_ar\nabla_br=f$, so it is timelike there. Use the future extension regular in the ingoing coordinates above, reached by an exterior future ingoing [null geodesic](../../../special-relativity.md#null-geodesic) with $\dot r=-E\sqrt h<0$. This determines $\nabla r$ to be future timelike in the inter-horizon block. Every nonzero future causal tangent $V$ therefore obeys

$$
\frac{dr}{d\lambda}=g(\nabla r,V)<0.
$$

At the future outer horizon the [gradient](../../../calculus.md#gradient) becomes future null and gives the corresponding one-way inequality $dr/d\lambda\leq0$. No future signal can cross that horizon outward to the selected exterior. The future inter-horizon block is consequently within $\mathcal B$; a future-directed path can leave it only through the inner horizon, not return through the outer horizon to the selected infinity.

This statement requires a branch and an end. The maximal extension also contains time-reversed inter-horizon blocks, where future-directed curves have increasing $r$ and emerge into an exterior: they are [white holes](../../../general-relativity.md#white-hole), not the selected [black hole](../../../general-relativity.md#black-hole) region. Thus the unqualified claim for every copy of $r_-<r<r_+$ in an arbitrary extension is false. Analytic continuation past a [Cauchy horizon](../../../general-relativity.md#cauchy-horizon) can also introduce other asymptotic ends; the displayed definition explicitly refers to the chosen component of infinity.

To sketch the causal structure, suppress the spacelike $\psi$ circle by its orbit-space projection. The induced three-dimensional [metric tensor](../../../general-relativity.md#metric-tensor) is

$$
ds_3^2=q+r^2h(d\psi-\Omega dt)^2,\qquad
q=-\frac f h\,dt^2+\frac{dr^2}{f}=\frac f h(-dt^2+dr_*^2).
$$

The [causal projection along a spacelike circular fiber](../../../general-relativity.md#causal-projection-along-a-spacelike-circular-fiber) is exact: any [causal curve](../../../general-relativity.md#causal-curve) projects to a $q$-[causal curve](../../../general-relativity.md#causal-curve), and every base curve has a lift $d\psi=\Omega dt$ with exactly its base norm. The diagrams therefore represent this two-dimensional orbit space, not a constant-$\psi$ slice of the three-dimensional submanifold.

There are three nonextremal block types. For $r>r_+$, $r_*$ spans the full real line from the outer horizon to infinity, producing an exterior diamond. For $r_-<r<r_+$, $r_*$ spans the full line with the time and space roles reversed; these diamonds contain the future black-hole or past white-hole branches. For $0<r<r_-$, $r_*$ is finite at zero and diverges at the inner horizon, producing a static half-diamond with a timelike singular edge. The supplied [Kretschmann scalar](../../../general-relativity.md#kretschmann-scalar) diverges as $384\alpha^4r_0^4/r^{12}$ at $r=0$, and $f>0$ on the inner side, so that edge is a genuine timelike [curvature singularity](../../../general-relativity.md#curvature-singularity). In contrast, both horizon radii are regular in horizon-adapted coordinates.

<a id="3/d/image-nonextremal-orbit-space-causal-structure"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311-penrose-nonextremal.png)

**[Figure 1](#3/d/image-nonextremal-orbit-space-causal-structure). Nonextremal orbit-space causal structure**.

The finite strip shows two exterior levels, a future trapped block, an inner static level with timelike singularities, and the next emerging block. Continuing through the inner [Cauchy horizons](../../../general-relativity.md#cauchy-horizon) repeats this pattern upward and downward in the maximal analytic extension. The inner boundary is not a spacelike Schwarzschild-type singularity. Such an ideal extension need not describe a physical collapse past its unstable inner horizon.

At $\alpha=r_0/2$, put $R=r_0/\sqrt2$. Then $r_+=r_-=R$, $f=(r^2-R^2)^2/r^4$, and the interval $r_-<r<r_+$ is empty. The lapse is positive on both sides, so there is no inter-horizon trapped diamond. The horizon is a [degenerate Killing horizon](../../../general-relativity.md#degenerate-killing-horizon), with $\kappa=0$. In the exterior $r_*\to-\infty$ as $r\downarrow R$, while inside $r_*\to+\infty$ as $r\uparrow R$; more precisely its leading pole is $-\sqrt2 R^2/[4(r-R)]$. Static proper distance to the horizon is infinite. Future ingoing rays still cross it at finite affine parameter, as the regular ingoing [metric tensor](../../../general-relativity.md#metric-tensor) shows.

<a id="3/d/image-extremal-conformal-blocks-and-horizon-gluing"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311-penrose-extremal.png)

**[Figure 2](#3/d/image-extremal-conformal-blocks-and-horizon-gluing). Extremal conformal blocks and horizon gluing**.

The extremal sketch gives the exterior diamond and singular interior half-diamond, with the complete gluing prescription: the exterior future horizon attaches to the interior past horizon; the interior future horizon attaches to the past horizon of another exterior. Repeating these attachments gives the maximal extension. The marked throat endpoints are conformal ideal endpoints, not bifurcation points of the [spacetime](../../../special-relativity.md#spacetime). This block representation avoids incorrectly treating the extremal geometry as two transverse horizons with a collapsed trapped region.

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work first in units $G=c=\hbar=k_B=1$. [Black-hole thermodynamics](../../../general-relativity.md#black-hole-thermodynamics) starts with the [laws of black-hole mechanics](../../../general-relativity.md#laws-of-black-hole-mechanics). For a [connected](../../../geometry-and-topology.md#connected-space) stationary regular [Killing horizon](../../../general-relativity.md#killing-horizon), the [Zeroth law of black-hole mechanics](../../../general-relativity.md#zeroth-law-of-black-hole-mechanics) makes its [surface gravity](../../../general-relativity.md#surface-gravity) $\kappa$ constant when the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) and [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) hold. This parallels uniform equilibrium [temperature](../../../thermodynamics.md#temperature). For neighboring stationary asymptotically flat four-dimensional Einstein-Maxwell [black holes](../../../general-relativity.md#black-hole), the [First law of black-hole mechanics](../../../general-relativity.md#first-law-of-black-hole-mechanics) is

$$
\delta M=\frac\kappa{8\pi}\delta A+\Omega_H\delta J+\Phi_H\delta Q,
$$

where $\Omega_H$ is the horizon [angular velocity](../../../classical-mechanics.md#angular-velocity) and $\Phi_H$ its [electric potential](../../../electromagnetism.md#electric-potential) relative to infinity. The last terms are rotational and electromagnetic work, analogous to the work terms in $\delta E=T\delta S+\text{work}$. The [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics), expressed by [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem), makes the total future horizon area nondecreasing for classical matter obeying the [null energy condition](../../../general-relativity.md#null-energy-condition) and global assumptions such as [strong asymptotic predictability](../../../general-relativity.md#strong-asymptotic-predictability). The [third law of black-hole mechanics](../../../general-relativity.md#third-law-of-black-hole-mechanics) is an unattainability statement: subject to the usual regularity assumptions, the [weak energy condition](../../../general-relativity.md#weak-energy-condition), and a bounded [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor), no finite physical process reduces the [surface gravity](../../../general-relativity.md#surface-gravity) of a regular horizon to zero. It does not assert that [extremal black holes](../../../general-relativity.md#extremal-black-hole) have zero area or zero [entropy](../../../thermodynamics.md#entropy).

Classical geometry alone fixes an analogy, not a nonzero physical [temperature](../../../thermodynamics.md#temperature). [Quantum field theory](../../../quantum-field-theory.md) supplies [Hawking temperature](../../../general-relativity.md#hawking-temperature) $T_H=\kappa/(2\pi)$. Comparing the area term of the first law with $T_H\delta S$ gives $\delta S=\delta A/4$ for nonextremal holes, and hence the standard [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy). Restoring physical constants,

$$
\boxed{T_H=\frac{\hbar\kappa}{2\pi c k_B},\qquad
S_{\mathrm{BH}}=\frac{k_Bc^3A}{4G\hbar}=\frac{k_BA}{4\ell_P^2}.}
$$

Here restored $\kappa$ is the physical acceleration [surface gravity](../../../general-relativity.md#surface-gravity) and $\ell_P^2=G\hbar/c^3$ is the squared [Planck length](../../../physics.md#planck-length). The first-law comparison determines the area coefficient, leaving an additive [entropy](../../../thermodynamics.md#entropy) constant unspecified; the displayed formula is the usual convention. Its area scaling, rather than ordinary volume scaling, signals that the available thermodynamic degrees of freedom of a gravitating system are constrained by the horizon geometry.

Particle production explains the quantum input. For a [real scalar field](../../../scalar-field-theory.md#real-scalar-field) obeying the massless covariant [wave equation](../../../wave-equation.md), the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) on solutions is

$$
(u,v)=i\int_\Sigma d\Sigma^a\left(u^*\nabla_av-v\nabla_au^*\right).
$$

The [wave equation](../../../wave-equation.md) makes its current divergence-free, so the product is independent of a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) when the boundary flux vanishes. Use suitably normalized [wave packets](../../../wave-equation.md#wave-packet) or the appropriate continuum distributions. Asymptotic past and future [Minkowski spacetimes](../../../special-relativity.md#minkowski-spacetime) give preferred [positive-frequency solution](../../../quantum-field-theory.md#positive-frequency-solution) mode bases $u_j^{\mathrm{in}}$ and $u_i^{\mathrm{out}}$, normalized by $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and $(u_i,u_j^*)=0$. Between those regions, a nonstationary geometry generally has no preferred positive-frequency splitting.

The mode bases are related by a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation),

$$
u_i^{\mathrm{out}}=\sum_j\left(\alpha_{ij}u_j^{\mathrm{in}}+\beta_{ij}u_j^{\mathrm{in}*}\right),
\qquad
\alpha\alpha^\dagger-\beta\beta^\dagger=I,\quad
\alpha\beta^T=\beta\alpha^T.
$$

The last identities follow from conservation of the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) and are the [canonical identities for a bosonic Bogoliubov transformation](../../../quantum-field-theory.md#canonical-identities-for-a-bosonic-bogoliubov-transformation). Expanding the field in either complete basis and extracting its positive-frequency coefficient gives

$$
a_i^{\mathrm{out}}=\sum_j\left(\alpha_{ij}^*a_j^{\mathrm{in}}-\beta_{ij}^*a_j^{\mathrm{in}\dagger}\right).
$$

Thus the state annihilated by every $a_j^{\mathrm{in}}$ has

$$
\boxed{\langle0_{\mathrm{in}}|N_i^{\mathrm{out}}|0_{\mathrm{in}}\rangle
=\sum_j|\beta_{ij}|^2.}
$$

This [particle number from Bogoliubov coefficients](../../../quantum-field-theory.md#particle-number-from-bogoliubov-coefficients) is nonzero when time evolution mixes positive and negative frequencies. It describes one state as vacuum in the early particle basis and populated in the late basis; it does not require an arbitrary choice of a vacuum at each intermediate time. For a finite implementable transformation the state remains a squeezed [pure quantum state](../../../quantum-theory.md#pure-state). In infinitely many modes, a common unitary [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space) implementation requires additional conditions, such as the beta map being a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator); finite [wave packet](../../../wave-equation.md#wave-packet) observables need not share every global divergence of an ideal continuum calculation.

For gravitational collapse, the future is not globally Minkowski: it contains a [black hole](../../../general-relativity.md#black-hole). The relevant late out-basis includes modes reaching [future null infinity](../../../general-relativity.md#future-null-infinity) together with modes entering the future [event horizon](../../../general-relativity.md#event-horizon). Modes on infinity alone are not a complete Cauchy basis. Nevertheless the same mode-mixing calculation determines the outgoing particle flux. Near a nonextremal horizon, the logarithm in the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) converts regular early null coordinates into the [Hawking exponential ray map](../../../general-relativity.md#hawking-exponential-ray-map)

$$
U_H-U=Ae^{-\kappa u},\qquad A>0,
$$

where $U$ is the early affine null coordinate and $u$ is late retarded time at infinity. Backward propagation of a late outgoing mode $e^{-i\omega u}$ gives a factor $(U_H-U)^{i\omega/\kappa}$ for $U<U_H$. Its positive- and negative-frequency Fourier [integrals](../../../calculus.md#integral) differ by [analytic continuation](../../../complex-analysis.md#analytic-continuation) around the logarithmic branch. With a convergence regulator they reduce to

$$
\int_0^\infty x^{ia}e^{-(\epsilon\pm i\omega')x}\,dx
=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia},\qquad a=\frac\omega\kappa.
$$

Taking $\epsilon\downarrow0$ gives the [thermal ratio of Hawking Bogoliubov coefficients](../../../general-relativity.md#thermal-ratio-of-hawking-bogoliubov-coefficients), $|\beta|^2/|\alpha|^2=e^{-2\pi\omega/\kappa}$. Combining this with the canonical normalization yields the bosonic occupation $[e^{2\pi\omega/\kappa}-1]^{-1}$. Late-time [wave packets](../../../wave-equation.md#wave-packet) turn formal continuum coefficients into a finite number flux.

A [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime) has $\kappa=1/(4M)$, so this spectrum has $T_H=1/(8\pi M)$. The exterior curvature potential partly reflects the outgoing modes. Its transmission [probabilities](../../../probability-theory.md#probability) are the [greybody factors](../../../general-relativity.md#greybody-factor), giving, for one massless scalar species in the stationary late-time approximation,

$$
\frac{d^2N}{du\,d\omega}=\frac1{2\pi}
\sum_{\ell=0}^{\infty}(2\ell+1)
\frac{\Gamma_\ell(\omega)}{e^{8\pi M\omega}-1}.
$$

Thus the horizon [temperature](../../../thermodynamics.md#temperature) is universal, while the spectrum received at infinity is not a perfect featureless [blackbody radiation](../../../statistical-physics.md#black-body-radiation) spectrum. The derivation assumes the near-horizon [quantum state](../../../quantum-mechanics.md#quantum-state) inherited from a regular collapse vacuum and ignores rapid backreaction over the timescale of the packets. Exponentially blueshifted precursor frequencies indicate the usual short-distance assumption in the semiclassical calculation, not an independently demonstrated quantum-gravity description of the endpoint.

The outgoing positive [energy](../../../classical-mechanics.md#energy) flux drives [black-hole evaporation](../../../general-relativity.md#black-hole-evaporation). At leading order for a large isolated [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime), area scales as $M^2$ and [temperature](../../../thermodynamics.md#temperature) as $M^{-1}$, giving $dM/du\sim-\gamma/M^2$ and a lifetime of order $M^3$, with the coefficient depending on species and transmission factors. Its [negative heat capacity of a Schwarzschild black hole](../../../general-relativity.md#negative-heat-capacity-of-a-schwarzschild-black-hole), $dM/dT_H=-8\pi M^2$, means that it heats up as it loses [mass](../../../classical-mechanics.md#mass) and cannot be in stable canonical equilibrium with an unlimited thermal reservoir. The approximation fails when quantum-gravitational scales are reached and does not fix whether the endpoint is complete evaporation, a remnant, or something else.

Area loss does not contradict the classical area theorem, because the quantum [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) need not obey the classical [null energy condition](../../../general-relativity.md#null-energy-condition); negative horizon [energy](../../../classical-mechanics.md#energy) accompanies the positive outgoing flux. The appropriate thermodynamic statement is the [generalized second law](../../../general-relativity.md#generalized-second-law), involving $S_{\mathrm{BH}}+S_{\mathrm{outside}}$. Finally, [Hawking radiation](../../../general-relativity.md#hawking-radiation) raises the [black hole information paradox](../../../general-relativity.md#black-hole-information-paradox): if a [pure quantum state](../../../quantum-theory.md#pure-state) completely evaporates into an exactly thermal [mixed quantum state](../../../quantum-theory.md#mixed-state) and its partners disappear, the result conflicts with ordinary [unitary time evolution](../../../quantum-mechanics.md#unitary-time-evolution). Early outgoing radiation can be mixed simply because of its [entanglement](../../../bell-state.md#entangled-state) with interior modes while the complete state remains a [pure quantum state](../../../quantum-theory.md#pure-state); that fact alone is not information loss. Resolving the fate of all correlations through the evaporation endpoint requires more than the leading semiclassical flux calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
