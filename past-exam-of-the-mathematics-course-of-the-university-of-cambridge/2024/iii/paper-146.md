# Paper 146

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_146.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_146.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 146](paper-146.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $J_0$ be the standard [complex structure](../../../complex-geometry.md#complex-structure) on $\mathbb R^{2n}$, let $\omega_0$ be the standard [symplectic form](../../../symplectic-geometry.md#symplectic-form), and let $g_0$ be the Euclidean [inner product](../../../linear-algebra.md#inner-product). They satisfy

$$
g_0(u,v)=\omega_0(u,J_0v),
\qquad
\omega_0(u,v)=g_0(J_0u,v).
$$

The [two-out-of-three property for unitary structures](../../../symplectic-geometry.md#two-out-of-three-property-for-unitary-structures) says that a real linear map preserving any two of these structures preserves the third. In terms of the corresponding [matrix groups](../../../group-theory.md#matrix-group),

$$
GL(n,\mathbb C)\cap Sp(2n,\mathbb R)
=Sp(2n,\mathbb R)\cap O(2n)
=O(2n)\cap GL(n,\mathbb C)
=U(n).
$$

For example, if $A$ preserves $J_0$ and $\omega_0$, then

$$
g_0(Au,Av)=\omega_0(Au,J_0Av)
=\omega_0(Au,AJ_0v)=g_0(u,v),
$$

so $A$ preserves $g_0$. If it preserves $J_0$ and $g_0$, the second displayed identity shows that it preserves $\omega_0$. Finally, $J_0$ is uniquely determined by $g_0(J_0u,v)=\omega_0(u,v)$, so preservation of $g_0$ and $\omega_0$ implies $AJ_0=J_0A$. The common intersection is therefore the [unitary group](../../../topological-group.md#unitary-group).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [unitary group](../../../topological-group.md#unitary-group) acts on the [Lagrangian Grassmannian](../../../symplectic-geometry.md#lagrangian-grassmannian) by $A\cdot L=A(L)$. Every Lagrangian subspace has an orthonormal basis, and adjoining its $J_0$-image gives a unitary basis, so this action is transitive. The stabilizer of the standard real subspace $\mathbb R^n\subset\mathbb C^n$ consists exactly of real unitary matrices, namely $O(n)$. Hence

$$
U(n)/O(n)\longrightarrow\operatorname{LGr}(\mathbb R^{2n}),
\qquad
A,O(n)\longmapsto A\mathbb R^n
$$

is a continuous bijection from a compact space to a Hausdorff space and is therefore a [homeomorphism](../../../topology.md#homeomorphism).

For $n=1$, every line in $\mathbb R^2$ is Lagrangian. Thus

$$
\operatorname{LGr}(\mathbb R^2)=\mathbb{RP}^1
\cong U(1)/O(1)=S^1/\{\pm1\}\cong S^1.
$$

Concretely, the line making angle $\theta$ with the real axis corresponds to $e^{2i\theta}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On the quotient from part (b), the [Maslov map](../../../symplectic-geometry.md#maslov-map)

$$
\mu:U(n)/O(n)\longrightarrow S^1,
\qquad
[A]\longmapsto\det(A)^2
$$

is well defined because $\det(Q)^2=1$ for $Q\in O(n)$. Consider the loop of [Lagrangian subspaces](../../../symplectic-geometry.md#lagrangian-subspace)

$$
\ell(t)=e^{\pi it}\mathbb R\oplus\mathbb R^{n-1},
\qquad 0\leq t\leq1.
$$

Its endpoints agree as unoriented subspaces, and $\mu\circ\ell(t)=e^{2\pi it}$ has degree one. If $\eta$ is the generator of $H^1(S^1;\mathbb Z)$, then

$$
\langle\mu^*\eta,[\ell]\rangle=1.
$$

Consequently $\mu^*\eta\ne0$, proving

$$
H^1(\operatorname{LGr}(\mathbb R^{2n});\mathbb Z)\ne0.
$$

The same integer is the [Maslov index](../../../symplectic-geometry.md#maslov-index) of $\ell$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Any [symplectic form](../../../symplectic-geometry.md#symplectic-form) on $S^2$ orients its [tangent bundle](../../../fiber-bundle.md#tangent-bundle). Choose a compatible [complex structure](../../../complex-geometry.md#complex-structure) and [inner product](../../../linear-algebra.md#inner-product); this reduces the structure group to $SO(2)$. Since every line in an oriented symplectic plane is Lagrangian,

$$
\mathcal LGr(TS^2)=\mathbb P(TS^2)
$$

is an oriented [circle bundle](../../../fiber-bundle.md#circle-bundle).

If a transition function of $TS^2$ rotates vectors through an angle $\alpha$, its action on unoriented lines rotates the coordinate $e^{2i\theta}$ through $2\alpha$. The [Euler class of the Lagrangian-line bundle of an oriented plane bundle](../../../symplectic-geometry.md#euler-class-of-the-lagrangian-line-bundle-of-an-oriented-plane-bundle) therefore gives

$$
e(\mathcal LGr(TS^2))=2e(TS^2).
$$

By the [Poincaré-Hopf theorem](../../../fiber-bundle.md#poincare-hopf-theorem),

$$
\langle e(TS^2),[S^2]\rangle=\chi(S^2)=2
$$

for the chosen orientation, up to changing both signs. Hence the Euler number of $\mathcal LGr(TS^2)$ is $\pm4$, which is nonzero. A smoothly trivial oriented circle bundle has zero [Euler class](../../../fiber-bundle.md#euler-class-of-a-vector-bundle), so $\mathcal LGr(TS^2)\to S^2$ cannot be smoothly trivial for any choice of symplectic form.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Take the [torus](../../../topology.md#torus)

$$
M=T^{2n}=\mathbb R^{2n}/\mathbb Z^{2n}
$$

with the translation-invariant [symplectic form](../../../symplectic-geometry.md#symplectic-form)

$$
\omega=\sum_{j=1}^n dx_j\wedge dy_j.
$$

The coordinate vector fields give a global symplectic frame of $TM$, so $TM$ is symplectically trivial. Passing fiberwise to the [Lagrangian Grassmannian bundle](../../../symplectic-geometry.md#lagrangian-grassmannian-bundle) gives

$$
\mathcal LGr(TM)\cong
T^{2n}\times\operatorname{LGr}(\mathbb R^{2n}),
$$

which is a smooth trivialization over the compact symplectic manifold $T^{2n}$.

## 2

↑ **Parent:** [Paper 146](paper-146.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Weinstein neighborhood theorem](../../../symplectic-geometry.md#weinstein-neighborhood-theorem) states that if $L$ is a compact [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) of $(M,\omega)$, then neighborhoods of $L$ in $M$ and of the zero section in its [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) $T^*L$ are [symplectomorphic](../../../symplectic-geometry.md#symplectomorphism). The symplectomorphism restricts to the identity on $L$, and the canonical form on $T^*L$ is taken with the sign matching the chosen convention.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take $L=S^2$. For any [Lagrangian embedding](../../../symplectic-geometry.md#lagrangian-embedding) of $S^2$ into a symplectic four-manifold, the symplectic form identifies the [normal bundle](../../../algebraic-geometry.md#normal-bundle) with $T^*S^2$. The [self-intersection formula](../../../algebraic-geometry.md#self-intersection-formula) and the [Euler characteristic](../../../homology.md#euler-characteristic) give

$$
[L]\cdot[L]
=\langle e(NL),[L]\rangle
=\langle e(T^*S^2),[S^2]\rangle
=2
$$

up to the harmless orientation sign. If a [smooth isotopy](../../../differential-geometry.md#smooth-isotopy) displaced $L$, its final image would represent the same homology class but have intersection number zero with $L$, a contradiction. This is the [smooth non-displaceability from self-intersection](../../../symplectic-geometry.md#smooth-non-displaceability-from-self-intersection).

For a compact ambient example, equip $S^2\times S^2$ with $\omega\oplus(-\omega)$. Its diagonal

$$
\Delta=\{(x,x):x\in S^2\}
$$

is Lagrangian because the two summands cancel on $T\Delta$, and the preceding argument shows that it is not smoothly displaceable.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $M=S^2$ with an area form and let $L$ be an equator dividing the sphere into two open hemispheres of equal area. Every curve in a [symplectic surface](../../../symplectic-geometry.md#symplectic-surface) is Lagrangian. A small normal push moves $L$ to a nearby latitude, so it is displaceable by a [smooth isotopy](../../../differential-geometry.md#smooth-isotopy).

Suppose a [symplectic isotopy](../../../symplectic-geometry.md#symplectic-isotopy) had final image $L'$ disjoint from $L$. The curve $L'$ must lie in one hemisphere. Of the two discs bounded by $L'$, the one contained in that hemisphere has area strictly below half the total area, and the other has area strictly above half. On the other hand, a symplectomorphism maps the original two hemispheres to the two discs bounded by $L'$ and preserves their areas, so both would have half the total area. This contradiction is the [symplectic non-displaceability of an area bisector](../../../symplectic-geometry.md#symplectic-non-displaceability-of-an-area-bisector).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let

$$
(M,\omega)=(T^2,dx\wedge dy),
\qquad
L=\{y=0\}.
$$

For any sufficiently small nonzero $\delta$, translation

$$
\phi_t(x,y)=(x,y+t\delta)
$$

is a [symplectic isotopy](../../../symplectic-geometry.md#symplectic-isotopy) with $\phi_1(L)\cap L=\varnothing$. Choosing $|\delta|$ arbitrarily small makes the isotopy arbitrarily small in every $C^k$ norm.

This isotopy has nonzero [flux homomorphism](../../../symplectic-geometry.md#flux-homomorphism), represented by $\delta\,dx$. In contrast, every [Hamiltonian isotopy](../../../symplectic-geometry.md#hamiltonian-isotopy) has zero flux. If a Hamiltonian image $L'$ were disjoint from $L$, the two homologous essential circles would bound an annulus $A$, and evaluation of the flux on $[L]$ would equal the signed symplectic area

$$
\int_A\omega,
$$

which is nonzero. This contradicts vanishing Hamiltonian flux, so $L$ is not Hamiltonian displaceable.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Again take a symplectic two-sphere, but let $L$ be a small latitude bounding a cap of area strictly below half the total area. A rotation carrying that cap to a disjoint cap carries $L$ to a disjoint Lagrangian circle. Rotations of the symplectic sphere are flows of [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field); for rotation about an axis, a height function is a [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function). Thus this rotation is a [Hamiltonian isotopy](../../../symplectic-geometry.md#hamiltonian-isotopy), and $L$ is Hamiltonian displaceable.

## 3

↑ **Parent:** [Paper 146](paper-146.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

[Moser's trick](../../../symplectic-geometry.md#moser-s-trick) states that if $M$ is compact and $\omega_t$, $0\leq t\leq1$, is a smooth family of [symplectic forms](../../../symplectic-geometry.md#symplectic-form) whose [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class is independent of $t$, then there is an [isotopy](../../../differential-geometry.md#isotopy) $\phi_t$ with

$$
\phi_t^*\omega_t=\omega_0.
$$

Since $[\dot\omega_t]=0$, choose a smooth family of one-forms $\sigma_t$ with $\dot\omega_t=d\sigma_t$. Nondegeneracy of $\omega_t$ uniquely determines a vector field $X_t$ by

$$
\iota_{X_t}\omega_t=-\sigma_t.
$$

Compactness makes its flow $\phi_t$ exist for the whole interval. [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) and $d\omega_t=0$ give

$$
\frac d{dt}\phi_t^*\omega_t
=\phi_t^*(\dot\omega_t+\mathcal L_{X_t}\omega_t)
=\phi_t^*(d\sigma_t+d\iota_{X_t}\omega_t)=0,
$$

which proves the theorem.

Smooth degree-$d$ hypersurfaces form the complement of the discriminant in the projective space of degree-$d$ homogeneous polynomials. This complement is path connected, so $X$ and $X'$ lie in a smooth one-parameter family. The [Ehresmann fibration theorem](../../../fiber-bundle.md#ehresmann-fibration-theorem) identifies the fibers smoothly. Under such an identification, the restrictions of the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) form a family $\omega_t$ whose cohomology class is the fixed restricted hyperplane class. Moser's trick therefore gives the [symplectic equivalence of smooth projective hypersurfaces](../../../symplectic-geometry.md#symplectic-equivalence-of-smooth-projective-hypersurfaces).

It remains to construct the finite subgroup for one convenient hypersurface. On the [Fermat hypersurface](../../../symplectic-geometry.md#fermat-hypersurface)

$$
X_F=\{z_0^d+\cdots+z_n^d=0\}\subset\mathbb{CP}^n,
$$

the group $(\mu_d)^{n+1}$ acts by diagonal coordinate multiplication. It preserves both $X_F$ and the Fubini-Study form. The kernel of its projective action is the diagonal subgroup $\mu_d$, so the effective [Fermat hypersurface diagonal symmetry](../../../symplectic-geometry.md#fermat-hypersurface-diagonal-symmetry) group is

$$
(\mathbb Z/d\mathbb Z)^{n+1}/\langle(1,\ldots,1)\rangle
\cong(\mathbb Z/d\mathbb Z)^n.
$$

Conjugating this action by a symplectomorphism $X_F\to X$ gives the required subgroup of $\operatorname{Symp}(X,\omega_{FS}|_X)$.

## 4

↑ **Parent:** [Paper 146](paper-146.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [symplectic neighborhood theorem](../../../symplectic-geometry.md#symplectic-neighborhood-theorem) says that a neighborhood of a compact [symplectic submanifold](../../../symplectic-geometry.md#symplectic-submanifold) is determined, up to symplectomorphism, by the restricted symplectic form and its [symplectic normal bundle](../../../symplectic-geometry.md#symplectic-normal-bundle). More precisely, if $f:S_0\to S_1$ is a symplectomorphism and an isomorphism of symplectic normal bundles covers $f$, then that bundle isomorphism extends to a symplectomorphism between neighborhoods of $S_0$ and $S_1$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $Q\subset\mathbb{CP}^2$ be a smooth complex conic. Its homology class is $2H$, so its [self-intersection number](../../../algebraic-geometry.md#self-intersection-number) is

$$
Q^2=(2H)^2=4.
$$

Rescale the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) so that $Q$ and $C$ have the same symplectic area. Their [normal bundles](../../../algebraic-geometry.md#normal-bundle) have opposite Euler numbers, $+4$ and $-4$, so the [symplectic sum](../../../symplectic-geometry.md#symplectic-sum) can be formed along $Q$ and $C$.

Concretely, remove tubular neighborhoods $\nu(C)$ and $\nu(Q)$ and glue the boundaries by a fiber-reversing bundle map. The [symplectic neighborhood theorem](../../../symplectic-geometry.md#symplectic-neighborhood-theorem) supplies the standard models needed for the gluing, and the symplectic-sum construction supplies a symplectic form on

$$
(X\setminus\nu(C))\cup_{L(4,1)}
(\mathbb{CP}^2\setminus\nu(Q)).
$$

The second piece is a rational homology ball. Thus this operation replaces the neighborhood of the $-4$ sphere by that rational ball and is the [symplectic rational blowdown of a minus-four sphere](../../../symplectic-geometry.md#symplectic-rational-blowdown-of-a-minus-four-sphere).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $F_0$ and $F_1$ be general homogeneous cubic forms with base locus $B$ of nine points. The incidence variety

$$
E(1)=\{([z],[s:t])\in\mathbb{CP}^2\times\mathbb{CP}^1:
sF_0(z)+tF_1(z)=0\}
$$

is the blowup of $\mathbb{CP}^2$ at $B$. Projection onto the second factor is the [elliptic fibration of the rational elliptic surface](../../../complex-geometry.md#elliptic-fibration-of-the-rational-elliptic-surface)

$$
\pi:E(1)\longrightarrow\mathbb{CP}^1,
\qquad
([z],[s:t])\longmapsto[s:t],
$$

and its fibers are connected plane cubics. Over any base point $p\in B$, the exceptional curve $E_p=\{p\}\times\mathbb{CP}^1$ maps isomorphically to the base, so it is a holomorphic section.

Write $H$ for the pullback of a line and $E_1,\ldots,E_9$ for the exceptional classes. The fiber class and the [canonical class of the rational elliptic surface](../../../complex-geometry.md#canonical-class-of-the-rational-elliptic-surface) are

$$
F=3H-\sum_{i=1}^9E_i,
\qquad
K_{E(1)}=-3H+\sum_{i=1}^9E_i=-F.
$$

The degree of $\pi|_C$ is $C\cdot F=d$. The [adjunction formula](../../../complex-geometry.md#adjunction-formula) now yields

$$
2g(C)-2=C^2+K_{E(1)}\cdot C=k-d.
$$

Therefore the [genus formula for a multisection of the rational elliptic surface](../../../complex-geometry.md#genus-formula-for-a-multisection-of-the-rational-elliptic-surface) is

$$
\boxed{g(C)=1+\frac{k-d}{2}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
