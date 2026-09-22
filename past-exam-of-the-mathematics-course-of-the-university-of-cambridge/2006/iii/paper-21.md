# Paper 21

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper21.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper21.pdf)

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

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $L=L_1\cap L_2$, and let $j:L\hookrightarrow M$ be inclusion. The [transverse intersection theorem](../../../differential-geometry.md#transverse-intersection-theorem) makes $L$ a smooth [submanifold](../../../differential-geometry.md#submanifold) without boundary, with

$$
T_xL=T_xL_1\cap T_xL_2,\qquad
\operatorname{codim}_{\mathbb R}L
=\operatorname{codim}_{\mathbb R}L_1+\operatorname{codim}_{\mathbb R}L_2.
$$

It is compact because it is a closed subset of either compact input [submanifold](../../../differential-geometry.md#submanifold).

Write $\nu_r=TM|_{L_r}/TL_r$. On $L$, consider the bundle map

$$
TM|_L\longrightarrow\nu_1|_L\oplus\nu_2|_L,\qquad
v\longmapsto(v\bmod TL_1,\ v\bmod TL_2).
$$

Its kernel is $TL$, and it is onto because $TL_1+TL_2=TM$ at every intersection point. Thus the [normal bundle of a transverse intersection](../../../algebraic-geometry.md#normal-bundle-of-a-transverse-intersection) has the actual bundle isomorphism

$$
\nu(j)\cong\nu_1|_L\oplus\nu_2|_L.
$$

Transfer the direct-sum [complex structure](../../../complex-geometry.md#complex-structure) $J_1\oplus J_2$ through this isomorphism. This supplies a [complex structure](../../../complex-geometry.md#complex-structure) on the [normal bundle](../../../algebraic-geometry.md#normal-bundle) itself, not merely after stabilization.

Geometrically, multiply the two classes by forming their external product in $M\times M$ and pulling it back along the diagonal $\Delta:M\to M\times M$. The transversality hypothesis is precisely what makes the inverse image of $L_1\times L_2$ under $\Delta$ the [submanifold](../../../differential-geometry.md#submanifold) $L$. The [normal bundle](../../../algebraic-geometry.md#normal-bundle) of this inverse image is the direct sum just calculated. Multiplication of the corresponding [Thom classes](../../../fiber-bundle.md#thom-class) agrees with the [Thom class](../../../fiber-bundle.md#thom-class) of this direct sum, so the [complex cobordism product represented by transverse intersections](../../../geometry-and-topology.md#complex-cobordism-product-represented-by-transverse-intersections) is

$$
\boxed{[L_1,i_1,\nu_1]*[L_2,i_2,\nu_2]
=[L_1\cap L_2,\ j,\ \nu_1|_L\oplus\nu_2|_L].}
$$

If the inputs have complex normal ranks $a,b$, the product has degree $2(a+b)$. If they are disjoint, the representative is empty and the product is zero.

## 2

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Regard $\operatorname{Mat}_n(\mathbb C)$ as a real vector space of dimension $2n^2$, and let $\operatorname{Herm}_n(\mathbb C)$ be the real vector space of Hermitian matrices, of dimension $n^2$. The smooth Gram map

$$
F(A)=A^*A
$$

has $F^{-1}(I)=U(n)$ and differential $DF_A(K)=A^*K+K^*A$. At a unitary $A$, any Hermitian matrix $H$ is obtained by taking $K=AH/2$. Indeed $A^*K=H/2$ and $K^*A=H/2$. Hence $I$ is a [regular value](../../../differential-geometry.md#regular-value), and the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) proves the [unitary group as a regular level set](../../../topological-group.md#unitary-group-as-a-regular-level-set) result:

$$
\boxed{U(n)\text{ is a smooth manifold of real dimension }n^2.}
$$

Similarly let $G(A)=A^TA$ from $\operatorname{Mat}_n(\mathbb R)$ to the symmetric real matrices, whose dimension is $n(n+1)/2$. At an orthogonal $A$ its differential is $DG_A(K)=A^TK+K^TA$, again onto by choosing $K=AH/2$ for a symmetric $H$. Therefore the [orthogonal group as a regular level set](../../../linear-algebra.md#orthogonal-group-as-a-regular-level-set) has

$$
\boxed{\dim_{\mathbb R}O(n)=n^2-\frac{n(n+1)}2=\frac{n(n-1)}2.}
$$

Matrix multiplication is smooth on both groups, and inversion is conjugate transpose or transpose, respectively, so these manifold structures also make them [Lie groups](../../../lie-theory.md#lie-group). Both groups are closed and bounded in their finite-dimensional ambient matrix spaces, hence compact.

Realification identifies a unitary complex matrix with an orthogonal transformation of $\mathbb R^{2n}$. This is a smooth injective group homomorphism, with closed image, so $U(n)$ is the stated Lie subgroup of $O(2n)$. The assumed maximal-rank quotient map has fibers diffeomorphic to $U(n)$. Consequently the compact [homogeneous space](../../../lie-theory.md#homogeneous-space), also known as the [space of orthogonal complex structures](../../../complex-geometry.md#space-of-orthogonal-complex-structures), has dimension

$$
d=\dim O(2n)-\dim U(n)=n(2n-1)-n^2=n(n-1).
$$

The original PDF's sphere is $S^{n^2}$, with a square on the exponent; its dimension exceeds $d$ by $n$.

For completeness, [maps to a sphere above the dimension of a compact smooth manifold are null-homotopic](../../../algebraic-topology.md#maps-to-a-sphere-above-the-dimension-of-a-compact-smooth-manifold-are-null-homotopic). Let $X$ be a compact [smooth manifold](../../../differential-geometry.md#smooth-manifold) of dimension $d<q$, with $q\geq1$, and let $f:X\to S^q\subset\mathbb R^{q+1}$ be continuous. Choose a finite open cover on which $f$ is uniformly close to its value at a chosen point of that open set, and take a smooth [partition of unity](../../../differential-geometry.md#partition-of-unity) subordinate to the cover. The weighted sum of those chosen sphere values is a smooth map $g_0:X\to\mathbb R^{q+1}$ uniformly within $\epsilon<1$ of $f$. It never vanishes. Normalize it to $g=g_0/\|g_0\|$. Normalizing $(1-s)f+sg_0$ gives a [homotopy](../../../algebraic-topology.md#homotopy) from $f$ to $g$, since that vector remains within $\epsilon$ of the unit vector $f$.

Every value of $g$ is critical because its differential has rank at most $d<q$. The [Sard theorem](../../../differential-geometry.md#sard-s-theorem) makes its image have measure zero in $S^q$, so it misses some point $p$. The punctured sphere $S^q\setminus\{p\}$ is homeomorphic to $\mathbb R^q$ and contractible. Thus $g$, and hence $f$, is null-homotopic. This reasoning does not require $X$ to be connected, and all constant maps are homotopic because $S^q$ is path connected.

Apply it with $X=O(2n)/U(n)$ and $q=n^2$, for positive integer $n$. We obtain

$$
\boxed{[O(2n)/U(n),\,S^{n^2}]=\{[\text{constant map}]\}.}
$$

The notation means [homotopy](../../../algebraic-topology.md#homotopy) classes of maps; no [homotopy](../../../algebraic-topology.md#homotopy) equivalence between the two spaces is asserted.

## 3

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\xi$ have real rank $r$, choose a bundle metric, and write $D(\xi),S(\xi)$ for its disk and sphere bundles. In a [multiplicative generalized cohomology theory](../../../cohomology.md#multiplicative-generalized-cohomology-theory), a [Thom class in a generalized cohomology theory](../../../fiber-bundle.md#thom-class-in-a-generalized-cohomology-theory) is a class

$$
u_h(\xi)\in h^r(D(\xi),S(\xi))
$$

whose restriction to each fiber pair $(D^r,S^{r-1})$ is the suspension of the coefficient unit $1\in h^0(\mathrm{pt})$ under the chosen oriented identification. Equivalently, it is a fiberwise generator over the coefficient ring compatible with the $h$-orientation. [Cup product](../../../cohomology.md#cup-product) with this class gives the [Thom isomorphism theorem](../../../fiber-bundle.md#thom-isomorphism-theorem)

$$
h^k(X)\longrightarrow h^{k+r}(D(\xi),S(\xi)),\qquad
a\longmapsto\pi^*a\smile u_h(\xi),
$$

where $X$ is the base.

Let $z:X\to D(\xi)$ be the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle) and let $\jmath:h^r(D(\xi),S(\xi))\to h^r(D(\xi))$ forget relative supports. The [Euler class in a generalized cohomology theory](../../../fiber-bundle.md#euler-class-in-a-generalized-cohomology-theory) is

$$
\boxed{e_h(\xi)=z^*\jmath(u_h(\xi))\in h^r(X).}
$$

Equivalently, identify relative cohomology with [reduced cohomology](../../../cohomology.md#reduced-cohomology) of the [Thom space](../../../fiber-bundle.md#thom-space) and pull its [Thom class](../../../fiber-bundle.md#thom-class) back along the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle) followed by the quotient map.

Suppose $s$ is a nowhere-zero section. Normalize it to $\widehat s(x)=s(x)/\|s(x)\|\in S(\xi)_x$. The maps

$$
H_t(x)=t\widehat s(x),\qquad 0\leq t\leq1,
$$

give a [homotopy](../../../algebraic-topology.md#homotopy) within $D(\xi)$ from $z$ to the sphere-valued section $\widehat s$. The image $\jmath(u_h(\xi))$ restricts to zero on $S(\xi)$, by the exact sequence of the pair. [Homotopy](../../../algebraic-topology.md#homotopy) invariance therefore yields

$$
z^*\jmath(u_h(\xi))
=\widehat s^{\,*}\jmath(u_h(\xi))=0.
$$

Thus [a nowhere-zero section annihilates generalized Euler classes](../../../fiber-bundle.md#a-nowhere-zero-section-annihilates-generalized-euler-classes):

$$
\boxed{e_h(\xi)=0.}
$$

The argument uses the actual nowhere-zero section and is valid for any chosen Thom orientation in the multiplicative theory.

## 4

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a complex bundle $E$, write $c_t(E)=\sum_{j\geq0}c_j^{MU}(E)t^j$, with $c_0(E)=1$ and $c_j(E)=0$ for $j>\operatorname{rank}_{\mathbb C}E$. The [Whitney sum formula for Chern classes](../../../algebraic-geometry.md#whitney-sum-formula-for-chern-classes) in [complex cobordism](../../../geometry-and-topology.md#complex-cobordism) is

$$
\boxed{c_t(\eta\oplus\xi)=c_t(\eta)c_t(\xi),\qquad
c_k(\eta\oplus\xi)=\sum_{a+b=k}c_a(\eta)c_b(\xi).}
$$

Products are in the complex-cobordism cohomology ring; these classes have even degrees $2j$. The [splitting principle for complex vector bundles](../../../algebraic-topology.md#splitting-principle-for-complex-vector-bundles) explains the formula: on a splitting space the [Chern classes](../../../algebraic-geometry.md#chern-class) are elementary symmetric functions of the first [Chern classes](../../../algebraic-geometry.md#chern-class) of the line summands, and joining the two lists multiplies their total Chern polynomials.

Use the line convention for the [projective bundle](../../../fiber-bundle.md#projective-bundle):

$$
\mathbb{CP}(\eta)=\{(x,\ell):x\in X,\ \ell\subset\eta_x\text{ is a complex line}\}.
$$

Its [relative tautological line bundle](../../../fiber-bundle.md#relative-tautological-line-bundle) is

$$
\eta(1)=\{((x,\ell),v):v\in\ell\}\longrightarrow\mathbb{CP}(\eta).
$$

It is a complex rank-one subbundle of $p^*\eta$. Choose a [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) and let $E=\eta(1)^\perp$, of rank $n-1$, so $p^*\eta=\eta(1)\oplus E$.

Throughout, $x=c_1^{MU}(\eta(1))$, the tautological line's class, as specified before the final equation. Put $a_k=p^*c_k^{MU}(\eta)$ and $b_k=c_k^{MU}(E)$, with $a_0=b_0=1$. Since $c_t(\eta(1))=1+xt$, Whitney multiplication gives

$$
\sum_{k=0}^{n}a_kt^k=(1+xt)\sum_{k=0}^{n-1}b_kt^k.
$$

Comparison of coefficients gives $a_k=b_k+xb_{k-1}$, hence recursively $b_k=a_k-xb_{k-1}$. Therefore the [Chern classes of a tautological-line complement](../../../fiber-bundle.md#chern-classes-of-a-tautological-line-complement) are

$$
\boxed{c_k^{MU}(\eta(1)^\perp)
=\sum_{j=0}^{k}(-1)^j x^j\,p^*c_{k-j}^{MU}(\eta)
\quad(0\leq k\leq n-1),}
$$

and the classes for $k\geq n$ vanish by the rank.

At degree $n$ the same recursion has $b_n=0$, giving

$$
0=a_n-xa_{n-1}+x^2a_{n-2}-\cdots+(-1)^nx^n.
$$

Multiplying by $(-1)^n$ proves the [projective bundle relation in complex cobordism](../../../algebraic-geometry.md#projective-bundle-relation-in-complex-cobordism)

$$
\boxed{x^n-p^*c_1^{MU}(\eta)x^{n-1}
+p^*c_2^{MU}(\eta)x^{n-2}-\cdots+(-1)^np^*c_n^{MU}(\eta)=0.}
$$

These alternating signs come from the inverse formal power series $(1+xt)^{-1}$. They do not require identifying the [First Chern class](../../../complex-geometry.md#first-chern-class) of a dual line with $-x$, which is generally incorrect in [complex cobordism](../../../geometry-and-topology.md#complex-cobordism).

The final sentence's designation $x=c_1(\eta)$ must mean the earlier $c_1(\eta(1))$. If instead one substitutes $p^*c_1(\eta)$ literally, the claimed relation is false even in ordinary cohomology. For example, take $\eta=L\oplus L$ over $\mathbb{CP}^2$, with $a=c_1(L)$ a generator. Its [projective bundle](../../../fiber-bundle.md#projective-bundle) is $\mathbb{CP}^2\times\mathbb{CP}^1$, and $p^*a^2\ne0$. With the incorrect substitution $x=2p^*a$, the rank-two polynomial evaluates to

$$
(2p^*a)^2-(2p^*a)(2p^*a)+p^*a^2=p^*a^2\ne0.
$$

The tautological-line interpretation above is the one consistent with the bundle decomposition and the stated relation.

## 5

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a real or [complex vector bundle](../../../fiber-bundle.md#complex-vector-bundle) $E$, choose a fiber metric. Its [Thom space](../../../fiber-bundle.md#thom-space) is the pointed quotient

$$
\operatorname{Th}(E)=D(E)/S(E),
$$

collapsing the [sphere bundle](../../../fiber-bundle.md#sphere-bundle) to one basepoint. When the base is compact, this is the [one-point compactification](../../../topology.md#alexandroff-extension) of the total space: fiberwise radial compression identifies the total space with the interior of $D(E)$, and all directions approaching its boundary become the single point at infinity.

Decompose $\mathbb C^{n+m+2}=V\oplus W$ with $V=\mathbb C^{n+1}$, $W=\mathbb C^{m+1}$, so the subspace being collapsed is $\mathbb P(V)=\mathbb{CP}^n$. Every line outside it has a representative $(v,w)$ with $w\ne0$. Its projection to $W$ gives the line $\ell=\mathbb Cw\in\mathbb P(W)=\mathbb{CP}^m$, and there is a unique complex-linear map $A:\ell\to V$ such that $A(w)=v$. The line in $V\oplus W$ is precisely the graph of $A$. This construction is unaffected by replacing $(v,w)$ with $(\lambda v,\lambda w)$.

Let $\gamma=\eta_1$ be the tautological line over $\mathbb P(W)$. The graph construction and its inverse are continuous, indeed smooth in the usual affine charts, and identify

$$
\mathbb{CP}^{n+m+1}\setminus\mathbb{CP}^{n}
\cong\operatorname{Tot}\bigl(\operatorname{Hom}_{\mathbb C}(\gamma,V)\bigr)
=\operatorname{Tot}\bigl((\gamma^*)^{\oplus(n+1)}\bigr).
$$

A [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) gives a complex-linear bundle isomorphism $\bar\gamma\cong\gamma^*$. With the Hermitian form linear in its first argument, it sends $\bar v$ to the functional $w\mapsto\langle w,v\rangle$. Linearity in the conjugate vector is exactly what makes this a complex, rather than merely real, isomorphism. Thus the bundle is $(\bar\eta_1)^{\oplus(n+1)}$, with the conjugation bars present in the original PDF.

Collapsing the closed subspace $\mathbb{CP}^n$ in [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) $\mathbb{CP}^{n+m+1}$ gives the [one-point compactification](../../../topology.md#alexandroff-extension) of its open complement: neighborhoods of the collapsed point have compact complements, and conversely every compact subset of the complement is closed in the ambient space. The graph [homeomorphism](../../../topology.md#homeomorphism) therefore extends over the added point. This proves the [projective-space quotient as a Thom space of conjugate tautological lines](../../../fiber-bundle.md#projective-space-quotient-as-a-thom-space-of-conjugate-tautological-lines):

$$
\boxed{\mathbb{CP}^{n+m+1}/\mathbb{CP}^{n}
\cong\operatorname{Th}\bigl((\bar\eta_1)^{\oplus(n+1)}
\longrightarrow\mathbb{CP}^{m}\bigr).}
$$

The graph coordinates also determine the normal [complex structures](../../../complex-geometry.md#complex-structure) requested in the second part. The copy $\mathbb P(W)$ corresponds to the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle) of the graph bundle, whose [normal bundle](../../../algebraic-geometry.md#normal-bundle) is that bundle itself. For a coordinate embedding $\mathbb{CP}^k\subset\mathbb{CP}^n$, use $W=\mathbb C^{k+1}$ and its complementary coordinate space $V=\mathbb C^{n-k}$. Then the [normal bundle of a linear complex-projective embedding](../../../algebraic-geometry.md#normal-bundle-of-a-linear-complex-projective-embedding) is

$$
\boxed{\nu_k=\operatorname{Hom}_{\mathbb C}(\gamma_k,\mathbb C^{n-k})
\cong(\gamma_k^*)^{\oplus(n-k)}
\cong\bar\gamma_k^{\oplus(n-k)}.}
$$

The [complex structure](../../../complex-geometry.md#complex-structure) is the linear structure in these graph coordinates. Equivalently, applying the preceding [homeomorphism](../../../topology.md#homeomorphism) with its parameters $n-k-1$ and $k$ identifies the [Thom space](../../../fiber-bundle.md#thom-space) of this [normal bundle](../../../algebraic-geometry.md#normal-bundle) with $\mathbb{CP}^n/\mathbb{CP}^{n-k-1}$, after reordering coordinates. Define $\nu_m$ in the identical way. The Hermitian-metric identification with the conjugate line does not change the complex normal orientation.

The original coordinate embeddings may be nested, so first move one into transverse position. Keep $\mathbb{CP}^k=\mathbb P(A)$ for the first $k+1$ coordinates, and move $\mathbb{CP}^m$ to $\mathbb P(B)$ for the last $m+1$ coordinates. A unitary coordinate permutation accomplishes this. Every unitary matrix can be joined to the identity by diagonalizing it and varying its eigenvalue phases continuously, so this move is an [ambient isotopy](../../../differential-geometry.md#ambient-isotopy). Its trace gives a cobordism carrying the transported normal [complex structure](../../../complex-geometry.md#complex-structure), and hence leaves the input cobordism class unchanged.

If $k+m\geq n$, then

$$
A+B=\mathbb C^{n+1},\qquad
\dim_{\mathbb C}(A\cap B)=k+m-n+1.
$$

Their projectivizations are transverse and meet in $\mathbb{CP}^{r}$, where $r=k+m-n$. The direct-sum normal structure from question 1 restricts to

$$
\nu_k|_{\mathbb{CP}^{r}}\oplus\nu_m|_{\mathbb{CP}^{r}}
\cong\bar\gamma_r^{\oplus((n-k)+(n-m))}
=\bar\gamma_r^{\oplus(n-r)}
\cong\nu_r.
$$

The quotient map defining the transverse normal-bundle isomorphism is complex-linear here, so it agrees with the standard normal [complex structure](../../../complex-geometry.md#complex-structure) and contributes no orientation sign. If $k+m<n$, the first and last coordinate subspaces have no nonzero vector in common, so their projectivizations are disjoint.

Consequently the [product of linear projective subspaces in complex cobordism](../../../geometry-and-topology.md#product-of-linear-projective-subspaces-in-complex-cobordism) is

$$
\boxed{
[\mathbb{CP}^{k},\nu_k]*[\mathbb{CP}^{m},\nu_m]
=\begin{cases}
[\mathbb{CP}^{k+m-n},\nu_{k+m-n}],&k+m\geq n,\\
0,&k+m<n.
\end{cases}}
$$

The product degree is $2(2n-k-m)$, equal to the real codimension of the stated intersection when it exists. In the equality case $k+m=n$, the representative is one point with its complex-oriented normal space.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
