# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper20.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $\Phi_t$ be the local [flow of a vector field](../../../calculus.md#flow-of-a-vector-field) $V$. The [Lie derivative of a differential form](../../../differential-form.md#lie-derivative-of-a-differential-form) is $\mathcal L_V\eta=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*\eta$. We prove [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula)

$$
\mathcal L_V=d\iota_V+\iota_Vd.
$$

Both sides are degree-zero [derivations of an algebra](../../../associative-algebra.md#derivation-of-an-algebra) on the [exterior algebra](../../../linear-algebra.md#exterior-algebra) of [differential forms](../../../differential-form.md). They agree on a [function](../../../function.md) $f$, since $\iota_Vdf=V(f)$. They also agree on $df$: pullback commutes with the [exterior derivative](../../../differential-form.md#exterior-derivative), so $\mathcal L_Vdf=d(Vf)$, while $(d\iota_V+\iota_Vd)df=d(Vf)$. Locally every [differential form](../../../differential-form.md) is a sum of products of [functions](../../../function.md) and coordinate differentials, proving the identity in every degree.

For a compactly supported [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) $V_H$, take the convention $\iota_{V_H}\omega=-dH$. Since $d\omega=0$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives $\mathcal L_{V_H}\omega=0$, so its complete [flow of a vector field](../../../calculus.md#flow-of-a-vector-field) consists of [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism). Given $p$ and $v\in T_pM$, a [bump function](../../../analysis.md#bump-function) lets us choose a compactly supported $H$ with $dH_p=-\iota_v\omega_p$, and hence $V_H(p)=v$. Choose such fields for a [basis](../../../vector-space.md#basis) of $T_pM$. Their successive small-time flows give a map with invertible derivative at the origin. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes the orbit of $p$ open. Every orbit is open; because $M$ is [connected](../../../geometry-and-topology.md#connected-space), there is only one orbit. Thus **the compactly supported symplectomorphisms act transitively on points**, by [Hamiltonian transitivity on a connected symplectic manifold](../../../symplectic-geometry.md#hamiltonian-transitivity-on-a-connected-symplectic-manifold).

On the unit [sphere](../../../geometry-and-topology.md#sphere), the standard [symplectic area](../../../symplectic-geometry.md#symplectic-area) is $4\pi$. The equator has complementary disks of areas $2\pi,2\pi$, whereas the latitude at height $1/2$ has complementary disks of areas $\pi,3\pi$: the cap above height $h$ has area $2\pi(1-h)$. A [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) must preserve the unordered pair of complementary areas. Therefore **no such symplectomorphism exists**, by [complementary areas obstruct symplectic equivalence of separating curves](../../../symplectic-geometry.md#complementary-areas-obstruct-symplectic-equivalence-of-separating-curves).

<a id="1/image-complementary-sphere-areas-distinguish-the-equator-from-the-latitude-at-height-one-half"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-20-sphere-area-obstruction.png)

**[Figure 1](#1/image-complementary-sphere-areas-distinguish-the-equator-from-the-latitude-at-height-one-half). Complementary sphere areas distinguish the equator from the latitude at height one half**.

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [symplectic neighborhood theorem](../../../symplectic-geometry.md#symplectic-neighborhood-theorem) says that a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) between compact [symplectic submanifolds](../../../symplectic-geometry.md#symplectic-submanifold), together with a [symplectic vector bundle](../../../fiber-bundle.md#symplectic-vector-bundle) isomorphism of their [symplectic normal bundles](../../../symplectic-geometry.md#symplectic-normal-bundle), extends to a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) of neighborhoods. To outline the proof, use [tubular neighborhoods](../../../differential-geometry.md#tubular-neighborhood) to extend the bundle identification smoothly. The two pulled-back [symplectic forms](../../../symplectic-geometry.md#symplectic-form) agree as bilinear forms along the zero section. The [relative Poincaré lemma](../../../differential-form.md#relative-poincare-lemma) writes their difference as $d\alpha$, with $\alpha$ vanishing there. Their linear interpolation $\omega_t$ remains [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) on a sufficiently small neighborhood. Solving

$$
\iota_{V_t}\omega_t=-\alpha
$$

and integrating $V_t$ gives the [relative Moser theorem](../../../symplectic-geometry.md#relative-moser-theorem); the flow fixes the submanifold and carries one form to the other.

For the [symplectic fiber sum along a square-zero surface](../../../symplectic-geometry.md#symplectic-fiber-sum-along-a-square-zero-surface), the [self-intersection](../../../algebraic-geometry.md#self-intersection-number) is the [Euler number](../../../fiber-bundle.md#euler-number-of-a-vector-bundle) of the oriented rank-two [normal bundle](../../../algebraic-geometry.md#normal-bundle). Thus each normal bundle is trivial. Rescale one ambient [symplectic form](../../../symplectic-geometry.md#symplectic-form) if necessary to equalize the areas of the two copies of $C$. The [Moser theorem](../../../symplectic-geometry.md#moser-s-trick) for the surface then supplies a base identification preserving their area forms. The [symplectic neighborhood theorem](../../../symplectic-geometry.md#symplectic-neighborhood-theorem) identifies each neighborhood with a product carrying

$$
\omega_C+\frac12d(r^2)\wedge d\theta.
$$

Remove small disk neighborhoods and glue collars with the base identification and

$$
\theta_Y=-\theta_X,\qquad
r_Y^2=a-r_X^2
$$

for a suitable positive constant $a$. Both signs reverse, so the normal two-forms match; the base forms already match. They define a closed [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) two-form across the neck, agreeing with the ambient forms elsewhere. This constructs the [symplectic sum](../../../symplectic-geometry.md#symplectic-sum). Its construction uses the area normalization and the chosen normal-bundle gluing.

For a smooth counterexample, take $X=Y=\mathbb{CP}^2$, and in a small four-ball in each choose an unknotted [sphere](../../../geometry-and-topology.md#sphere) bounding a three-ball. These spheres are [null-homologous](../../../homology.md#null-homologous-cycle) and have [self-intersection](../../../algebraic-geometry.md#self-intersection-number) zero. Their standard smooth fiber sum is

$$
Z\cong\mathbb{CP}^2\mathbin{\#}\mathbb{CP}^2
\mathbin{\#}(S^1\times S^3).
$$

Indeed, the complement of the standard $S^2\times D^2$ in $S^4$ is $S^1\times D^3$; doubling these complements gives $S^1\times S^3$, and the two ambient projective-plane summands remain as [connected sums](../../../differential-geometry.md#connected-sum-of-oriented-manifolds). This is the [smooth fiber sum along unknotted null-homologous spheres](../../../topology.md#smooth-fiber-sum-along-unknotted-null-homologous-spheres).

In the induced [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), both summands in $Z=\mathbb{CP}^2\#(\mathbb{CP}^2\#(S^1\times S^3))$ have positive [positive index of the intersection form](../../../homology.md#positive-index-of-the-intersection-form). The [symplectic connected-sum obstruction](../../../topology.md#symplectic-connected-sum-obstruction) therefore rules out a [symplectic form](../../../symplectic-geometry.md#symplectic-form): connected-sum vanishing of the [Seiberg–Witten invariant of a four-manifold](../../../topology.md#seiberg-witten-invariant-of-a-four-manifold) contradicts [Taubes nonvanishing theorem](../../../topology.md#taubes-nonvanishing-theorem). In the opposite orientation the [intersection form](../../../homology.md#intersection-form) is negative definite, also ruling out a [symplectic form](../../../symplectic-geometry.md#symplectic-form), whose class has positive square. Thus **the smooth fiber sum need not be symplectic**.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [symplectic blowup](../../../symplectic-geometry.md#symplectic-blowup) replaces a small [symplectic ball](../../../symplectic-geometry.md#symplectic-ball) around the point by an [exceptional divisor](../../../complex-geometry.md#exceptional-divisor) $\mathbb{CP}^{n-1}$, for $\dim_{\mathbb R}X=2n$. One can construct its form by [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction). In a [Darboux chart](../../../symplectic-geometry.md#darboux-chart), consider $\mathbb C^n\times\mathbb C$ with the [circle action](../../../group-theory.md#circle-action)

$$
e^{it}\cdot(z,w)=(e^{it}z,e^{-it}w),
\qquad \mu(z,w)=\frac{|z|^2-|w|^2}{2}.
$$

On $\mu^{-1}(R^2/2)$ the action is free because $z\ne0$. Its quotient therefore carries a smooth [symplectic form](../../../symplectic-geometry.md#symplectic-form). Where $w\ne0$, choose the representative with $w$ positive real; the reduced form is the original form on $|z|>R$. Where $w=0$, the quotient is the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration) quotient of $|z|=R$, namely $\mathbb{CP}^{n-1}$. The local quotient is the tautological complex line bundle near its zero section, hence the local blowup. Glue this model to the exterior of the ball to obtain a [symplectic form](../../../symplectic-geometry.md#symplectic-form) on the blowup.

The area of a projective line in the exceptional divisor is $\varepsilon=\pi R^2$. For a closed $X$, changing this size changes the [symplectic volume](../../../symplectic-geometry.md#symplectic-volume):

$$
\operatorname{Vol}(\widetilde X,\widetilde\omega)
=\operatorname{Vol}(X,\omega)-\frac{\varepsilon^n}{n!}.
$$

Consequently **the blowup is not determined up to symplectomorphism without a size choice**. The underlying smooth blowup is fixed, but the symplectic construction has a parameter, as in [symplectic blowup size changes volume](../../../symplectic-geometry.md#symplectic-blowup-size-changes-volume).

For the blowdown map $\pi$ and exceptional divisor $E$, the [First Chern class](../../../complex-geometry.md#first-chern-class) is

$$
\boxed{c_1(T\widetilde X)=\pi^*c_1(TX)-(n-1)\operatorname{PD}[E]}.
$$

In real dimension four this becomes $\pi^*c_1(TX)-\operatorname{PD}[E]$, the [first Chern class formula for a symplectic blowup](../../../symplectic-geometry.md#first-chern-class-formula-for-a-symplectic-blowup).

The tangent bundle of the standard four-[torus](../../../topology.md#torus) is a trivial complex rank-two bundle, so its [symplectic canonical class](../../../complex-geometry.md#symplectic-canonical-class) is zero. For a generic fiber $F$ of a symplectic [Lefschetz pencil](../../../symplectic-geometry.md#lefschetz-pencil), the [symplectic adjunction formula](../../../symplectic-geometry.md#symplectic-adjunction-formula) gives $2g-2=F^2$. Two generic fibers intersect precisely at the base points, each with local [intersection number](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) one in the pencil model $[z_1:z_2]$. Hence

$$
\boxed{\#\{\text{base points}\}=F^2=2g-2}.
$$

This is [base-point count for a Lefschetz pencil on a symplectic four-torus](../../../symplectic-geometry.md#base-point-count-for-a-lefschetz-pencil-on-a-symplectic-four-torus).

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) $J$ is compatible with $\omega$ if $J^2=-I$, $\omega(Ju,Jv)=\omega(u,v)$, and $g_J(u,v)=\omega(u,Jv)$ is a positive-definite [inner product](../../../linear-algebra.md#inner-product). To construct one, choose a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $h$ and define $A$ by $h(Au,v)=\omega(u,v)$. The map $A$ is invertible and [skew-adjoint](../../../functional-analysis.md#skew-adjoint-generator), so $-A^2$ is positive definite. Its positive square root $P=(-A^2)^{1/2}$ commutes with $A$, and

$$
J=AP^{-1},\qquad
J^2=-I,\qquad
\omega(u,Jv)=h(u,Pv)>0\quad(u=v\ne0).
$$

The same identities show that $J$ preserves $\omega$. The positive square root depends smoothly on $A$, giving a smooth [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure).

For a compatible $J$, applying this [metric construction of a compatible almost complex structure](../../../complex-geometry.md#metric-construction-of-a-compatible-almost-complex-structure) to $g_J$ returns $J$. Given $J_0,J_1$, apply it to $(1-t)g_{J_0}+tg_{J_1}$ to obtain a path joining them. In fact interpolation to any fixed auxiliary metric gives a contraction. Thus **the space is nonempty and connected**, and even [contractible](../../../algebraic-topology.md#contractible-space), by [contractibility of compatible almost complex structures](../../../complex-geometry.md#contractibility-of-compatible-almost-complex-structures).

[Regularity of a J-holomorphic curve](../../../symplectic-geometry.md#regularity-of-a-j-holomorphic-curve) $u$ means that its linearized [Cauchy–Riemann operator](../../../symplectic-geometry.md#cauchy-riemann-operator) $D_u$ is [surjective](../../../algebra.md#surjective-function). Differentiating in coordinates gives

$$
D_u\xi=\partial_s\xi+J(u)\partial_t\xi
+(dJ)_u(\xi)\partial_tu,
$$

up to the harmless factor $1/2$ in the convention for $\bar\partial_J$. For constant $u$, the last term vanishes, $J(u)$ is constant, and the pulled-back tangent bundle is $\mathbb{CP}^1\times T_{u}M$. Identifying $T_uM$ with $\mathbb C^n$, this is a direct sum of $n$ copies of the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) on the trivial line bundle. Its cokernel is $H^{0,1}(\mathbb{CP}^1,\mathcal O)=0$, by [Dolbeault cohomology of the projective line](../../../complex-geometry.md#dolbeault-cohomology-of-the-projective-line). Hence constant maps are regular for every compatible $J$.

The [Energy identity for a J-holomorphic curve](../../../symplectic-geometry.md#energy-identity-for-a-j-holomorphic-curve) says that the energy is $\int_{\mathbb{CP}^1}u^*\omega$. If the [homology class](../../../homology.md#homology-class) is zero, this integral is zero, forcing $du=0$. Thus **every zero-class sphere is constant and regular**.

In real dimension four, the [Fredholm index](../../../functional-analysis.md#fredholm-index) of the parametrized sphere operator is $4+2c_1(A)$. At a regular nonconstant sphere, quotienting by the six-dimensional [Möbius transformation](../../../group-theory.md#mobius-transformation) group gives a local moduli space, or an orbifold for finite stabilizers, of real dimension

$$
\boxed{2c_1(A)-2}.
$$

This is the [dimension formula for regular J-holomorphic spheres](../../../symplectic-geometry.md#dimension-formula-for-regular-j-holomorphic-spheres).

For a [simple J-holomorphic sphere](../../../symplectic-geometry.md#simple-j-holomorphic-sphere) in class $A$, the [adjunction inequality for a simple J-holomorphic sphere](../../../symplectic-geometry.md#adjunction-inequality-for-a-simple-j-holomorphic-sphere) gives $c_1(A)\leq A^2+2$. If $A^2\leq-2$, the displayed moduli dimension is negative, so such a regular [simple J-holomorphic sphere](../../../symplectic-geometry.md#simple-j-holomorphic-sphere) cannot exist. To cover nonsimple maps as well, interpret regularity here as regularity for all nonconstant maps under discussion. A degree-$m$ cover, $m\geq2$, of a [simple J-holomorphic sphere](../../../symplectic-geometry.md#simple-j-holomorphic-sphere) in class $B$ has $A=mB$, with $B^2\leq-1$ and $c_1(B)\leq1$. Its local family of [rational covering maps of the projective line](../../../isolated-singularity.md#rational-covering-maps-of-the-projective-line) modulo domain reparametrization has real dimension $4m-4$, while the predicted dimension is

$$
2m\,c_1(B)-2\leq2m-2<4m-4.
$$

It therefore cannot be regular. This proves **there are no regular spheres in a class with square at most minus two**, by [negative-square exclusion under full sphere regularity](../../../symplectic-geometry.md#negative-square-exclusion-under-full-sphere-regularity). Regularity only for simple curves would not suffice: multiple covers of an exceptional minus-one sphere are the counterexample.

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [symplectic capacity](../../../symplectic-geometry.md#symplectic-capacity) assigns $c(X,\omega)\in[0,\infty]$ to [symplectic manifolds](../../../symplectic-geometry.md#symplectic-manifold) in a fixed dimension, is monotone under [symplectic embeddings](../../../symplectic-geometry.md#symplectic-embedding), satisfies $c(X,a\omega)=a\,c(X,\omega)$ for $a>0$, and is nontrivial in the sense that

$$
0<c(B^{2n}(1))\leq c(B^2(1)\times\mathbb R^{2n-2})<\infty.
$$

The second domain is the standard [symplectic cylinder](../../../symplectic-geometry.md#symplectic-cylinder). A [normalized symplectic capacity](../../../symplectic-geometry.md#normalized-symplectic-capacity) assigns $\pi$ to both unit domains, hence $\pi R^2$ to both radius-$R$ domains. The general axioms already give invariance under [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism) and quadratic scaling under coordinate dilation. For the rigidity argument, use the assumed existence of capacities in each dimension, including after adding a symplectic plane; normalization is not needed.

Let $\phi_j$ be [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism) converging locally uniformly to a smooth [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $\phi$. Work in [Darboux charts](../../../symplectic-geometry.md#darboux-chart). For a sufficiently small [solid ellipsoid](../../../geometry-and-topology.md#solid-ellipsoid) $E$ centered at a chosen point and $0<a<1$, uniform convergence and [degree of a continuous mapping](../../../homology.md#degree-of-a-continuous-mapping) give, for large $j$,

$$
\phi_j(aE)\subseteq\phi(E)\subseteq\phi_j(a^{-1}E).
$$

For the second inclusion, $\phi^{-1}\phi_j$ is uniformly close to the identity on the larger ellipsoid. Its boundary stays outside $\overline E$ and is homotopic there to the identity, so it has degree one about every point of $E$ and must cover $E$. Monotonicity and scaling now give $a^2c(E)\leq c(\phi(E))\leq a^{-2}c(E)$. Letting $a$ tend to one proves [capacity preservation under uniform limits](../../../symplectic-geometry.md#capacity-preservation-under-uniform-limits).

At the chosen point, write $T=D\phi$. The rescaled maps $(\phi(tz)-\phi(0))/t$ preserve capacities of ellipsoids and converge uniformly on compact sets to $T$. Applying the same sandwich argument proves that $T$ preserves the capacities of all [solid ellipsoids](../../../geometry-and-topology.md#solid-ellipsoid); so does $T^{-1}$.

We prove the required [linear capacity rigidity](../../../symplectic-geometry.md#linear-capacity-rigidity) explicitly. Write the standard [symplectic form](../../../symplectic-geometry.md#symplectic-form) as $\Omega$. Suppose $\Omega(u,v)=1$ and

$$
0<|\Omega(T^Tu,T^Tv)|=\lambda^2<1.
$$

Complete $u,v$ to a [symplectic basis](../../../linear-algebra.md#symplectic-basis), and complete $T^Tu/\lambda$, with the appropriately signed $T^Tv/\lambda$, to another [symplectic basis](../../../linear-algebra.md#symplectic-basis). If their basis matrices are $P,P'$, then $A=(P')^{-1}T^TP$ has first two columns $\lambda e_1,\pm\lambda f_1$. Hence $A^T$ sends the unit ball into the [symplectic cylinder](../../../symplectic-geometry.md#symplectic-cylinder) of radius $\lambda$. This matrix differs from $T$ by symplectic linear maps, so it preserves capacities of ellipsoids. Its first coordinate pair is multiplied by $\lambda$, with a possible sign, and therefore $(A^T)^k$ sends the unit ball into the cylinder of radius $\lambda^k$. Monotonicity gives

$$
0<c(B^{2n}(1))\leq\lambda^{2k}c(Z^{2n}(1))
$$

for every $k$, contradicting finiteness of the right-hand unit-cylinder capacity as $k$ tends to infinity. For a normalized capacity, the first iterate already gives the contradiction.

A zero pairing is handled by a small perturbation of $u,v$. A pairing of absolute value greater than one gives the same contradiction for $T^{-1}$, after normalizing the transformed pair. Thus

$$
|\Omega(T^Tu,T^Tv)|=|\Omega(u,v)|
$$

for every pair. The squared bilinear forms agree, so their difference times their sum is the zero polynomial. The real polynomial ring is an [integral domain](../../../commutative-algebra.md#integral-domain); consequently one factor vanishes identically. Therefore $T$ is either symplectic or [anti-symplectic](../../../symplectic-geometry.md#anti-symplectic-map).

To eliminate the negative sign, repeat the argument for $\phi_j\times\operatorname{id}_{\mathbb R^2}$, which are [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism) for $\omega\oplus\omega_{\mathbb R^2}$. If $\phi^*\omega=-\omega$ at the chosen point, the limit pulls this product form back to $-\omega\oplus\omega_{\mathbb R^2}$, which is neither the product form nor its negative. This contradicts the preceding derivative classification. Thus $\phi^*\omega=\omega$ everywhere. We have proved the [Eliashberg–Gromov rigidity theorem](../../../symplectic-geometry.md#eliashberg-gromov-rigidity-theorem): **the symplectomorphism group is closed in the $C^0$ topology on diffeomorphisms**.

Finally put $E=W^\perp$, with perpendicularity taken for the standard Euclidean [inner product](../../../linear-algebra.md#inner-product). Its dimension is two, so being nonisotropic means that the restricted [symplectic form](../../../symplectic-geometry.md#symplectic-form) is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form). For the standard compatible complex structure $J$, $W^\omega=JE$. If $Jv\in W\cap JE$, then $v\in E$ and $\omega(v,e)=0$ for every $e\in E$, forcing $v=0$. Thus $W$ is a [symplectic subspace](../../../linear-algebra.md#symplectic-subspace) and admits a [symplectic basis](../../../linear-algebra.md#symplectic-basis) extended to the whole space.

In the resulting linear symplectic coordinates, $W$ is $\{q_1=p_1=0\}$. The projection of the bounded set $U$ to the $(q_1,p_1)$ plane is bounded, so $U+W$ lies in a [symplectic cylinder](../../../symplectic-geometry.md#symplectic-cylinder) of some finite radius $R$. As $U$ is nonempty and open, it contains a ball of some radius $r>0$, which is also contained in $U+W$. Monotonicity and scaling give

$$
\boxed{0<r^2c(B^{2n}(1))\leq c(U+W)\leq R^2c(Z^{2n}(1))<\infty},
$$

as in [capacity of a bounded set thickened by a symplectic subspace](../../../symplectic-geometry.md#capacity-of-a-bounded-set-thickened-by-a-symplectic-subspace). For a [normalized symplectic capacity](../../../symplectic-geometry.md#normalized-symplectic-capacity), the two bounds simplify to $\pi r^2$ and $\pi R^2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
