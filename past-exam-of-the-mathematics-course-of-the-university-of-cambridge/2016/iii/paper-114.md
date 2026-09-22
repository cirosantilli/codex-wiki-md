# Paper 114

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_114.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_114.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

First account for the unlabelled coefficient-sequence construction. The two [short exact sequences](../../../module-theory.md#short-exact-sequence) of [abelian groups](../../../group.md#abelian-group) are

$$
0\longrightarrow\mathbb Z\xrightarrow{\,n\,}\mathbb Z\xrightarrow{\widehat\alpha}\mathbb Z/n\longrightarrow0,
\qquad
0\longrightarrow\mathbb Z/n\xrightarrow{\,j\,}\mathbb Z/n^2\xrightarrow{\alpha}\mathbb Z/n\longrightarrow0,
\quad j([a])=[na].
$$

The [singular chain groups](../../../homology.md#singular-chain-group) of $X$ are free abelian. Applying $\operatorname{Hom}(C_q(X),-)$ therefore preserves these exact sequences, degree by degree, giving [short exact sequences of cochain complexes](../../../algebra.md#short-exact-sequence-of-cochain-complexes). The associated [long exact sequence from a coefficient sequence](../../../homology.md#long-exact-sequence-from-a-coefficient-sequence) gives the displayed maps in [cohomology](../../../cohomology.md); the connecting maps are the [integral Bockstein homomorphism](../../../homology.md#integral-bockstein-homomorphism) $\widehat\beta$ and the modulo-$n$ [Bockstein homomorphism](../../../homology.md#bockstein-homomorphism) $\beta$. The first omitted map is multiplication by $n$, and the second is induced by $j$.

For the requested example, attach an $(i+1)$-cell to $S^i$ using a map of degree $n$. The resulting [Moore space](../../../algebraic-topology.md#moore-space-algebraic-topology) $X=M(\mathbb Z/n,i)$ has positive-degree [cellular chain complex](../../../homology.md#cellular-chain-complex)

$$
0\longrightarrow\mathbb Z\xrightarrow{\,n\,}\mathbb Z\longrightarrow0
$$

in degrees $i+1,i$. This construction also works for $i=1$, using the degree-$n$ map of the circle. In [cellular cohomology](../../../homology.md#cellular-cohomology) with coefficients $\mathbb Z/n$, the differential is zero, so both $H^i$ and $H^{i+1}$ are $\mathbb Z/n$.

Lift the cochain taking value $1$ on the $i$-cell to a cochain with coefficients $\mathbb Z/n^2$. Its coboundary takes value $n$ on the $(i+1)$-cell, which is $j(1)$. The definition of the [connecting homomorphism](../../../homology.md#connecting-homomorphism) therefore sends the degree-$i$ generator to the degree-$(i+1)$ generator. Hence

$$
\boxed{\beta:H^i(M(\mathbb Z/n,i);\mathbb Z/n)\xrightarrow{\ \cong\ }H^{i+1}(M(\mathbb Z/n,i);\mathbb Z/n).}
$$

It is nonzero for every $i\geq1$ and $n\geq2$, including composite $n$. This is the [Bockstein on a cyclic Moore space](../../../algebraic-topology.md#bockstein-on-a-cyclic-moore-space).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $\rho:H^*(X;\mathbb Z)\to H^*(X;\mathbb Z/n)$ for coefficient reduction. Compare the two coefficient sequences in part (a): the maps from the integral sequence to the finite sequence are reduction modulo $n$ on the left, reduction modulo $n^2$ in the middle, and the identity on the right. The square involving the injections commutes because $[na]_{n^2}=j([a]_n)$.

Naturality of the [connecting homomorphism](../../../homology.md#connecting-homomorphism) gives the [Bockstein factorization through integral cohomology](../../../homology.md#bockstein-factorization-through-integral-cohomology)

$$
\boxed{\beta=\rho\widehat\beta.}
$$

One can see this directly without a diagram: lift a modulo-$n$ cocycle to an integral cochain $a$. Its coboundary has the form $\delta a=nb$. Then $\widehat\beta[a]=[b]$, whereas $\beta[a]=[b\bmod n]$.

Exactness of the integral coefficient sequence gives $\widehat\beta\rho=0$: a class obtained by reducing an integral cocycle has zero integral connecting class. Consequently

$$
\boxed{\beta^2=\rho\widehat\beta\rho\widehat\beta=0.}
$$

This [Bockstein square-zero identity](../../../homology.md#bockstein-square-zero-identity) holds without requiring $n$ to be prime. At the cochain level, $\delta^2a=0$ and the torsion-free integral cochain groups imply $\delta b=0$, which also makes the second connecting class vanish.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The standard [CW complex](../../../algebraic-topology.md#cw-complex) structure on [Real projective space](../../../algebraic-topology.md#real-projective-space) has one cell in each dimension from zero to three. Its integral cellular boundary is multiplication by $2$ in even positive degrees and zero in odd degrees. Thus the integral [cellular cochain complex](../../../homology.md#cellular-cochain-complex) for $\mathbb{RP}^3$ is

$$
\mathbb Z\xrightarrow{\,0\,}\mathbb Z\xrightarrow{\,2\,}\mathbb Z\xrightarrow{\,0\,}\mathbb Z
$$

in degrees $0,1,2,3$. With coefficients $\mathbb F_2$, all its differentials vanish, so every one of these four [cohomology groups](../../../cohomology.md#cohomology-group) is one-dimensional.

The lift-and-divide construction of the [Bockstein homomorphism](../../../homology.md#bockstein-homomorphism) turns the integral differential $2$ into $1$ modulo $2$. Therefore $\beta:H^1\to H^2$ is an isomorphism, while the maps from degrees $0,2,3$ are zero. The [Bockstein cohomology](../../../homology.md#bockstein-cohomology) is consequently

$$
\boxed{H\beta^q(\mathbb{RP}^3;2)=\begin{cases}\mathbb F_2,&q=0,3,\\0,&\text{otherwise}.\end{cases}}
$$

For comparison, in the [mod-two cohomology ring of real projective space](../../../algebraic-topology.md#mod-two-cohomology-ring-of-real-projective-space) $\mathbb F_2[t]/(t^4)$, $|t|=1$, this says $\beta(t)=t^2$, $\beta(t^2)=0$ and $\beta(t^3)=0$. The last two formulas also follow from the [Bockstein derivation rule](../../../homology.md#bockstein-derivation-rule) and the truncation $t^4=0$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For any finite-dimensional bounded [cochain complex](../../../algebra.md#cochain-complex) $(V^*,d)$ over a [field](../../../algebra.md#field), let $r_q=\operatorname{rank}(d:V^q\to V^{q+1})$, with zero ranks outside its degree range. Then

$$
\dim H^q(V,d)=\dim V^q-r_q-r_{q-1}.
$$

Taking the alternating sum cancels the two rank sums. Thus taking [cohomology](../../../cohomology.md) preserves the [Euler characteristic](../../../homology.md#euler-characteristic) of a finite graded complex. Apply this to $V^q=H^q(M;\mathbb F_p)$ and $d=\beta$, using part (b).

A closed three-dimensional [manifold](../../../topology.md#topological-manifold) has finite-dimensional [cohomology](../../../cohomology.md), vanishing above degree three. Its [Euler characteristic](../../../homology.md#euler-characteristic) is zero, even when it is not orientable: [Poincare duality](../../../cohomology.md#poincare-duality) with $\mathbb F_2$ coefficients gives $b_q=b_{3-q}$, so the alternating sum vanishes. A finite triangulation, or finite [CW complex](../../../algebraic-topology.md#cw-complex) model, shows that the alternating sum is the same integer with coefficients in any field, since it equals the alternating count of cells. Therefore

$$
\boxed{\chi\bigl(H\beta^*(M;p)\bigr)=\chi(M)=0.}
$$

The primeness assumption makes $\mathbb Z/p$ a field; no orientation assumption on $M$ is needed.

## 2

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Give the [closed orientable surface](../../../topology.md#closed-orientable-surface) its standard [CW complex](../../../algebraic-topology.md#cw-complex) structure: one zero-cell, $2g$ one-cells, and one two-cell attached by the product of $g$ commutators. The cellular boundary of the two-cell is zero, since every edge occurs once with each orientation in that word; the one-cell boundaries are also zero. Hence

$$
H^q(\Sigma_g;\mathbb Z)\cong\begin{cases}\mathbb Z,&q=0,2,\\\mathbb Z^{2g},&q=1,\\0,&\text{otherwise}.\end{cases}
$$

Here we use the [cellular homology theorem](../../../homology.md#cellular-homology-theorem), identifying cellular and singular homology, and the [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology): its exact sequence has terms $\operatorname{Ext}(H_{q-1},\mathbb Z)$ and $\operatorname{Hom}(H_q,\mathbb Z)$. All the homology groups here are free, so the Ext terms vanish.

The ring structure comes from [Poincare duality](../../../cohomology.md#poincare-duality) and [algebraic intersection number of curves on an oriented surface](../../../topology.md#algebraic-intersection-number-of-curves-on-an-oriented-surface). For a closed oriented surface, cap product with its [fundamental class](../../../cohomology.md#fundamental-class) identifies degree-one [cohomology](../../../cohomology.md) with degree-one homology; evaluating the [cup product](../../../cohomology.md#cup-product) of two such classes equals the signed intersection number of their dual one-cycles. Choose the usual $g$ pairs of handle curves, each pair meeting positively once, and distinct pairs disjoint. Their dual classes can accordingly be named $a_1,b_1,\ldots,a_g,b_g$ so that, for the positive orientation class $\omega$,

$$
\boxed{a_i\smile b_j=\delta_{ij}\omega,\qquad b_j\smile a_i=-\delta_{ij}\omega,\qquad a_i\smile a_j=b_i\smile b_j=0.}
$$

These formulas include squares. More generally, [graded commutativity of the cup product](../../../cohomology.md#graded-commutativity-of-the-cup-product) kills every degree-one square here because $H^2$ is torsion-free. The unit generates $H^0$, and products involving $\omega$ and any positive-degree class vanish for dimensional reasons. These additive groups and multiplication rules completely describe the [cohomology ring of a closed oriented surface](../../../cohomology.md#cohomology-ring-of-a-closed-oriented-surface), including $g=0$, when there are no degree-one generators. The intersection pairing is integral and unimodular, rather than merely nondegenerate over a field.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Suppose $F:\Sigma_g\to\Sigma_h$ has degree one. For degree-one classes $u,v$ on the target, naturality of the [cup product](../../../cohomology.md#cup-product) and the definition of the [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds) give

$$
\left\langle F^*u\smile F^*v,[\Sigma_g]\right\rangle=\left\langle u\smile v,F_*[\Sigma_g]\right\rangle=\left\langle u\smile v,[\Sigma_h]\right\rangle.
$$

If a nonzero $u$ had $F^*u=0$, nondegeneracy of the [Poincare duality pairing](../../../cohomology.md#poincare-duality-pairing) would supply $v$ with nonzero right side, a contradiction. Thus $F^*$ injects the $2h$-dimensional real degree-one [cohomology](../../../cohomology.md) into the $2g$-dimensional source. Hence $g\geq h$. This is the [cohomological injectivity of a degree-one map](../../../cohomology.md#cohomological-injectivity-of-a-degree-one-map) in this setting.

Conversely, for $g\geq h$, express $\Sigma_g$ as $\Sigma_h\#\Sigma_{g-h}$. Collapse the second punctured summand and the joining circle to a point. The quotient of the retained punctured summand by its boundary is homeomorphic to $\Sigma_h$, giving a continuous map to that surface. Its restriction to a small oriented disc away from the collapsing region is an orientation-preserving homeomorphism, and a point in this disc has exactly one preimage. The induced map on local top homology, and hence on the [fundamental class](../../../cohomology.md#fundamental-class), has coefficient $+1$. The map therefore has degree one. For $h=0$, the same construction is the familiar collapse of the complement of a disc to obtain $S^2$.

Consequently

$$
\boxed{\text{A degree-one map }\Sigma_g\longrightarrow\Sigma_h\text{ exists exactly when }g\geq h.}
$$

This proves both directions of the [degree-one maps between closed oriented surfaces](../../../homology.md#degree-one-maps-between-closed-oriented-surfaces) criterion. The case $g=h$ also admits the identity map.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $A=\Sigma_h^\partial$. This [surface with boundary](../../../topology.md#surface-with-boundary) deformation retracts onto a wedge of $2h$ circles, so $H^1(A;\mathbb R)$ has dimension $2h$ and $H^2(A;\mathbb R)=0$. If $r$ were a [retraction](../../../topology.md#retraction), $\iota^*r^*=\mathrm{id}$ would make $r^*$ injective. Its image $W\subset H^1(\Sigma_g;\mathbb R)$ would have dimension $2h$.

Every pair of classes $u,v$ in $H^1(A;\mathbb R)$ has $u\smile v=0$, since $H^2(A;\mathbb R)=0$. Naturality gives

$$
r^*u\smile r^*v=r^*(u\smile v)=0.
$$

Thus $W$ is an [isotropic subspace of a symplectic vector space](../../../linear-algebra.md#isotropic-subspace-of-a-symplectic-vector-space) for the nondegenerate skew [Poincare duality pairing](../../../cohomology.md#poincare-duality-pairing) on the $2g$-dimensional space $H^1(\Sigma_g;\mathbb R)$. The stated linear-algebra bound gives $2h\leq g$. Hence

$$
\boxed{h>g/2\quad\Longrightarrow\quad\text{no retraction exists}.}
$$

**The bound is sharp.** Double $A$ along its boundary: $D(A)=A\cup_{\partial A}A$ is the closed oriented surface of genus $2h$. Identify each copy with $A$ and fold them onto one copy. The two maps agree on the joining circle, so they give a continuous [retraction](../../../topology.md#retraction) fixing the first copy pointwise. This includes $h=0$, where the double of a disc is a sphere.

More generally, for $g\geq2h$, add $g-2h$ handles in the interior of the second copy. Pinch those extra handles onto their connecting point, keeping the boundary fixed, and then fold onto $A$. This is still a [retraction](../../../topology.md#retraction). In fact the construction works for any embedding in the question: the connected complement has one boundary component and genus $g-h$ by Euler-characteristic additivity, and the [classification theorem for surfaces](../../../geometry-and-topology.md#classification-theorem-for-surfaces) identifies it, relative to that boundary, with a copy of $A$ having $g-2h$ additional handles. Thus the exact existence criterion is $2h\leq g$, as expressed by [retraction onto a punctured oriented surface](../../../topology.md#retraction-onto-a-punctured-oriented-surface).

## 3

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

**The assertion is true.** The standard filtration $\mathbb{CP}^0\subset\cdots\subset\mathbb{CP}^n$ gives one cell in each dimension $0,2,\ldots,2n$. There are no odd-dimensional cells, so all cellular differentials vanish. The [cellular homology theorem](../../../homology.md#cellular-homology-theorem) and the [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology) give one copy of $\mathbb Z$ in each even degree from zero to $2n$, and zero in every other degree.

Let $x$ be the [Poincare dual](../../../cohomology.md#poincare-dual) of a [projective hyperplane](../../../algebraic-topology.md#projective-hyperplane), with the complex orientation. It has degree two and evaluates to $+1$ on a [complex projective line](../../../algebraic-topology.md#complex-projective-line), so it is the positive generator of $H^2$. We use the intersection interpretation of the [cup product](../../../cohomology.md#cup-product): the product of duals of oriented submanifolds in transverse position is the dual of their oriented intersection. Distinct transverse complex hyperplanes intersect in $\mathbb{CP}^{n-j}$ after $j$ intersections, with positive complex orientation. Thus $x^j$ is the dual of that linear subspace.

Pairing $x^j$ with a transverse linear $\mathbb{CP}^j$ gives one positively oriented intersection point. Therefore $x^j$ is a primitive generator of $H^{2j}$, for every $0\leq j\leq n$. There is no [cohomology](../../../cohomology.md) above dimension $2n$, so $x^{n+1}=0$. These facts show that the surjective graded ring map from $\mathbb Z[x]$ has exactly the indicated kernel:

$$
\boxed{H^*(\mathbb{CP}^n;\mathbb Z)\cong\mathbb Z[x]/(x^{n+1}),\qquad |x|=2.}
$$

This proves the [cohomology ring of complex projective space](../../../algebraic-topology.md#cohomology-ring-of-complex-projective-space), rather than only its additive groups. For $n=0$ it is $\mathbb Z$, with $x=0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

**The assertion is false.** Take $m=3$ and $n=2$. For the constant attaching map, the [cell attachment](../../../algebraic-topology.md#cell-attachment) gives $S^2\vee S^4$. Its degree-two generator has square zero: restricting the square to either sphere gives zero, and restrictions identify its degree-four [cohomology](../../../cohomology.md) with that of the $S^4$ summand.

For the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration) $\eta:S^3\to S^2=\mathbb{CP}^1$, the attachment instead gives $\mathbb{CP}^2$. One can verify the attaching map explicitly with the characteristic map

$$
D^4\longrightarrow\mathbb{CP}^2,\qquad (z_1,z_2)\longmapsto[z_1:z_2:\sqrt{1-|z_1|^2-|z_2|^2}].
$$

Its interior maps homeomorphically to the complement of $\mathbb{CP}^1$; on the boundary it sends $(z_1,z_2)$ to $[z_1:z_2:0]$, exactly the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration). By part (a), the degree-two generator of $H^*(\mathbb{CP}^2;\mathbb Z)$ has nonzero square generating degree four. Hence

$$
\boxed{H^*(X_{\mathrm{constant}};\mathbb Z)\not\cong H^*(X_\eta;\mathbb Z)\text{ as graded rings}.}
$$

The additive groups agree, but multiplication distinguishes the attachments.

The dimension condition explains why this example is the relevant one. In general the only positive-degree additive generators lie in degrees $n$ and $m+1$. A potentially nonzero product can only be the square of the degree-$n$ generator, and only when $m+1=2n$. Its coefficient is the [Hopf invariant](../../../algebraic-topology.md#hopf-invariant) of the attaching map. Here the constant map has invariant zero, whereas the complex [Hopf fibration](../../../algebraic-topology.md#hopf-fibration) has invariant one.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For nonzero finite-dimensional $U$ and $V$, **the intended assertion is true**. Write $a=\dim U$, $b=\dim V$, and replace $W$ by $\operatorname{im}\phi$, of dimension $r$. Injectivity on the stated slices implies $\phi(u\otimes v)\ne0$ whenever $u,v\ne0$. Consequently the [bilinear map](../../../linear-algebra.md#bilinear-map) defines a continuous map of [Complex projective spaces](../../../algebraic-topology.md#complex-projective-space)

$$
F:\mathbb P(U)\times\mathbb P(V)\longrightarrow\mathbb P(\operatorname{im}\phi),\qquad ([u],[v])\longmapsto[\phi(u\otimes v)].
$$

The rank $r$ is at least one, since one such nonzero tensor has nonzero image.

Let $L_U,L_V,L_W$ be the respective [tautological bundles](../../../fiber-bundle.md#tautological-bundle). Fiberwise, $\phi$ identifies $L_U\otimes L_V$ with $F^*L_W$. For the positive hyperplane classes $x=c_1(L_U^*)$, $y=c_1(L_V^*)$ and $z=c_1(L_W^*)$ (zero when the projective space is a point), the [first Chern class of a tensor product of complex line bundles](../../../complex-geometry.md#first-chern-class-of-a-tensor-product-of-complex-line-bundles) gives

$$
F^*z=x+y.
$$

The [Künneth theorem](../../../cohomology.md#kunneth-theorem), together with part (a), identifies the product [cohomology ring](../../../cohomology.md#cohomology-ring) with

$$
H^*(\mathbb P(U)\times\mathbb P(V);\mathbb Z)=\mathbb Z[x,y]/(x^a,y^b).
$$

There are no Tor terms because the factor groups are free. In particular, its monomials $x^iy^j$ with $0\leq i<a$, $0\leq j<b$ form an integral additive basis. In top degree,

$$
(x+y)^{a+b-2}=\binom{a+b-2}{a-1}x^{a-1}y^{b-1}\ne0.
$$

If $r\leq a+b-2$, the target relation $z^r=0$ would imply $(x+y)^r=0$ and hence contradict this nonzero top power. Thus

$$
\boxed{\dim_{\mathbb C}\operatorname{im}\phi\geq\dim_{\mathbb C}U+\dim_{\mathbb C}V-1.}
$$

When $a=b=1$, the already-established inequality $r\geq1$ gives the same conclusion. The [complex bilinear dimension bound](../../../linear-algebra.md#complex-bilinear-dimension-bound) is sharp: multiplication of complex polynomials of degrees less than $a$ and $b$ has target dimension $a+b-1$, is injective in either nonzero fixed factor, and its image spans every monomial in that target.

**Literal zero-space qualification.** The printed assertion does not explicitly exclude zero vector spaces. If $U=0$, $V=\mathbb C^2$ and $W=0$, its slice-injectivity hypothesis is vacuous, while the claimed inequality would be $0\geq1$. Thus, with zero spaces permitted, this is a counterexample to the assertion exactly as written; the proof above supplies the usual nonzero finite-dimensional interpretation.

## 4

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $m=\dim M$ and $q=m-\dim Y$. Here a closed submanifold means compact and without boundary, which is the condition needed for a compactly supported dual class. The orientations of $M$ and $Y$ orient the [normal bundle](../../../algebraic-geometry.md#normal-bundle) $\nu_Y$. Its [Thom class](../../../fiber-bundle.md#thom-class) is the unique relative class of degree $q$ restricting to the chosen orientation generator on every normal fiber. A [tubular neighborhood](../../../differential-geometry.md#tubular-neighborhood) identifies this class with one near $Y$ in $M$. Choose a compact normal disc neighborhood and extend the relative class to [compactly supported cohomology](../../../cohomology.md#compactly-supported-cohomology) of $M$. Equivalently, apply [Poincare duality](../../../cohomology.md#poincare-duality) $H_c^q(M;\mathbb Q)\cong H_{m-q}(M;\mathbb Q)$ to the pushed-forward [fundamental class](../../../cohomology.md#fundamental-class) of $Y$:

$$
\boxed{\varepsilon_Y=\operatorname{PD}_M(i_*[Y])\in H_c^q(M;\mathbb Q).}
$$

This [compactly supported dual of a compact submanifold](../../../cohomology.md#compactly-supported-dual-of-a-compact-submanifold) is independent of the tubular neighborhood and represents intersection with $Y$. Fix the convention $\langle\varepsilon_Y\smile a,[M]\rangle=\langle i^*a,[Y]\rangle$ in complementary degree. Its image in ordinary [cohomology](../../../cohomology.md) restricts to zero on $M\setminus Y$, because it comes from relative [cohomology](../../../cohomology.md) supported near $Y$. If a submanifold is only closed as a subset but is noncompact, its usual dual lies in ordinary [cohomology](../../../cohomology.md) instead; compact support is not asserted in that situation.

Now let $\Delta\subset N\times N$ be the diagonal, with the orientation inherited from $N$, and let $\delta=\varepsilon_\Delta\in H^n(N\times N;\mathbb Q)$. For each $i$, choose a basis $a_{i,j}$ of $H^i(N;\mathbb Q)$ and its dual basis $b_{i,j}$ of $H^{n-i}(N;\mathbb Q)$ satisfying $\langle a_{i,j}\smile b_{i,k},[N]\rangle=\delta_{jk}$. The [Poincare duality pairing](../../../cohomology.md#poincare-duality-pairing) and the [Künneth theorem](../../../cohomology.md#kunneth-theorem) give the [cohomology class of the diagonal](../../../algebraic-topology.md#cohomology-class-of-the-diagonal)

$$
\delta=\sum_{i,j}(-1)^{i(n-i+1)}p_1^*b_{i,j}\smile p_2^*a_{i,j}.
$$

The sign can be checked from the defining identity

$$
\left\langle\delta\smile(p_1^*u\smile p_2^*v),[N\times N]\right\rangle=\langle u\smile v,[N]\rangle.
$$

For $|u|=i$, moving the degree-$i$ class in the second factor past $u$ contributes $(-1)^i$, and interchanging $b_{i,j}$ and $u$ contributes $(-1)^{i(n-i)}$; the displayed coefficient cancels their product. Equivalently its exponent is $ni$ modulo two.

The [cohomological pushforward between closed oriented manifolds](../../../cohomology.md#cohomological-pushforward-between-closed-oriented-manifolds) is characterized by

$$
\langle f^!c\smile b,[N]\rangle=\langle c\smile f^*b,[M]\rangle,
$$

for complementary degrees. This follows immediately from its definition by [Poincare duality](../../../cohomology.md#poincare-duality) and naturality of evaluation on pushed-forward homology. In degree $i$, the [matrix trace](../../../linear-algebra.md#matrix-trace) of $f^!g^*$ on $H^i(N;\mathbb Q)$ is consequently

$$
\operatorname{tr}(f^!g^*)=\sum_j\langle g^*a_{i,j}\smile f^*b_{i,j},[M]\rangle.
$$

For finite-dimensional maps between two possibly different vector spaces, $\operatorname{tr}(AB)=\operatorname{tr}(BA)$. Thus this [matrix trace](../../../linear-algebra.md#matrix-trace) equals that of $g^*f^!$ on $H^i(M;\mathbb Q)$. Pulling back the diagonal formula by $F=(f,g)$ and applying [graded commutativity of the cup product](../../../cohomology.md#graded-commutativity-of-the-cup-product) now yields

$$
\boxed{\left\langle(f,g)^*\delta,[M]\right\rangle=\sum_i(-1)^i\operatorname{tr}(g^*f^!)=L(f,g).}
$$

This establishes the [Lefschetz coincidence number](../../../algebraic-topology.md#lefschetz-coincidence-number) with the requested sign convention.

If $f(m)\ne g(m)$ for every $m$, the map $(f,g)$ factors through $(N\times N)\setminus\Delta$. The diagonal class restricts to zero there, so its pullback is zero and $L(f,g)=0$. Taking the contrapositive proves the [Lefschetz coincidence theorem](../../../algebraic-topology.md#lefschetz-coincidence-theorem):

$$
\boxed{L(f,g)\ne0\quad\Longrightarrow\quad f(m)=g(m)\text{ for some }m\in M.}
$$

No transversality or isolated-coincidence assumption is needed. This cohomological argument also applies to continuous maps, which covers the last request.

For a map $f:M\to N$ of degree $d$, the adjoint identity above gives, for all complementary classes $a,b$ on $N$,

$$
\langle f^!f^*a\smile b,[N]\rangle=\langle f^*(a\smile b),[M]\rangle=d\langle a\smile b,[N]\rangle.
$$

Nondegeneracy therefore gives $f^!f^*=d\,\mathrm{id}$. Cyclic invariance of [matrix trace](../../../linear-algebra.md#matrix-trace) proves the [self-coincidence number of a map of nonzero degree](../../../algebraic-topology.md#self-coincidence-number-of-a-map-of-nonzero-degree) formula

$$
L(f,f)=d\,\chi(N).
$$

In particular, $\mathbb{CP}^{2k}$ has one even-dimensional [cohomology](../../../cohomology.md) generator in each degree $0,2,\ldots,4k$, so $\chi(\mathbb{CP}^{2k})=2k+1$. Hence

$$
\boxed{L(f,f)=(2k+1)d\ne0.}
$$

If $g$ is homotopic to $f$, [homotopy invariance of cohomology](../../../cohomology.md#homotopy-invariance-of-cohomology) gives $g^*=f^*$ and thus $L(f,g)=L(f,f)$. The [Lefschetz coincidence theorem](../../../algebraic-topology.md#lefschetz-coincidence-theorem) supplies a point at which $f$ and $g$ agree.

## 5

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Here is an intrinsic definition that also proves well-definedness. For a [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) $L$, define its [First Chern class](../../../complex-geometry.md#first-chern-class) to be the [Euler class](../../../fiber-bundle.md#euler-class-of-a-vector-bundle) of its canonically oriented underlying real rank-two bundle: pull its integral [Thom class](../../../fiber-bundle.md#thom-class) back along the zero section after forgetting relative support. The complex orientation fixes the sign, so this construction makes no arbitrary choice of generator.

For a rank-$r>0$ [complex vector bundle](../../../fiber-bundle.md#complex-vector-bundle) $E$, let $\pi:\mathbb P(E)\to X$ be its [projective bundle](../../../fiber-bundle.md#projective-bundle) of lines, let $S\subset\pi^*E$ be the [tautological bundle](../../../fiber-bundle.md#tautological-bundle), and put $h=-c_1(S)=c_1(S^*)$. On every fiber $\mathbb{CP}^{r-1}$, $h$ is the positive degree-two generator. The [Leray-Hirsch theorem](../../../fiber-bundle.md#leray-hirsch-theorem) says that if globally defined [cohomology](../../../cohomology.md) classes restrict to a free basis of the [cohomology](../../../cohomology.md) of every fiber, then multiplication by those classes identifies the [cohomology](../../../cohomology.md) of the total space with a [free module](../../../module-theory.md#free-module) over the base. Applied here, it gives

$$
\bigoplus_{j=0}^{r-1}H^{*-2j}(X;\mathbb Z)\xrightarrow{\ \cong\ }H^*(\mathbb P(E);\mathbb Z),\qquad(a_j)_j\longmapsto\sum_j\pi^*a_j\smile h^j.
$$

The finite trivializing cover in the question is sufficient for this application: the assertion holds on each trivializing open set by the [Künneth theorem](../../../cohomology.md#kunneth-theorem), since the fiber has finite free [cohomology](../../../cohomology.md), and the [Mayer–Vietoris sequence](../../../algebraic-topology.md#mayer-vietoris-sequence) and the [Five lemma](../../../category-theory.md#five-lemma) glue it over the finite cover. The same local argument constructs the oriented [Thom class](../../../fiber-bundle.md#thom-class) used for line bundles. It does not require a choice of classifying map.

There are therefore unique classes $c_i(E)\in H^{2i}(X;\mathbb Z)$ such that

$$
\boxed{h^r+\pi^*c_1(E)h^{r-1}+\cdots+\pi^*c_r(E)=0.}
$$

Define $c_0(E)=1$ and $c_i(E)=0$ for $i>r$. For rank zero the [Total Chern class](../../../algebraic-geometry.md#total-chern-class) is $1$. This is the [projective bundle definition of Chern classes](../../../algebraic-geometry.md#projective-bundle-definition-of-chern-classes). Existence and uniqueness follow by expressing $h^r$ in the displayed [free module](../../../module-theory.md#free-module) basis, with degrees determining each coefficient. The [projective bundle](../../../fiber-bundle.md#projective-bundle) and [tautological bundle](../../../fiber-bundle.md#tautological-bundle) are intrinsic to $E$, and the line [Thom class](../../../fiber-bundle.md#thom-class) is uniquely fixed by orientation. Hence the resulting [Chern classes](../../../algebraic-geometry.md#chern-class) do not depend on trivializations or other auxiliary choices. For a line bundle the relation is $h+c_1(E)=0$, agreeing with the original normalization. Pulling back this unique relation also proves naturality. This standard construction and the sum theorem are treated in [Vector Bundles and K-Theory, Section 3.1](https://pi.math.cornell.edu/~hatcher/VBKT/VB.pdf).

The requested result is the [Whitney sum formula for Chern classes](../../../algebraic-geometry.md#whitney-sum-formula-for-chern-classes):

$$
\boxed{c(E\oplus E')=c(E)c(E'),\qquad c_k(E\oplus E')=\sum_{i+j=k}c_i(E)\smile c_j(E').}
$$

Here $c(E)=1+c_1(E)+\cdots+c_r(E)$, and the formula holds for complex vector bundles over a common base. In particular, a trivial bundle has total Chern class $1$.

Now take $B=\mathbb{CP}^{n-1}$ and let $L\subset B\times\mathbb C^n$ be its [tautological bundle](../../../fiber-bundle.md#tautological-bundle). The standard [Hermitian inner product](../../../linear-algebra.md#hermitian-form) gives the rank-$(n-1)$ complex bundle $Q=L^\perp$, with $L\oplus Q\cong\underline{\mathbb C}^{\,n}$. The [orthogonal complex line flag manifold](../../../fiber-bundle.md#orthogonal-complex-line-flag-manifold) in the question is precisely $\mathbb P(Q)$: over a first line $\ell$, the second line is any line in $\ell^\perp$. Local orthonormal frames give this identification as a [fiber bundle](../../../fiber-bundle.md), with fiber $\mathbb{CP}^{n-2}$.

Let $x=c_1(L^*)$ on $B$, also writing $x$ for its pullback to $\mathbb P(Q)$. By part 3(a), $H^*(B;\mathbb Z)=\mathbb Z[x]/(x^n)$. The [Whitney sum formula for Chern classes](../../../algebraic-geometry.md#whitney-sum-formula-for-chern-classes) gives

$$
(1-x)c(Q)=1,\qquad c(Q)=1+x+x^2+\cdots+x^{n-1},\qquad c_i(Q)=x^i.
$$

Let $S_2$ be the second tautological line on $\mathbb P(Q)$, and set $y=c_1(S_2^*)$. Thus $x,y$ are exactly the pullbacks of the positive hyperplane classes from the two projective factors. The [projective bundle definition of Chern classes](../../../algebraic-geometry.md#projective-bundle-definition-of-chern-classes) for $Q$ gives

$$
y^{n-1}+xy^{n-2}+x^2y^{n-3}+\cdots+x^{n-1}=0.
$$

Together with $x^n=0$, this gives a surjective graded ring map

$$
\mathbb Z[x,y]\big/(x^n,\,x^{n-1}+x^{n-2}y+\cdots+xy^{n-2}+y^{n-1})\longrightarrow H^*(X;\mathbb Z).
$$

There are **no additional relations**. Indeed the second relation is monic of degree $n-1$ in $y$, so [polynomial division](../../../polynomial.md#polynomial-division) makes its source free over $\mathbb Z[x]/(x^n)$ on $1,y,\ldots,y^{n-2}$. The [projective bundle formula for complex vector bundles](../../../fiber-bundle.md#projective-bundle-formula-for-complex-vector-bundles) gives exactly the same free basis on the target. The map sends each basis element to its corresponding basis element, and is therefore an isomorphism. Consequently

$$
\boxed{H^*(X;\mathbb Z)=\mathbb Z[x,y]/\left(x^n,\ \sum_{j=0}^{n-1}x^{n-1-j}y^j\right),\qquad |x|=|y|=2.}
$$

This is the [cohomology ring of the orthogonal complex line flag manifold](../../../fiber-bundle.md#cohomology-ring-of-the-orthogonal-complex-line-flag-manifold). Its additive basis is $x^iy^j$ with $0\leq i<n$, $0\leq j<n-1$. As a symmetry check, multiplying the second relation by $y-x$ gives $y^n-x^n=0$, so $y^n=0$ as expected from the second projection. For $n=2$, every line has a unique orthogonal line, and the relations become $x^2=0$, $x+y=0$, giving the ring of $\mathbb{CP}^1$. If $n=1$, the space is empty and the second relation is $1=0$, so the printed formula still gives the zero [cohomology ring](../../../cohomology.md#cohomology-ring).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
