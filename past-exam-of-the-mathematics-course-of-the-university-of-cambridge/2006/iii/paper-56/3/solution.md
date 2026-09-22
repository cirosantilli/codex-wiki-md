<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Yang-Mills instanton](../../../../../yang-mills-instanton.md) is a localized finite-action Euclidean [gauge field](../../../../../gauge-field.md) with self-dual or anti-self-dual [gauge curvature](../../../../../gauge-field-strength.md). It is a four-dimensional space-time event, rather than a static three-dimensional finite-energy monopole. Take [gauge group](../../../../../gauge-group.md) $SU(2)$ first, with [Skew-Hermitian](../../../../../skew-hermitian-matrix.md) generators $T_a=-i\sigma_a/2$, $[T_a,T_b]=\epsilon_{abc}T_c$, and $\operatorname{tr}(T_aT_b)=-\delta_{ab}/2$. Write

$$
A=A_\mu dx^\mu,\quad F=dA+A\wedge A,\quad D_\mu=\partial_\mu+[A_\mu,\,\cdot\,],
$$

and fix orientation $dx^1\wedge dx^2\wedge dx^3\wedge dx^4$. The positive [Euclidean action](../../../../../euclidean-action.md) is

$$
S=-\frac1{g^2}\int\operatorname{tr}(F\wedge *F)
=\frac1{4g^2}\int F^a_{\mu\nu}F^a_{\mu\nu}\,d^4x.
$$

Varying $F$ gives $\delta F=D\delta A$. Integration by parts makes stationarity equivalent to $D_\mu F_{\mu\nu}=0$. The [Bianchi identity](../../../../../bianchi-identity.md) $DF=0$ follows by expanding $F=dA+A\wedge A$, using $d^2=0$, and cancelling the remaining [matrix commutator](../../../../../commutator.md) terms. Consequently $F=\pm *F$ implies the [Yang-Mills equations](../../../../../yang-mills-equations.md): $D*F=\pm DF=0$. [Self-duality of gauge curvature](../../../../../self-duality-of-gauge-curvature.md) is an extra first-order condition, not a property of every finite-action [gauge connection](../../../../../connection-vector-bundle.md).

For the usual [instanton](../../../../../instanton.md) decay conditions, the field is asymptotically pure gauge, $A\sim h^{-1}dh$ on the sphere at infinity. The boundary map $h:S^3\to SU(2)\simeq S^3$ has an [integer](../../../../../integer.md) degree. With the present trace convention define the [instanton number](../../../../../instanton-number.md) by

$$
k=-\frac1{8\pi^2}\int\operatorname{tr}(F\wedge F)
=\frac1{32\pi^2}\int F^a_{\mu\nu}(*F)^a_{\mu\nu}\,d^4x.
$$

The identity

$$
\operatorname{tr}(F\wedge F)=d\operatorname{tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right)
$$

turns this integral into a boundary winding integral: for $A=h^{-1}dh$, the three-form in parentheses is $-\tfrac13\operatorname{tr}(h^{-1}dh)^3$, giving $k=(24\pi^2)^{-1}\int_{S^3}\operatorname{tr}(h^{-1}dh)^3$, with the chosen boundary orientation. The normalized invariant three-form computes the degree of $h$, so $k\in\mathbb Z$. Equivalently the gauge bundle extends across conformal infinity to a bundle on $S^4$, and this is its [Second Chern number](../../../../../second-chern-number.md) convention. A smooth deformation preserving the boundary class cannot change this [integer](../../../../../integer.md).

Square completion gives the [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md):

$$
S=\frac1{8g^2}\int(F^a_{\mu\nu}\mp(*F)^a_{\mu\nu})^2d^4x
\ \pm\ \frac{8\pi^2}{g^2}k
\quad\Longrightarrow\quad
\boxed{S\ge\frac{8\pi^2}{g^2}|k|.}
$$

Self-dual [gauge curvature](../../../../../gauge-field-strength.md) saturates the bound for $k>0$, and anti-self-dual [gauge curvature](../../../../../gauge-field-strength.md) for $k<0$. These are [Yang-Mills action](../../../../../yang-mills-action.md) minima within their topological sectors. Gauge variations give redundant directions, and variations along the moduli give [zero modes](../../../../../zero-mode.md); there is no negative second variation within the fixed-charge sector at a bound-saturating solution.

An explicit charge-one solution is the [BPST instanton](../../../../../bpst-instanton.md). Put $y=x-a$, $r^2=y_\mu y_\mu$, $d=r^2+\rho^2$, with $\rho>0$. The self-dual ['t Hooft symbols](../../../../../t-hooft-symbol.md) are defined by $\eta^a_{ij}=\epsilon_{aij}$ and $\eta^a_{i4}=\delta_{ai}$, extended antisymmetrically. Then

$$
A_\mu^a=\frac{2\eta^a_{\mu\nu}y_\nu}{d},\qquad
F_{\mu\nu}^a=-\frac{4\rho^2\eta^a_{\mu\nu}}{d^2}.
$$

For completeness, differentiation supplies $-4\eta^a_{\mu\nu}/d-4K^a_{\mu\nu}/d^2$, where $K^a_{\mu\nu}=\eta^a_{\nu\lambda}y_\lambda y_\mu-\eta^a_{\mu\lambda}y_\lambda y_\nu$. The [matrix commutator](../../../../../commutator.md) term supplies $4C^a_{\mu\nu}/d^2$, and the symbol identity

$$
C^a_{\mu\nu}=\epsilon_{abc}\eta^b_{\mu\lambda}\eta^c_{\nu\sigma}y_\lambda y_\sigma
=r^2\eta^a_{\mu\nu}+K^a_{\mu\nu}
$$

reduces their sum to the stated [gauge curvature](../../../../../gauge-field-strength.md). Since $*\eta^a=\eta^a$, it is self-dual and solves the [Yang-Mills equations](../../../../../yang-mills-equations.md). The [gauge potential](../../../../../gauge-field.md) is regular at the center in this gauge, and [gauge curvature](../../../../../gauge-field-strength.md) falls as $r^{-4}$ at infinity.

The squared-symbol sum is 12, so

$$
F^a_{\mu\nu}F^a_{\mu\nu}=\frac{192\rho^4}{(r^2+\rho^2)^4},\qquad
\int_{\mathbb R^4}\frac{\rho^4}{(r^2+\rho^2)^4}\,d^4x=\frac{\pi^2}{6}.
$$

The second integral follows from $d^4x=2\pi^2r^3dr$ and the substitution $u=r^2$. Thus

$$
\boxed{S_{\rm BPST}=8\pi^2/g^2,\qquad k=1.}
$$

Replacing the symbols by their anti-self-dual counterparts reverses the charge and gives an [anti-instanton](../../../../../anti-instanton.md). A compact non-Abelian group with an $SU(2)$ subgroup admits corresponding embedded examples.

The center $a\in\mathbb R^4$ gives four position moduli and $\rho>0$ gives one size modulus. In a [framed instanton moduli space](../../../../../framed-instanton-moduli-space.md), [gauge transformations](../../../../../gauge-transformation.md) are required to approach the identity at infinity, so three global $SU(2)$ orientation parameters remain, making eight real parameters for one [instanton](../../../../../instanton.md). If constant [gauge transformations](../../../../../gauge-transformation.md) are also divided out, only the five position-and-size parameters remain. The size costs no classical [Yang-Mills action](../../../../../yang-mills-action.md): under $A_\mu(x)\mapsto\lambda A_\mu(\lambda x)$, [gauge curvature](../../../../../gauge-field-strength.md) scales by $\lambda^2$ and the four-dimensional volume by $\lambda^{-4}$. As $\rho\to0$, [gauge curvature](../../../../../gauge-field-strength.md) concentrates at the center; the limiting object is a singular bubbling boundary of [moduli space](../../../../../moduli-space.md), not a smooth zero-size solution.

Higher-charge solutions require genuine nonlinear constructions, rather than a linear sum of charge-one [gauge potentials](../../../../../gauge-field.md). The [ADHM construction](../../../../../adhm-construction.md) gives a finite-dimensional description. For $V=\mathbb C^\ell$, $W=\mathbb C^N$, take $B_1,B_2\in\operatorname{End}(V)$, $I:W\to V$, $J:V\to W$, satisfying

$$
[B_1,B_2]+IJ=0,\qquad
[B_1,B_1^\dagger]+[B_2,B_2^\dagger]+II^\dagger-J^\dagger J=0,
$$

modulo the natural [group action](../../../../../group-action.md) of $U(\ell)$. Here $\ell$ is the charge magnitude, avoiding confusion with the signed $k$ above. Regularity requires the following [matrix](../../../../../matrix.md) to have full row rank everywhere:

$$
\mathcal D_z=
\begin{pmatrix}B_2-z_2&B_1-z_1&I\\-B_1^\dagger+\bar z_1&B_2^\dagger-\bar z_2&J^\dagger\end{pmatrix},
\qquad z_1=x^1+ix^2,\quad z_2=x^3+ix^4.
$$

The complex constraint kills the off-diagonal block of $\mathcal D_z\mathcal D_z^\dagger$, while the real constraint equates its diagonal blocks. Thus $\mathcal D_z\mathcal D_z^\dagger=1_2\otimes f^{-1}$. Choose an orthonormal [matrix](../../../../../matrix.md) of kernel columns $\Psi$, with $\Psi^\dagger\Psi=1_N$, and define $A=\Psi^\dagger d\Psi$.

This is not merely a parameter count: its [gauge curvature](../../../../../gauge-field-strength.md) is checked by the [ADHM factorization identity](../../../../../adhm-factorization-identity.md). The complementary [orthogonal projection](../../../../../orthogonal-projection.md) is $\mathcal D_z^\dagger(1_2\otimes f)\mathcal D_z$. Differentiating $\mathcal D_z\Psi=0$ in the identity $F=d\Psi^\dagger(1-\Psi\Psi^\dagger)\wedge d\Psi$ gives

$$
F=\Psi^\dagger d\mathcal D_z^\dagger(1_2\otimes f)\wedge d\mathcal D_z\Psi.
$$

The space-time [differential two-forms](../../../../../2-form.md) appearing here are generated by $dz_1\wedge d\bar z_1-dz_2\wedge d\bar z_2$, $dz_1\wedge d\bar z_2$, and $d\bar z_1\wedge dz_2$. For orientation $1234$ these are anti-self-dual. Hence the construction yields anti-self-dual [gauge connections](../../../../../connection-vector-bundle.md), of charge $k=-\ell$ in the present convention; the reversed construction gives positive charge. Regular ADHM data describe the smooth framed [instanton](../../../../../instanton.md) moduli, while degenerate rank conditions allow singular limits.

There are $4\ell^2+4\ell N$ real data parameters. The three real [matrix](../../../../../matrix.md) [moment map](../../../../../moment-map.md) equations impose $3\ell^2$ conditions, and quotient by $U(\ell)$ removes another $\ell^2$, giving $4\ell N$ dimensions at regular points. For $SU(2)$ this is $8\ell$ framed dimensions and $8\ell-3$ unframed dimensions on the irreducible locus. This explains how the one-instanton parameters fit into the higher-charge family.

The [Penrose-Ward correspondence](../../../../../penrose-ward-correspondence.md) provides a complementary description by [holomorphic vector bundles](../../../../../holomorphic-vector-bundle.md) on [twistor space](../../../../../twistor-space.md), trivial on the real [twistor lines](../../../../../twistor-line.md) for the Euclidean problem and equipped with the suitable reality structure. Triviality on every complexified line is a stronger condition and is not required for ordinary Euclidean [instantons](../../../../../instanton.md). Symmetry reductions of the anti-self-dual equations give integrable three-dimensional systems such as the [Bogomolny equations](../../../../../bogomolny-equations.md).

In the quantum theory, a Euclidean [instanton](../../../../../instanton.md) interpolates between [Yang-Mills vacua](../../../../../yang-mills-vacuum.md) of different [Chern-Simons number](../../../../../chern-simons-number-of-a-gauge-field.md). Choosing Euclidean time $x^1$ and spatial orientation $234$, its signed charge is the final [Chern-Simons number](../../../../../chern-simons-number-of-a-gauge-field.md) minus the initial one, so it describes [quantum tunnelling](../../../../../quantum-tunnelling.md) between winding sectors. Semiclassical contributions are suppressed by $\exp[-8\pi^2|k|/g^2]$; a [Yang-Mills theta term](../../../../../yang-mills-theta-term.md) adds a phase $\exp(i\vartheta k)$. One integrates over the [instanton](../../../../../instanton.md) [collective coordinates](../../../../../collective-coordinate-of-a-soliton.md) and includes fluctuation determinants rather than treating one classical solution as the entire quantum answer. [Instantons](../../../../../instanton.md) therefore connect finite-action classical geometry, topology of gauge bundles, exact nonlinear constructions, and nonperturbative quantum effects.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
