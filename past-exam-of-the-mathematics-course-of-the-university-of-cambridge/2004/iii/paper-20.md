# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper20.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $X\in\mathfrak g=T_eG$, let $X^L$ be the [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) with value $X$ at the identity. Its integral curve through the identity is the unique [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) $\gamma_X$ with $\gamma_X'(0)=X$. It exists for all real time: local existence followed by translation and the identity $\gamma_X(t+s)=\gamma_X(t)\gamma_X(s)$ extends it indefinitely. The [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) is

$$
\boxed{\exp X=\gamma_X(1),\qquad \exp(tX)=\gamma_X(t).}
$$

It is smooth and $d_0\exp=\operatorname{id}_{\mathfrak g}$, because differentiating $t\mapsto\exp(tX)$ at zero gives $X$. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) therefore makes it a local [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) at zero.

If $G$ is abelian, the product $t\mapsto\exp(tX)\exp(tY)$ is a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) with initial tangent $X+Y$. Uniqueness gives $\exp(t(X+Y))=\exp(tX)\exp(tY)$, hence

$$
\boxed{\exp(X+Y)=\exp X\exp Y.}
$$

Conversely, if this additive [homomorphism](../../../algebra.md#homomorphism) identity holds, all $\exp(tX)$ and $\exp(sY)$ commute. Differentiating their adjoint action shows $[X,Y]=0$. Alternatively, their commuting images contain an identity neighbourhood; that neighbourhood generates the [identity component of a Lie group](../../../lie-theory.md#identity-component-of-a-lie-group), so the [identity component](../../../geometry-and-topology.md#identity-component) is abelian. Conversely, if the [Lie algebra](../../../lie-algebra.md) is abelian, its [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) commute, so their flows commute. Hence all [one-parameter subgroups](../../../lie-theory.md#one-parameter-subgroup) commute; their product with initial tangent $X+Y$ is the [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) for $X+Y$. The [Lie exponential map](../../../lie-theory.md#exponential-map-of-a-lie-group) is therefore additive, and its image generates an abelian identity component. Thus **the stated equivalence holds for connected $G$**. Without connectedness the exact assertion is that the [Lie exponential map](../../../lie-theory.md#exponential-map-of-a-lie-group) is a [homomorphism](../../../algebra.md#homomorphism) precisely when $G^\circ$ is abelian. The converse implication to all of $G$ is false: in $O(2)$ the [Lie algebra](../../../lie-algebra.md) consists of $tJ$, where

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\exp(tJ)=R_t.
$$

Rotations satisfy $R_{t+s}=R_tR_s$, but a reflection $S$ satisfies $SR_tS^{-1}=R_{-t}$, so the full [orthogonal group](../../../linear-algebra.md#orthogonal-group) is not abelian.

Now take a connected [abelian Lie group](../../../lie-theory.md#abelian-lie-group) of dimension $n$. Its [Lie exponential map](../../../lie-theory.md#exponential-map-of-a-lie-group) is a [homomorphism](../../../algebra.md#homomorphism) whose image contains an identity neighbourhood, hence an open [subgroup](../../../group.md#subgroup). A connected [group](../../../group.md) has no proper open [subgroup](../../../group.md#subgroup), so this map is onto. Its kernel $\Lambda$ is discrete, since it is injective on a neighbourhood of zero. The induced map is a bijective [local diffeomorphism](../../../calculus.md#local-diffeomorphism) and therefore a [Lie group isomorphism](../../../lie-theory.md#lie-group-isomorphism)

$$
G\cong\mathbb R^n/\Lambda.
$$

Here is the needed classification of $\Lambda$. Let $r$ be the dimension of its real span. Choose $\lambda_1,\ldots,\lambda_r\in\Lambda$ that form a real basis of that span. Their [integer](../../../number-theory.md#integer) span $\Lambda_0$ has finite index in $\Lambda$: subtract [integer](../../../number-theory.md#integer) multiples of the $\lambda_i$ to put each [coset](../../../group-theory.md#coset) representative in a compact parallelepiped. Only finitely many points of $\Lambda$ lie there, since discreteness at zero gives a uniform positive separation between distinct points. Thus $\Lambda$ is finitely generated and torsion-free, and the [structure theorem for finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups) makes it free abelian of rank $r$. Its [integer](../../../number-theory.md#integer) basis is a real basis of the span. A linear change of coordinates consequently sends $\Lambda$ to $\mathbb Z^r\times\{0\}$ in $\mathbb R^n$.

This proves the [classification of connected abelian Lie groups](../../../lie-theory.md#classification-of-connected-abelian-lie-groups):

$$
\boxed{G\cong(\mathbb R/\mathbb Z)^r\times\mathbb R^{n-r}
=\mathbb T^r\times\mathbb R^s,\qquad r+s=n.}
$$

The isomorphism depends on the choice of lattice basis and complementary [vector space](../../../vector-space.md). Compactness is equivalent to $s=0$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [complex analytic Lie group](../../../lie-theory.md#complex-lie-group) is a [complex manifold](../../../complex-geometry.md#complex-manifold) whose multiplication and inversion are [holomorphic maps between complex manifolds](../../../complex-geometry.md#holomorphic-map-between-complex-manifolds). Its identity [tangent space](../../../differential-geometry.md#tangent-space) is a complex [Lie algebra](../../../lie-algebra.md), and the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group)

$$
\operatorname{Ad}:G\longrightarrow\operatorname{GL}_{\mathbb C}(\mathfrak g),\qquad
\operatorname{Ad}_g=d_e(h\mapsto ghg^{-1})
$$

is holomorphic: differentiating the holomorphic conjugation map with respect to its second variable gives holomorphically varying matrix entries.

Every scalar holomorphic [function](../../../function.md) on a compact connected [complex manifold](../../../complex-geometry.md#complex-manifold) is constant. Indeed its modulus attains a maximum; the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle), applied in complex coordinate charts and along complex lines, makes it locally constant there, and connectedness propagates that constancy. Apply this to each entry of $\operatorname{Ad}$. Since $\operatorname{Ad}_e=I$, it follows that $\operatorname{Ad}_g=I$ for every $g$. Differentiation gives

$$
\operatorname{ad}_X(Y)=[X,Y]=0.
$$

Thus $\mathfrak g$ is abelian, and the connected [group](../../../group.md) $G$ is abelian by the identity-neighbourhood argument in part (i). This proves that [compact connected complex Lie groups are complex tori](../../../lie-theory.md#compact-connected-complex-lie-groups-are-complex-tori).

If $n=\dim_{\mathbb C}G$, identify $\mathfrak g$ with $\mathbb C^n$. The [Lie exponential map](../../../lie-theory.md#exponential-map-of-a-lie-group) is holomorphic, additive, onto, and a local biholomorphism, by the holomorphic left-invariant differential equation and its identity derivative. Its kernel $B$ is a [discrete subgroup](../../../topological-group.md#discrete-subgroup) of the additive space $\mathbb C^n$. The induced map yields

$$
\boxed{G\cong\mathbb C^n/B}
$$

as complex [Lie groups](../../../lie-theory.md#lie-group), not merely as real [groups](../../../group.md). Compactness further forces $B$ to be a full-rank real lattice. If its real span $W$ were proper, projection would give a surjective continuous map $\mathbb C^n/B\to\mathbb R^{2n}/W$, contradicting compactness. The discrete-subgroup argument in part (i) therefore gives $B\cong\mathbb Z^{2n}$. The quotient is a [complex torus](../../../complex-geometry.md#complex-torus); it need not split into one-dimensional complex tori.

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Interpret $\theta$ as a continuous finite-dimensional complex [group representation](../../../representation-theory.md#group-representation), so its values lie in $\operatorname{GL}_{\mathbb C}(V)$, and interpret approximation in the [uniform norm](../../../functional-analysis.md#supremum-norm). Assume the usual Hausdorff convention for the compact topological [group](../../../group.md). The following argument proves the required form of the [Peter-Weyl theorem](../../../representation-theory.md#peter-weyl-theorem) without first assuming that $G$ is a [Lie group](../../../lie-theory.md#lie-group).

Start with normalized [Haar measure](../../../measure-theory.md#haar-measure). It is both left- and right-invariant on a compact [group](../../../group.md). Average any [Hermitian inner product](../../../linear-algebra.md#hermitian-form) to make a finite-dimensional representation unitary. The left regular action $L_a h(x)=h(a^{-1}x)$ is already unitary on $L^2(G)$.

Choose a continuous nonnegative [function](../../../function.md) $k$ supported in a small symmetric identity neighbourhood, with $k(z^{-1})=k(z)$ and $\int k=1$. Such [functions](../../../function.md) are obtained from a nonzero continuous bump near the identity, symmetrizing and normalizing. Define

$$
T_kh(x)=\int_Gk(y^{-1}x)h(y)\,dy
=\int_Gk(z)h(xz^{-1})\,dz.
$$

The [convolution](../../../fourier-analysis.md#convolution) operator $T_k$ commutes with [left translations](../../../lie-theory.md#left-and-right-translation-on-a-lie-group). Its continuous kernel is Hermitian, hence it is self-adjoint. It is compact on $L^2(G)$: approximate the continuous kernel uniformly by finite sums of separated [functions](../../../function.md) of $x$ and $y$, using the [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) on the compact product. The corresponding operators have finite rank and converge in operator norm. It also maps into $C(G)$ and satisfies

$$
\|T_kh\|_\infty\leq\|k\|_2\|h\|_2,
$$

by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality); continuity follows from the [uniform continuity](../../../topological-analysis.md#uniform-continuity) of the translated kernel.

The [spectral theorem for compact self-adjoint operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) decomposes the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of its kernel into finite-dimensional [eigenspaces](../../../linear-operator-theory.md#eigenspace) with nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Every such [eigenspace](../../../linear-operator-theory.md#eigenspace) is left-translation invariant, and all its elements are continuous, since $h=T_kh/\lambda$ there. If $W\subset C(G)$ is one of these invariant spaces, write $\rho(a)=L_a|_W$. Evaluation at the identity gives

$$
h(x)=\operatorname{ev}_e\bigl(\rho(x^{-1})h\bigr)
=\bigl(\rho^\vee(x)\operatorname{ev}_e\bigr)(h).
$$

Thus $h$ is a [matrix coefficient](../../../representation-theory.md#matrix-coefficient) of the [dual representation](../../../representation-theory.md#dual-representation). This identifies each finite spectral sum with finite-dimensional representation data.

To get uniform rather than just $L^2$ approximation, let $S_N$ project onto increasing finite sums of the nonzero [eigenspaces](../../../linear-operator-theory.md#eigenspace). For $f\in C(G)$, $T_kf$ is orthogonal to the kernel, so $S_NT_kf\to T_kf$ in $L^2$. Applying the displayed smoothing bound gives

$$
\|T_kS_NT_kf-T_k^2f\|_\infty\longrightarrow0.
$$

Meanwhile, choosing the support of $k$ sufficiently small makes $T_kf$ uniformly close to $f$, by [uniform continuity](../../../topological-analysis.md#uniform-continuity) under small translations. Since $\|T_k\|_{C\to C}\leq1$, it also makes $T_k^2f$ uniformly close to $f$. Every $T_kS_NT_kf$ belongs to a finite sum of invariant [eigenspaces](../../../linear-operator-theory.md#eigenspace), hence is a finite sum of [matrix coefficients](../../../representation-theory.md#matrix-coefficient). This completes the [convolution proof of uniform Peter-Weyl approximation](../../../representation-theory.md#convolution-proof-of-uniform-peter-weyl-approximation).

A coefficient $\ell(\theta(g)v)$ equals $\operatorname{tr}(\alpha\theta(g))$ for the rank-one [endomorphism](../../../algebra.md#endomorphism) $\alpha=v\otimes\ell$. Finite sums of coefficients can be combined using a direct-sum representation and a block-diagonal $\alpha$. Therefore the conclusion has exactly the requested form:

$$
\boxed{\text{For every }\varepsilon>0\text{ there are }V,\theta,\alpha
\text{ with }\sup_{g\in G}|f(g)-\operatorname{tr}(\alpha\theta(g))|<\varepsilon.}
$$

For a [class function](../../../representation-theory.md#class-function) $f$, apply [conjugation averaging on a compact group](../../../representation-theory.md#conjugation-averaging-on-a-compact-group),

$$
\mathcal AF(g)=\int_G F(hgh^{-1})\,dh.
$$

It fixes $f$ and is a contraction in the [uniform norm](../../../functional-analysis.md#supremum-norm), so averaging an approximation preserves its error bound. A [trace](../../../linear-algebra.md#matrix-trace) coefficient averages to $\operatorname{tr}(\overline\alpha\theta(g))$, where

$$
\overline\alpha=\int_G\theta(h)^{-1}\alpha\theta(h)\,dh.
$$

This [endomorphism](../../../algebra.md#endomorphism) commutes with the representation. A finite-dimensional [unitary representation](../../../representation-theory.md#unitary-representation) splits into irreducibles by repeatedly taking invariant orthogonal complements. On each irreducible diagonal block, [Schur lemma](../../../representation-theory.md#schur-s-lemma) makes its average a scalar multiple of the identity, namely its [trace](../../../linear-algebra.md#matrix-trace) divided by the block dimension. Off-diagonal blocks do not contribute to the total [trace](../../../linear-algebra.md#matrix-trace). Thus the averaged coefficient is a finite [linear combination](../../../vector-space.md#linear-combination) of [irreducible characters](../../../representation-theory.md#irreducible-character). Consequently **irreducible complex characters span a uniformly dense subspace of the continuous [class functions](../../../representation-theory.md#class-function)**.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

By part (i), finite-dimensional continuous [unitary representations](../../../representation-theory.md#unitary-representation) separate points of the compact [group](../../../group.md). More explicitly, if every representation sent some $g\ne e$ to the identity, all their [matrix coefficients](../../../representation-theory.md#matrix-coefficient) would take the same values at $g$ and $e$. Uniform density would force every continuous scalar [function](../../../function.md) to do so, contradicting separation of points on a compact Hausdorff space. Hence

$$
\bigcap_\theta\ker\theta=\{e\}.
$$

Each representation kernel is a closed [normal subgroup](../../../group-theory.md#normal-subgroup). We claim that the intersection can be reduced to finitely many kernels. Begin with $K_0=G$. If $K_j\ne\{e\}$, choose $g_j\in K_j\setminus\{e\}$ and a representation $\theta_{j+1}$ with $\theta_{j+1}(g_j)\ne I$. Then

$$
K_{j+1}=K_j\cap\ker\theta_{j+1}\subsetneq K_j.
$$

An indefinite continuation would violate the [descending chain condition](../../../algebra.md#descending-chain-condition) for [closed subgroups](../../../topological-group.md#closed-subgroup). Thus after finitely many steps, $K_N=\{e\}$.

The direct sum $\rho=\theta_1\oplus\cdots\oplus\theta_N$ is consequently a finite-dimensional [faithful representation](../../../representation-theory.md#faithful-representation), with continuous injective [homomorphism](../../../algebra.md#homomorphism)

$$
\rho:G\longrightarrow U(d).
$$

Compactness of $G$ makes this a homeomorphism onto a compact, hence closed, image. The [closed-subgroup theorem](../../../lie-theory.md#closed-subgroup-theorem) makes that image an embedded [Lie subgroup](../../../lie-theory.md#lie-subgroup) of the finite-dimensional unitary [group](../../../group.md). Transporting its smooth structure to $G$ proves

$$
\boxed{G\text{ is a compact Lie group.}}
$$

This is the mechanism behind the assertion that [compact groups with a descending chain condition are Lie groups](../../../topological-group.md#compact-groups-with-a-descending-chain-condition-are-lie-groups): the chain condition turns an arbitrarily large separating family into one finite-dimensional [faithful representation](../../../representation-theory.md#faithful-representation).

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Lie group–Lie algebra correspondence](../../../lie-theory.md#lie-group-lie-algebra-correspondence) separates local differential structure from global topology. For a [Lie group](../../../lie-theory.md#lie-group) $G$, define $LG=T_eG$ as a [real vector space](../../../vector-space.md#real-vector-space). Extend each $X\in T_eG$ to the [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field)

$$
X^L(g)=d_eL_g(X).
$$

The [commutator](../../../lie-algebra.md#commutator) of two such [vector fields](../../../calculus.md#vector-field) is again left-invariant. Set

$$
\boxed{[X,Y]=[X^L,Y^L](e).}
$$

The vector-field [commutator](../../../lie-algebra.md#commutator) is bilinear, antisymmetric and satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity), so this makes $T_eG$ a [Lie algebra](../../../lie-algebra.md). For a matrix [group](../../../group.md) this bracket is $XY-YX$.

For a smooth [Lie group homomorphism](../../../lie-theory.md#lie-group-homomorphism) $\phi:G_1\to G_2$, its differential at the identity is the [linear map](../../../vector-space.md#linear-map)

$$
L\phi=d_{e_1}\phi:\mathfrak g_1\longrightarrow\mathfrak g_2.
$$

The identity $\phi\circ L_g=L_{\phi(g)}\circ\phi$ shows that the corresponding left-invariant fields are $\phi$-related. Brackets of related [vector fields](../../../calculus.md#vector-field) are related, hence

$$
\boxed{L\phi([X,Y])=[L\phi(X),L\phi(Y)].}
$$

The chain rule also gives $L(\psi\circ\phi)=L\psi\circ L\phi$ and $L(\operatorname{id})=\operatorname{id}$. Thus differentiation is a functor from [Lie groups](../../../lie-theory.md#lie-group) and smooth [homomorphisms](../../../algebra.md#homomorphism) to real [Lie algebras](../../../lie-algebra.md) and bracket-preserving [linear maps](../../../vector-space.md#linear-map).

To see what information the differential retains, apply $\phi$ to a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup). Its initial tangent is $L\phi(X)$, so uniqueness yields

$$
\boxed{\phi(\exp X)=\exp(L\phi(X)).}
$$

If $G_1$ is connected, a small exponential neighbourhood generates it. Every $g\in G_1$ is a finite product $\exp X_1\cdots\exp X_k$, and therefore

$$
\phi(g)=\exp(L\phi(X_1))\cdots\exp(L\phi(X_k)).
$$

For an already existing [homomorphism](../../../algebra.md#homomorphism) this expression is independent of the chosen product because it equals $\phi(g)$. Two [homomorphisms](../../../algebra.md#homomorphism) with the same differential agree on that neighbourhood and hence everywhere. This proves that a [Lie group homomorphism determined by its differential](../../../lie-theory.md#lie-group-homomorphism-determined-by-its-differential) requires a connected source.

On a disconnected source only the restriction to $G_1^\circ$ is determined. For instance a nontrivial finite discrete [group](../../../group.md) has zero [Lie algebra](../../../lie-algebra.md), so its identity and trivial [endomorphisms](../../../algebra.md#endomorphism) have the same zero differential but are different maps. The discussion of all components must therefore include additional global data. The remaining parts explain the corresponding existence and topology conditions.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

An isomorphism of [Lie algebras](../../../lie-algebra.md) identifies the local multiplication laws of the identity components. In exponential coordinates the local product is governed by the [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula),

$$
\log(\exp X\exp Y)=X+Y+\frac12[X,Y]
+\frac1{12}[X,[X,Y]]+\frac1{12}[Y,[Y,X]]+\cdots.
$$

A bracket-preserving linear isomorphism carries this law to the corresponding law in the other [Lie algebra](../../../lie-algebra.md). Thus the identity components are locally isomorphic. This statement is local; the exponential coordinates need not cover the whole [group](../../../group.md).

The stronger global description uses a [universal covering Lie group](../../../lie-theory.md#universal-covering-lie-group). The [universal cover](../../../algebraic-topology.md#universal-cover) of a connected [Lie group](../../../lie-theory.md#lie-group) acquires a [group](../../../group.md) law by lifting multiplication with a chosen identity; uniqueness of lifts supplies associativity and inversion. The [covering map](../../../algebraic-topology.md#covering-space) is a [local diffeomorphism](../../../calculus.md#local-diffeomorphism) and a [Lie group homomorphism](../../../lie-theory.md#lie-group-homomorphism), with discrete kernel. That kernel is central: conjugation of one of its elements gives a continuous map from the connected covering [group](../../../group.md) into a discrete set, so it is constantly that element.

By integration of the given [Lie algebra isomorphism](../../../lie-algebra.md#lie-algebra-isomorphism) and its inverse on [simply connected](../../../algebraic-topology.md#simply-connected-space) covers, these covers are isomorphic. Their two compositions have identity differential and therefore are identity maps by the preceding uniqueness argument. Consequently, for some connected [simply connected](../../../algebraic-topology.md#simply-connected-space) [Lie group](../../../lie-theory.md#lie-group) $\widetilde G$,

$$
\boxed{G_1^\circ\cong\widetilde G/\Gamma_1,\qquad
G_2^\circ\cong\widetilde G/\Gamma_2,}
$$

where $\Gamma_1,\Gamma_2$ are discrete central [subgroups](../../../group.md#subgroup). Different quotients need not be isomorphic. The additive [group](../../../group.md) $\mathbb R$ and the [circle group](../../../lie-theory.md#circle-group) $\mathbb R/2\pi\mathbb Z$ have the same one-dimensional [Lie algebra](../../../lie-algebra.md) but different compactness and [fundamental groups](../../../algebraic-topology.md#fundamental-group). Another familiar pair is the [SU(2) group](../../../topological-group.md#su-2-group) and the [SO(3) group](../../../linear-algebra.md#so-3-group), with the latter the quotient of the former by $\{I,-I\}$.

Thus **isomorphic [Lie algebras](../../../lie-algebra.md) give isomorphic connected [simply connected](../../../algebraic-topology.md#simply-connected-space) [groups](../../../group.md), and identify arbitrary identity components up to discrete central quotients**. For disconnected [groups](../../../group.md) the [Lie algebra](../../../lie-algebra.md) also omits the [group](../../../group.md) of components and its conjugation and extension data. For example $\mathbb R\times F$, for any finite [group](../../../group.md) $F$, always has [Lie algebra](../../../lie-algebra.md) $\mathbb R$, while its component [group](../../../group.md) is $F$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a finite-dimensional real [Lie algebra](../../../lie-algebra.md) $\mathfrak h$, the [Lie third theorem](../../../lie-theory.md#lie-third-theorem) asserts the existence of a connected [simply connected](../../../algebraic-topology.md#simply-connected-space) [Lie group](../../../lie-theory.md#lie-group) whose [Lie algebra](../../../lie-algebra.md) is $\mathfrak h$. There are two complementary views of the construction.

Locally, the [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) defines multiplication on a sufficiently small neighbourhood of zero in $\mathfrak h$. Its leading terms are $X+Y+\tfrac12[X,Y]$, its identity is zero, and inversion is $X\mapsto-X$. The convergent BCH series in finite dimensions and the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) provide the local associative law. Continuing and globalizing this local [group](../../../group.md) gives its [simply connected](../../../algebraic-topology.md#simply-connected-space) integration; the globalization is a substantive step, rather than a claim that one exponential chart gives all of the [group](../../../group.md).

A matrix construction makes that global step more concrete. The [Ado theorem](../../../lie-algebra.md#ado-s-theorem) gives a faithful finite-dimensional representation

$$
\iota:\mathfrak h\hookrightarrow\mathfrak{gl}_N(\mathbb R).
$$

Consider the left-invariant distribution $D_A=A\iota(\mathfrak h)$ on $\operatorname{GL}_N(\mathbb R)$. It is involutive because $\iota(\mathfrak h)$ is closed under [commutators](../../../lie-algebra.md#commutator). The [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) integrates it to its connected leaf through the identity. This leaf carries the intrinsic immersed-submanifold structure of the connected [Lie subgroup](../../../lie-theory.md#lie-subgroup) generated by the matrix exponentials $e^{\iota(X)}$. Its tangent [Lie algebra](../../../lie-algebra.md) is exactly $\iota(\mathfrak h)$; multiplication and inversion preserve the leaf and give its [Lie group](../../../lie-theory.md#lie-group) operations. Call this immersed [group](../../../group.md) $H_0$.

Taking its [universal covering Lie group](../../../lie-theory.md#universal-covering-lie-group) gives

$$
\boxed{\operatorname{Lie}(\widetilde H_0)\cong\mathfrak h,\qquad
\widetilde H_0\text{ connected and simply connected}.}
$$

Ado's faithfulness matters: the adjoint representation alone loses central elements. Also, the [subgroup](../../../group.md#subgroup) generated by the exponentials need not be closed in the ambient matrix [group](../../../group.md). For an irrational $a$, the map $t\mapsto(R_t,R_{at})$ gives a dense one-dimensional immersed [subgroup](../../../group.md#subgroup) of the two-dimensional torus. Its intrinsic [group](../../../group.md) is $\mathbb R$, whereas its closure has a two-dimensional [Lie algebra](../../../lie-algebra.md). Taking an ambient closure in the construction would therefore be incorrect.

Finally, any other connected [Lie group](../../../lie-theory.md#lie-group) with [Lie algebra](../../../lie-algebra.md) $\mathfrak h$ is obtained from this [simply connected](../../../algebraic-topology.md#simply-connected-space) integration by a discrete central quotient, as in part (i). The [simply connected](../../../algebraic-topology.md#simply-connected-space) integration is unique up to isomorphism, but an arbitrary corresponding [group](../../../group.md) is not.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism) $\theta:\mathfrak g_1\to\mathfrak g_2$ always defines a local [group homomorphism](../../../group-theory.md#group-homomorphism) near the identities by the exponential charts:

$$
\phi(\exp X)=\exp(\theta X)
$$

for sufficiently small $X$. Preservation of the BCH multiplication law makes this a local [homomorphism](../../../algebra.md#homomorphism). The issue is extending it consistently around all paths and periods in the source.

Suppose first that $G_1$ is connected and [simply connected](../../../algebraic-topology.md#simply-connected-space). For a piecewise smooth path $\gamma:[0,1]\to G_1$ from $e_1$ to $g$, let

$$
A(t)=d_{\gamma(t)}L_{\gamma(t)^{-1}}\,\dot\gamma(t)
$$

be its left logarithmic velocity. Solve in $G_2$ the differential equation

$$
\dot\eta(t)=d_{e_2}L_{\eta(t)}\,\theta(A(t)),\qquad\eta(0)=e_2.
$$

The equation exists throughout the finite path interval: bounded smooth body velocity gives a uniform local existence interval at the identity, and [left translation](../../../lie-theory.md#left-and-right-translation-on-a-lie-group) repeatedly continues the solution. Define the proposed map by the endpoint $\Phi(g)=\eta(1)$.

Bracket preservation makes this endpoint invariant under fixed-endpoint [homotopy](../../../algebraic-topology.md#homotopy). To see the mechanism, for a two-parameter path write $A=\gamma^{-1}\partial_t\gamma$ and $B=\gamma^{-1}\partial_s\gamma$, using the [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) rather than literal multiplication for nonmatrix [groups](../../../group.md). The [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) gives

$$
\partial_sA-\partial_tB=[A,B].
$$

After applying $\theta$, the same identity holds for $a=\theta A$ and $b=\theta B$. If $c=\eta^{-1}\partial_s\eta$, the transport equation implies

$$
\partial_tc=\partial_sa-[a,c],\qquad
\partial_tb=\partial_sa-[a,b].
$$

Both have zero initial value because the path starts at a fixed identity. Uniqueness gives $c=b$. At the fixed endpoint, $B(s,1)=0$, hence $\partial_s\eta(s,1)=0$. The endpoint is therefore unchanged by the [homotopy](../../../algebraic-topology.md#homotopy). Simple connectedness then makes it independent of the chosen path.

For paths to $g$ and $h$, concatenate the first with the left translate by $g$ of the second. Its transported endpoint is $\Phi(g)\Phi(h)$, because left logarithmic velocity is unchanged by [left translation](../../../lie-theory.md#left-and-right-translation-on-a-lie-group). It follows that $\Phi(gh)=\Phi(g)\Phi(h)$. Near the identity, choose $\gamma(t)=\exp(tX)$; transport yields $\Phi(\exp X)=\exp(\theta X)$. Thus $\Phi$ is smooth near the identity and, by translation, everywhere, and its differential is $\theta$. The uniqueness argument from the root solution gives

$$
\boxed{\text{A connected simply connected source admits a unique global }\Phi\text{ with }d_e\Phi=\theta.}
$$

This is [integration of a Lie algebra homomorphism](../../../lie-algebra.md#integration-of-a-lie-algebra-homomorphism).

For a connected source that is not [simply connected](../../../algebraic-topology.md#simply-connected-space), first integrate $\theta$ on its [universal cover](../../../algebraic-topology.md#universal-cover) $p:\widetilde G_1\to G_1$. The resulting map $\widetilde\Phi:\widetilde G_1\to G_2$ descends exactly when

$$
\boxed{\widetilde\Phi(\ker p)=\{e_2\}.}
$$

Indeed two lifts of one element differ by a kernel element, so this condition is both necessary and sufficient for their images to agree. It is the [period obstruction to integration of a Lie algebra homomorphism](../../../lie-algebra.md#period-obstruction-to-integration-of-a-lie-algebra-homomorphism). For $G_1=G_2=S^1$, identify the [Lie algebras](../../../lie-algebra.md) with $\mathbb R$ and take $\theta(t)=ct$. The integrated map on the cover is $t\mapsto e^{ict}$, which respects the source period $2\pi$ precisely when $c\in\mathbb Z$. Therefore half-scaling is a valid [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism) but does not integrate to a circle [homomorphism](../../../algebra.md#homomorphism). If both [groups](../../../group.md) are written as [simply connected](../../../algebraic-topology.md#simply-connected-space) covers modulo central [subgroups](../../../group.md#subgroup), the equivalent descent condition is that the integrated cover map send $\Gamma_1$ into $\Gamma_2$.

For disconnected $G_1$, first solve this problem on $G_1^\circ$, obtaining $\phi_0$. One must then assign images $a_\gamma$ to representatives $s_\gamma$ of the component [group](../../../group.md). These assignments must satisfy the conjugation and multiplication relations. Explicitly, with $s_e=e$ and $s_\gamma s_\delta=s_{\gamma\delta}c_{\gamma,\delta}$ for $c_{\gamma,\delta}\in G_1^\circ$, the conditions are

$$
a_\gamma\phi_0(h)a_\gamma^{-1}
=\phi_0(s_\gamma h s_\gamma^{-1}),\qquad
a_\gamma a_\delta=a_{\gamma\delta}\phi_0(c_{\gamma,\delta}),\qquad a_e=e_2.
$$

When these can be solved, $\phi(s_\gamma h)=a_\gamma\phi_0(h)$ is a smooth global [homomorphism](../../../algebra.md#homomorphism). They may prevent existence or allow several extensions with the same differential. Thus **a bracket-preserving [linear map](../../../vector-space.md#linear-map) gives local data; global integration requires the source's periods and, when present, its component relations to be respected**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
