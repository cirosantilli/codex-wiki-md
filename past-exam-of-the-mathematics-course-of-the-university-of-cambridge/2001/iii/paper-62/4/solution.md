<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose Hermitian generators $T^a$ of the gauge [Lie algebra](../../../../../lie-algebra-split.md), with $[T^a,T^b]=if^{abc}T^c$, and write $A_\mu=A_\mu^aT^a$. For the usual compact gauge algebra choose $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$. More generally use a nondegenerate invariant [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) on the algebra in place of this trace contraction; a completely arbitrary component metric would not give gauge invariance.

A matter vector is useful to fix conventions: with $\psi'=U(x)\psi$ and $D_\mu=\partial_\mu-igA_\mu$, require $D_\mu'\psi'=U D_\mu\psi$. Acting on an arbitrary vector gives the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md)

$$
\boxed{A_\mu'=UA_\mu U^{-1}+\frac{i}{g}U\partial_\mu U^{-1},\qquad
D_\mu'=U D_\mu U^{-1}.}
$$

For $U=1+ig\theta+O(\theta^2)$ this becomes

$$
\delta A_\mu=D_\mu\theta=\partial_\mu\theta-ig[A_\mu,\theta],\qquad
(D_\mu\theta)^a=\partial_\mu\theta^a+gf^{abc}A_\mu^b\theta^c.
$$

Here the second $D_\mu$ denotes the induced [derivative](../../../../../derivative.md) in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md).

Define the curvature by $[D_\mu,D_\nu]=-igF_{\mu\nu}$. Expanding the [commutator](../../../../../commutator.md) derives

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu-ig[A_\mu,A_\nu],\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+gf^{abc}A_\mu^bA_\nu^c.
$$

Since [commutators](../../../../../commutator.md) of the transformed [derivatives](../../../../../derivative.md) conjugate, $F_{\mu\nu}'=UF_{\mu\nu}U^{-1}$. Cyclicity of the trace proves the [invariant bilinear-form construction of a Yang-Mills action](../../../../../invariant-bilinear-form-construction-of-a-yang-mills-action.md):

$$
\boxed{\mathcal L_{\rm YM}=-\frac12\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})
=-\frac14F_{\mu\nu}^aF^{a\mu\nu}.}
$$

For a general invariant form $h$, the corresponding proof is $h([\theta,X],Y)+h(X,[\theta,Y])=0$, applied to the two curvature factors. No matter field is required in this pure-gauge Lagrangian.

Introduce the adjoint [Faddeev-Popov ghost](../../../../../faddeev-popov-ghost.md) $c^a$ and antighost $\bar c^a$, independent Grassmann-odd scalar fields of [ghost numbers](../../../../../ghost-number.md) $+1$ and $-1$, together with the Grassmann-even [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $b^a$ of [ghost number](../../../../../ghost-number.md) zero. The bar labels the independent antighost, not an additional propagating complex-conjugate matter field. Choose a left [BRST symmetry](../../../../../brst-symmetry.md) differential:

$$
\boxed{sA_\mu^a=(D_\mu c)^a,\qquad
sc^a=-\frac g2f^{abc}c^bc^c,\qquad
s\bar c^a=b^a,\qquad sb^a=0.}
$$

It is an odd derivation: $s(XY)=(sX)Y+(-1)^{|X|}X(sY)$ for homogeneous [Grassmann parity](../../../../../grassmann-parity.md) $|X|$. The two relevant properties are $s\mathcal L_{\rm YM}=0$ and off-shell nilpotence $s^2=0$. The first is gauge invariance with parameter replaced by the ghost, and the second follows from the [Lie algebra](../../../../../lie-algebra-split.md)'s graded Jacobi identities. Thus

$$
s(\mathcal L_{\rm YM}+s\Psi)=s\mathcal L_{\rm YM}+s^2\Psi=0.
$$

Algebraically this holds for any $\Psi$; a physical gauge-fixing addition uses an odd [gauge-fixing fermion](../../../../../gauge-fixing-fermion.md) of [ghost number](../../../../../ghost-number.md) $-1$ so that $s\Psi$ is even and has [ghost number](../../../../../ghost-number.md) zero.

For [BRST-exact covariant gauge fixing](../../../../../brst-exact-covariant-gauge-fixing.md), choose

$$
\Psi=\bar c^a\left(\partial^\mu A_\mu^a+\frac12b^a\right).
$$

The [graded Leibniz rule](../../../../../graded-leibniz-rule.md) supplies the essential minus sign:

$$
s\Psi=b^a\partial^\mu A_\mu^a+\frac12b^ab^a-\bar c^a\partial^\mu(D_\mu c)^a.
$$

Use [Gaussian gauge fixing with an auxiliary field](../../../../../gaussian-gauge-fixing-with-an-auxiliary-field.md) to integrate $b$. Pointwise,

$$
b^aF^a+\frac12(b^a)^2=\frac12(b^a+F^a)^2-\frac12(F^a)^2,
\qquad F^a=\partial^\mu A_\mu^a.
$$

Translation of the regulated oscillatory Gaussian leaves only a field-independent normalization. The remaining Lagrangian is therefore

$$
\boxed{\mathcal L_{\rm YM}-\frac12(\partial^\mu A_\mu^a)^2
-\bar c^a\partial_\mu(D^\mu c)^a.}
$$

This is covariant [Feynman gauge](../../../../../feynman-gauge.md), with gauge parameter one. Eliminating $b$ need not retain manifest off-shell nilpotence in the reduced field variables; the original auxiliary-field action gives the off-shell [BRST symmetry](../../../../../brst-symmetry.md) formulation.

Finally, the ungauge-fixed quadratic [momentum](../../../../../momentum.md) kernel is

$$
Q_{\mu\nu}^{ab}(p)=\delta^{ab}(-p^2\eta_{\mu\nu}+p_\mu p_\nu),\qquad
Q_{\mu\nu}^{ab}p^\nu=0.
$$

Gauge directions are null vectors, so there is no inverse defining a vector [propagator](../../../../../propagator.md), and the functional integral also counts an infinite [gauge orbit](../../../../../gauge-orbit.md) volume. The added gauge-fixing term cancels the longitudinal part, leaving $Q_{\mu\nu}^{ab}=-\delta^{ab}p^2\eta_{\mu\nu}$. With the vacuum prescription, the [propagators](../../../../../propagator.md) are

$$
\boxed{\langle A_\mu^a A_\nu^b\rangle(p)=-\frac{i\delta^{ab}\eta_{\mu\nu}}{p^2+i0},\qquad
\langle c^a\bar c^b\rangle(p)=\frac{i\delta^{ab}}{p^2+i0}.}
$$

The ghost action represents the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) and supplies ghost-vector vertices; closed ghost loops have the fermionic minus sign. Expanding the cubic and quartic Yang-Mills terms and this ghost interaction now defines consistent perturbative [Feynman rules](../../../../../feynman-rule.md). Physical mass-shell poles remain, whereas the gauge degeneracy has been removed. Possible global gauge-fixing obstructions and boundary zero modes are separate from the perturbative inverse around the trivial vacuum.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
