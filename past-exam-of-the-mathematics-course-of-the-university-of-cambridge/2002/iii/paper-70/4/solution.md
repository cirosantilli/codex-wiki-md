<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use an [SU(2)](../../../../../su-2-group.md) [connection one-form](../../../../../connection-one-form.md) $A=A_\mu dx^\mu$ with [Skew-Hermitian](../../../../../skew-hermitian-matrix.md) generators $T_a=-i\sigma_a/2$, so $\operatorname{tr}(T_aT_b)=-\delta_{ab}/2$. Absorb the gauge coupling into $A$, and write its [gauge curvature](../../../../../gauge-field-strength.md) as $F=dA+A\wedge A$. The [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) convention is $A^h=h^{-1}Ah+h^{-1}dh$, giving $F^h=h^{-1}Fh$.

In four dimensions the [Second Chern form](../../../../../second-chern-form.md) and [Second Chern number](../../../../../second-chern-number.md) of the associated fundamental rank-two bundle are

$$
c_2(A)=\frac1{8\pi^2}\operatorname{tr}(F\wedge F),\qquad
k_C=\int_Mc_2(A)\in\mathbb Z.
$$

Here $M$ is a closed oriented four-manifold. This sign follows by expanding the total [Chern class](../../../../../chern-class.md) $\det(1+iF/(2\pi))$ and using $\operatorname{tr}F=0$. The first Chern class vanishes for [SU(2)](../../../../../su-2-group.md); the second is the degree-four characteristic class relevant here. With the same curvature convention the commonly positive self-dual [instanton number](../../../../../instanton-number.md) is

$$
Q=-\frac1{8\pi^2}\int_M\operatorname{tr}(F\wedge F)=-k_C.
$$

Both sign conventions occur; fixing them at the outset avoids identifying opposite-oriented integers.

The form is [gauge-invariant](../../../../../gauge-invariance.md) by conjugation and cyclicity of the [matrix trace](../../../../../matrix-trace.md). The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) $D_AF=0$ makes it closed. To see that its integral is independent of the connection, vary $A$:

$$
\delta F=D_A\delta A,\qquad
\delta\operatorname{tr}(F\wedge F)
=2d\,\operatorname{tr}(\delta A\wedge F).
$$

On a closed $M$ the integral of this exact form vanishes. This is [Chern-Weil connection transgression](../../../../../chern-weil-connection-transgression.md), showing that $k_C$ depends on the bundle's topology rather than on a particular [gauge field](../../../../../gauge-field.md).

Locally the same four-form is an exterior derivative. The [Chern-Simons 3-form](../../../../../chern-simons-3-form.md)

$$
\omega_3(A)=\operatorname{tr}\left(A\wedge dA+
\frac23A\wedge A\wedge A\right)
$$

satisfies

$$
d\omega_3=\operatorname{tr}(F\wedge F).
$$

For verification, differentiating gives $\operatorname{tr}(dA\wedge dA+2dA\wedge A\wedge A)$; expansion of $F\wedge F$ gives these terms and $\operatorname{tr}A^4$. Graded cyclicity moves the first one-form through the other three, changing the sign, so $\operatorname{tr}A^4=0$. This local exactness does not make the [Second Chern number](../../../../../second-chern-number.md) zero on every closed manifold: on a nontrivial bundle the gauge potentials and $\omega_3$ are only patchwise defined.

For the usual finite-action sector on $\mathbb R^4$, impose pure-gauge behavior $A\to h^{-1}dh$ at infinity. Compactification gives a bundle over $S^4$, with transition map $h:S^3\to SU(2)$. The [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md) gives $d(h^{-1}dh)=-(h^{-1}dh)^2$, hence

$$
\omega_3(h^{-1}dh)=-\frac13\operatorname{tr}(h^{-1}dh)^3.
$$

With the outward boundary orientation, [Stokes theorem](../../../../../stokes-theorem.md) therefore gives

$$
k_C=-\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{tr}(h^{-1}dh)^3,\qquad
Q=\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{tr}(h^{-1}dh)^3.
$$

These are opposite choices of the [winding number](../../../../../winding-number.md), and either becomes the [topological degree](../../../../../topological-degree.md) of $h$ after specifying the orientation of the target [SU(2)](../../../../../su-2-group.md) sphere. Thus integrality also follows from $\pi_3(SU(2))=\mathbb Z$. Smooth deformations preserving the asymptotic sector cannot change it.

The positive Euclidean [Yang-Mills action](../../../../../yang-mills-action.md) is

$$
S=-\frac1{g^2}\int_M\operatorname{tr}(F\wedge *F)
=\frac1{4g^2}\int_MF_{\mu\nu}^aF_{\mu\nu}^a\,d^4x.
$$

Define $\|X\|^2=-\int\operatorname{tr}(X\wedge *X)$. Since the [Hodge star](../../../../../hodge-star-operator.md) has square one on two-forms in Euclidean dimension four,

$$
S=\frac1{2g^2}\|F-s*F\|^2+\frac{8\pi^2s}{g^2}Q,
\qquad s=\pm1.
$$

Choosing $s=\operatorname{sgn}Q$ gives the [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md)

$$
\boxed{S\geq\frac{8\pi^2}{g^2}|Q|,\qquad
F=s*F\ \text{at equality}.}
$$

The [self-dual Yang-Mills equations](../../../../../self-dual-yang-mills-equations.md) and their anti-self-dual version imply the [Yang-Mills equations](../../../../../yang-mills-equations.md) $D_A*F=0$ by the [Bianchi identity](../../../../../bianchi-identity.md). Their finite-action solutions are [Yang-Mills instantons](../../../../../yang-mills-instanton.md).

For a concrete self-dual example, the [BPST instanton](../../../../../bpst-instanton.md) with center $a$ and size $\rho>0$ has

$$
A_\mu^a=\frac{2\eta^a_{\mu\nu}(x-a)^\nu}{|x-a|^2+\rho^2},
\qquad
F_{\mu\nu}^a=-\frac{4\rho^2\eta^a_{\mu\nu}}
{(|x-a|^2+\rho^2)^2},
$$

where $\eta^a_{\mu\nu}$ are self-dual ['t Hooft symbols](../../../../../t-hooft-symbol.md). Their contraction is $\sum_{a,\mu,\nu}(\eta^a_{\mu\nu})^2=12$. Thus $F_{\mu\nu}^aF_{\mu\nu}^a=192\rho^4/(|x-a|^2+\rho^2)^4$, and

$$
\int_{\mathbb R^4}\frac{\rho^4\,d^4x}{(|x|^2+\rho^2)^4}
=2\pi^2\int_0^\infty\frac{\rho^4r^3\,dr}{(r^2+\rho^2)^4}
=\frac{\pi^2}{6}.
$$

This gives $S=8\pi^2/g^2$ and $Q=1$. Reversing duality gives $Q=-1$. The free center, size and framed gauge orientation illustrate the [instanton moduli space](../../../../../instanton-moduli-space.md).

On a three-dimensional slice $\Sigma$, there is no four-form Chern integral intrinsic to the slice. Its transgression is the [Chern-Simons number of a gauge field](../../../../../chern-simons-number-of-a-gauge-field.md), in the instanton-charge convention

$$
N_{\mathrm{CS}}[A]=-\frac1{8\pi^2}\int_\Sigma\omega_3(A).
$$

It is a real number for a general connection, not necessarily an integer, and is not strictly gauge invariant. Set $\theta=h^{-1}dh$ and $\bar\theta=dh\,h^{-1}$. Substituting $A^h=h^{-1}Ah+\theta$, using $d\theta=-\theta^2$ and graded trace cyclicity, gives the [gauge change of the Chern-Simons three-form](../../../../../gauge-change-of-the-chern-simons-three-form.md)

$$
\omega_3(A^h)=\omega_3(A)-d\operatorname{tr}(\bar\theta\wedge A)
-\frac13\operatorname{tr}\theta^3.
$$

The mixed terms collect into the displayed exact form; the last term is also fixed by the pure-gauge case $A=0$. Therefore on a closed $\Sigma$, or with boundary conditions making the exact-form integral vanish,

$$
\boxed{N_{\mathrm{CS}}[A^h]=N_{\mathrm{CS}}[A]+w(h),\qquad
w(h)=\frac1{24\pi^2}\int_\Sigma\operatorname{tr}(h^{-1}dh)^3\in\mathbb Z.}
$$

Thus $N_{\mathrm{CS}}\bmod\mathbb Z$, or $\exp(2\pi iN_{\mathrm{CS}})$, is gauge invariant. Gauge maps homotopic to the identity have $w=0$; maps of nonzero winding are large transformations even when they equal the identity at infinity.

For a [Yang-Mills vacuum](../../../../../yang-mills-vacuum.md) on $\mathbb R^3$, zero magnetic [energy](../../../../../energy.md) requires $F_{ij}=0$. On simply connected space this is a pure gauge $A=h^{-1}dh$, and $N_{\mathrm{CS}}=w(h)$ is an integer after fixing the asymptotic trivialization. Quotienting only by transformations homotopic to the identity leaves integer-labelled vacuum representatives. Allowing all winding transformations identifies them classically; quantum states can instead transform by a phase, producing the [theta vacuum](../../../../../theta-vacuum.md). A three-dimensional pure-gauge representative carries a winding number but is not a localized positive-energy monopole. In fact [no static finite-energy lump in three-dimensional pure Yang-Mills theory](../../../../../no-static-finite-energy-lump-in-three-dimensional-pure-yang-mills-theory.md) exists with the usual decay conditions: $A_i^{(s)}(x)=sA_i(sx)$ gives $E(s)=sE(1)$, and stationarity forces $E=0$.

Finally, on an oriented spacetime slab $[t_-,t_+]\times\Sigma$, with no side-boundary contribution, the transgression identity gives

$$
\boxed{Q=N_{\mathrm{CS}}(t_+)-N_{\mathrm{CS}}(t_-).}
$$

A [Yang-Mills instanton](../../../../../yang-mills-instanton.md) therefore interpolates between vacuum representatives whose [Chern-Simons numbers](../../../../../chern-simons-number-of-a-gauge-field.md) differ by its integer charge. In a four-dimensional quantum theory a [Yang-Mills theta term](../../../../../yang-mills-theta-term.md) weights such sectors by $e^{i\theta Q}$, making $\theta$ periodic modulo $2\pi$. In an intrinsically three-dimensional theory an action $2\pi\ell N_{\mathrm{CS}}$ has a gauge-invariant phase $e^{iS}$ only for integer level $\ell$ under all winding gauge maps. These statements distinguish the gauge-invariant integer four-dimensional Chern charge from the three-dimensional connection-dependent quantity defined modulo integers.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
