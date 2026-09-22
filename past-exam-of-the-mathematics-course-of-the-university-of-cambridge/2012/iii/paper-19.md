# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_19.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Choose a generator $[S^n]$ of $\widetilde H_n(S^n;\mathbb Z)\cong\mathbb Z$. The [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) of a [continuous map](../../../topology.md#continuous-map) is the integer determined by

$$
\boxed{f_*[S^n]=(\deg f)[S^n].}
$$

For $n\geq1$ this is ordinary top-dimensional [homology](../../../homology.md); using [reduced homology](../../../homology.md#reduced-homology) also gives a convention for $n=0$. Domain and target use the same [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), so reversing the chosen generator in both leaves the integer unchanged. [Homotopy invariance of homology](../../../homology.md#homotopy-invariance-of-homology) makes the [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) invariant under [homotopy](../../../algebraic-topology.md#homotopy).

We interpret the [manifold criterion for a suspension](../../../algebraic-topology.md#manifold-criterion-for-a-suspension) in the category of nonempty [topological manifolds](../../../topology.md#topological-manifold) without boundary, and “[sphere](../../../geometry-and-topology.md#sphere)” as homeomorphic to the standard [sphere](../../../geometry-and-topology.md#sphere). Let $X$ have dimension $d$. If $X\cong S^d$, an explicit [homeomorphism](../../../topology.md#homeomorphism) from its [suspension](../../../algebraic-topology.md#suspension-topology) to $S^{d+1}$ is

$$
[x,t]\longmapsto(\sin(\pi t)x,\cos(\pi t)).
$$

It is a [continuous map](../../../topology.md#continuous-map) that is a [bijection](../../../function.md#bijection): the two collapsed ends become the poles, and every other point determines $t$ and $x$ uniquely. The [compact-to-Hausdorff continuous bijection theorem](../../../topology.md#compact-to-hausdorff-continuous-bijection-theorem) makes it a [homeomorphism](../../../topology.md#homeomorphism).

Conversely suppose $SX$ is a [topological manifold](../../../topology.md#topological-manifold). Its open part $X\times(0,1)$ shows its dimension is $d+1$. At a suspension vertex $v$ there is an open cone neighbourhood $U$ on $X$. It is [contractible](../../../algebraic-topology.md#contractible-space), while $U\setminus\{v\}$ admits a [deformation retraction](../../../algebraic-topology.md#deformation-retraction) onto $X$. The [long exact sequence in relative homology](../../../homology.md#long-exact-sequence-in-relative-homology) and [excision](../../../homology.md#excision-theorem) give the [local homology from a link](../../../homology.md#local-homology-from-a-link) calculation

$$
H_i(SX,SX\setminus\{v\};\mathbb Z)\cong\widetilde H_{i-1}(X;\mathbb Z).
$$

A point of a $(d+1)$-dimensional [topological manifold](../../../topology.md#topological-manifold) without boundary has [local homology](../../../homology.md#local-homology) $\mathbb Z$ in degree $d+1$ and zero in all other degrees. Consequently

$$
\widetilde H_j(X;\mathbb Z)\cong
\begin{cases}\mathbb Z,&j=d,\\0,&j\neq d.\end{cases}
$$

Thus $X$ is an [integral homology sphere](../../../cohomology.md#homology-sphere). This conclusion alone does not identify its [homeomorphism](../../../topology.md#homeomorphism) type.

If $d\geq2$, it is also [simply connected](../../../algebraic-topology.md#simply-connected-space). Choose a cone neighbourhood $U$ of the vertex and an open coordinate ball $B$ around the vertex inside $U$. By [compactness](../../../topology.md#compact-space) of $X$, sufficiently short entire cone neighbourhoods fit inside any neighbourhood of $v$: the inverse image of that neighbourhood contains $X\times\{0\}$, and a finite subcover supplies one uniform collar length. Choose such a shorter cone $V\subset B$. The inclusions of punctured neighbourhoods factor as

$$
V\setminus\{v\}\longrightarrow B\setminus\{v\}\longrightarrow U\setminus\{v\}.
$$

The composite induces an [isomorphism](../../../algebra.md#isomorphism) of [fundamental groups](../../../algebraic-topology.md#fundamental-group), since both cone punctures are products of $X$ with intervals and their inclusion is a [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence). The middle punctured ball has the [homotopy type](../../../algebraic-topology.md#homotopy-type) of $S^d$ and is [simply connected](../../../algebraic-topology.md#simply-connected-space) for $d\geq2$. Hence the composite is also zero on the [fundamental group](../../../algebraic-topology.md#fundamental-group), forcing $\pi_1(X)=0$. This uses the nested neighbourhoods, not an unsupported claim that an arbitrary punctured neighbourhood is a [sphere](../../../geometry-and-topology.md#sphere).

The [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem), applied successively to the vanishing lower [homology groups](../../../homology.md#homology-group), now gives $\pi_j(X)=0$ for $j<d$ and $\pi_d(X)\cong H_d(X)\cong\mathbb Z$. A representative of its generator is a [continuous map](../../../topology.md#continuous-map) $S^d\to X$ inducing an [isomorphism](../../../algebra.md#isomorphism) in every [integral homology](../../../homology.md#integral-homology) degree. [Topological manifolds](../../../topology.md#topological-manifold) have the [homotopy type](../../../algebraic-topology.md#homotopy-type) of [CW complexes](../../../algebraic-topology.md#cw-complex), so the [homological Whitehead theorem](../../../algebraic-topology.md#homological-whitehead-theorem) makes it a [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence). We have proved that $X$ is a [homotopy sphere](../../../cohomology.md#homotopy-sphere).

At this point the **topological classification theorem is essential**: the [topological generalized Poincare theorem](../../../cohomology.md#topological-generalized-poincare-theorem) says that a closed [homotopy sphere](../../../cohomology.md#homotopy-sphere) is homeomorphic to the standard [sphere](../../../geometry-and-topology.md#sphere). Applying it completes the converse for $d\geq2$. For $d=1$, the local calculation makes $X$ a connected [compact](../../../topology.md#compact-space) one-dimensional [manifold](../../../topology.md#topological-manifold) without boundary, hence a [circle](../../../topology.md#circle). For $d=0$, a [compact](../../../topology.md#compact-space) zero-dimensional [manifold](../../../topology.md#topological-manifold) is a finite set, and $\widetilde H_0(X)\cong\mathbb Z$ forces exactly two points. Thus it is $S^0$. Altogether,

$$
\boxed{SX\text{ is a topological manifold without boundary}\iff X\cong S^d.}
$$

The last classification step is not a consequence of [homology](../../../homology.md) alone, and we make no assertion of [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) with a prescribed smooth structure. If the word [manifold](../../../topology.md#topological-manifold) allows boundary on both sides, the printed assertion needs this correction: the suspension of the interval is a closed disk. For instance $[x,t]\mapsto((2x-1)(1-|2t-1|),2t-1)$ identifies it with the filled diamond $|u|+|v|\leq1$, although the interval is not a [sphere](../../../geometry-and-topology.md#sphere).

To construct [sphere maps of arbitrary integer degree](../../../homology.md#sphere-maps-of-arbitrary-integer-degree), first use $h_m:S^1\to S^1$, $h_m(z)=z^m$ for any integer $m$, including the constant map when $m=0$. Lifting its argument to the real line gives $\theta\mapsto m\theta$, so the fundamental one-cycle is sent to $m$ times itself. Therefore $\deg h_m=m$.

Two cone neighbourhoods cover a [suspension](../../../algebraic-topology.md#suspension-topology); their intersection admits a [deformation retraction](../../../algebraic-topology.md#deformation-retraction) onto the original space. The reduced [Mayer–Vietoris theorem](../../../algebraic-topology.md#mayer-vietoris-sequence) gives a natural [suspension isomorphism](../../../algebraic-topology.md#suspension-isomorphism)

$$
\widetilde H_{q+1}(SX)\cong\widetilde H_q(X).
$$

Naturality means that the [suspension](../../../algebraic-topology.md#suspension-topology) of a [continuous map](../../../topology.md#continuous-map) induces the same integer multiplier. This proves [degree under suspension](../../../homology.md#degree-under-suspension). Using the standard identification $S(S^k)\cong S^{k+1}$, set

$$
\boxed{f_{n,m}=S^{\,n-1}h_m:S^n\to S^n,\qquad \deg f_{n,m}=m\quad(n\geq1).}
$$

Thus every integer occurs in every positive [sphere](../../../geometry-and-topology.md#sphere) dimension, with negative degrees handled just as well as positive ones.

If “every $n$” includes zero, that final printed assertion is false. The generator of $\widetilde H_0(S^0)$ is the difference of its two points. A map of a two-point set is the identity, the transposition, or one of two constant maps, giving precisely

$$
\boxed{\deg f\in\{-1,0,1\}\quad\text{on }S^0.}
$$

These [degrees of maps of the zero-sphere](../../../homology.md#degrees-of-maps-of-the-zero-sphere) are the explicit exception to the arbitrary-degree construction.

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use [integral homology](../../../homology.md#integral-homology) throughout. The [singular chain group](../../../homology.md#singular-chain-group) $C_k(X)$ is free on the [continuous maps](../../../topology.md#continuous-map) from the standard $k$-simplex to $X$. Since the [boundary operator](../../../homology.md#boundary-operator) preserves chains lying in $A$, these form a [chain subcomplex](../../../homology.md#chain-subcomplex). The [relative chain complex](../../../homology.md#relative-chain-complex) and its [relative homology](../../../homology.md#relative-homology) are

$$
C_k(X,A)=C_k(X)/C_k(A),\qquad
\boxed{H_k(X,A)=\ker(\partial:C_k(X,A)\to C_{k-1}(X,A))/\operatorname{im}(\partial:C_{k+1}(X,A)\to C_k(X,A)).}
$$

The [short exact sequence of chain complexes](../../../homology.md#short-exact-sequence-of-chain-complexes) gives the [long exact sequence in relative homology](../../../homology.md#long-exact-sequence-in-relative-homology).

A sufficient hypothesis for the quotient comparison is a nonempty [good pair](../../../homology.md#good-pair): $A$ is closed and has an open neighbourhood $U$ which admits a [deformation retraction](../../../algebraic-topology.md#deformation-retraction) onto $A$ while fixing $A$ throughout. A [CW pair](../../../algebraic-topology.md#cw-pair) is another standard sufficient setting. These hypotheses hold for a simple closed curve in the surface here, using its annular [collar neighbourhood](../../../differential-geometry.md#collar-neighbourhood). The induced [quotient map](../../../topology.md#quotient-map) $q:X\to Y=X/A$ collapses $A$ to a point $a$.

Here is the proof of the [collapsing a pair theorem](../../../homology.md#collapsing-a-pair-theorem). Put $V=U/A\subset Y$. The [deformation retraction](../../../algebraic-topology.md#deformation-retraction) makes $H_*(U,A)=0$, so the [long exact sequence](../../../homology.md#long-exact-sequence) of the triple gives $H_*(X,A)\cong H_*(X,U)$. It also contracts $V$ onto $a$, giving $H_*(Y,\{a\})\cong H_*(Y,V)$. Because $A$ is closed inside the open neighbourhood $U$, [excision](../../../homology.md#excision-theorem) gives

$$
H_*(X,U)\cong H_*(X\setminus A,U\setminus A).
$$

Similarly, [excision](../../../homology.md#excision-theorem) of the closed point $a$ in the open set $V$ gives

$$
H_*(Y,V)\cong H_*(Y\setminus\{a\},V\setminus\{a\}).
$$

The [quotient map](../../../topology.md#quotient-map) restricts to a [homeomorphism](../../../topology.md#homeomorphism) between the two punctured pairs, so these are the same groups and the identifications commute with $q_*$. Finally $H_*(Y,\{a\})\cong\widetilde H_*(Y)$, including degree zero. Thus

$$
\boxed{q_*:H_k(X,A)\xrightarrow{\sim}\widetilde H_k(X/A).}
$$

The neighbourhood condition is part of the result; the quotient assertion is not made for arbitrary bad pairs.

For the genus-two [closed orientable surface](../../../topology.md#closed-orientable-surface) with its chosen [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), $H_0(X)=\mathbb Z$, $H_1(X)=\mathbb Z^4$, $H_2(X)=\mathbb Z$, with higher groups zero. The curve has $H_0(A)=H_1(A)=\mathbb Z$. Its relevant [long exact sequence in relative homology](../../../homology.md#long-exact-sequence-in-relative-homology) is

$$
0\longrightarrow\mathbb Z\longrightarrow H_2(X,A)
\longrightarrow\mathbb Z\xrightarrow{i_*}\mathbb Z^4
\longrightarrow H_1(X,A)\longrightarrow\mathbb Z\xrightarrow{\sim}\mathbb Z\longrightarrow0.
$$

The final map is an [isomorphism](../../../algebra.md#isomorphism) because both spaces are connected. Consequently $H_1(X,A)=\operatorname{coker}i_*$ and $H_0(X,A)=0$; all relative groups above degree two vanish. The [quotient topological space](../../../topology.md#quotient-topological-space) is connected, so its unreduced $H_0$ is $\mathbb Z$.

In the separating case, the curve is the oriented boundary of one of the two subsurfaces. Its [homology class](../../../homology.md#homology-class) in $X$ is therefore zero, so $i_*=0$. The [exact sequence](../../../homology.md#exact-sequence) becomes

$$
0\to\mathbb Z\to H_2(X,A)\to\mathbb Z\to0,
\qquad H_1(X,A)=\mathbb Z^4.
$$

The first sequence splits since its quotient is a free [abelian group](../../../group.md#abelian-group). Hence the [homology after collapsing a separating surface curve](../../../homology.md#homology-after-collapsing-a-separating-surface-curve) is

$$
\boxed{H_k(X/A;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,\\
\mathbb Z^4,&k=1,\\
\mathbb Z^2,&k=2,\\
0,&k\geq3.
\end{cases}}
$$

Geometrically, collapsing the boundary of each once-punctured [torus](../../../topology.md#torus) fills its puncture with a cone on the [circle](../../../topology.md#circle), which is a disk. The quotient is a [wedge sum](../../../topology.md#wedge-sum) of two tori at the collapsed point. Their two independent [fundamental classes](../../../cohomology.md#fundamental-class) explain the extra second-homology generator.

In the nonseparating case, join the two new boundary components of the cut surface by an arc. Upon regluing, this supplies a closed curve meeting $A$ once transversely. The signed [intersection pairing on an oriented surface](../../../cohomology.md#intersection-pairing-on-an-oriented-surface) therefore provides an integer homomorphism $H_1(X)\to\mathbb Z$ taking $[A]$ to $\pm1$. Thus $[A]$ is a nonzero [primitive homology class](../../../homology.md#primitive-homology-class), and $i_*:\mathbb Z\to\mathbb Z^4$ is an injection onto a direct summand. Its kernel is zero and its cokernel is $\mathbb Z^3$. The same [exact sequence](../../../homology.md#exact-sequence) gives $H_2(X,A)\cong H_2(X)\cong\mathbb Z$. Therefore the [homology after collapsing a nonseparating surface curve](../../../homology.md#homology-after-collapsing-a-nonseparating-surface-curve) is

$$
\boxed{H_k(X/A;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,2,\\
\mathbb Z^3,&k=1,\\
0,&k\geq3.
\end{cases}}
$$

Another description starts from the genus-one surface with two boundary circles. Collapse those two circles separately to obtain a closed [torus](../../../topology.md#torus) with two marked points, then identify the two points. Identifying two distinct points in a connected [CW complex](../../../algebraic-topology.md#cw-complex) adds a loop up to [homotopy](../../../algebraic-topology.md#homotopy), so this quotient has the [homotopy type](../../../algebraic-topology.md#homotopy-type) of $T^2\vee S^1$. The preceding [relative homology](../../../homology.md#relative-homology) calculation proves the groups without requiring that [homotopy](../../../algebraic-topology.md#homotopy) description.

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [CW complex](../../../algebraic-topology.md#cw-complex) $X$, let $X^k$ be its $k$-skeleton. The [cellular chain complex](../../../homology.md#cellular-chain-complex) is

$$
C_k^{\mathrm{cell}}(X)=H_k(X^k,X^{k-1};\mathbb Z)\cong\bigoplus_{\text{$k$-cells }e}\mathbb Z[e].
$$

The [isomorphism](../../../algebra.md#isomorphism) uses [excision](../../../homology.md#excision-theorem) and $H_k(D^k,S^{k-1})\cong\mathbb Z$, after choosing an [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) for each cell. In degree zero, take $X^{-1}=\varnothing$ and the free group on the vertices. The differential is the composite

$$
H_k(X^k,X^{k-1})\xrightarrow{\partial}H_{k-1}(X^{k-1})
\longrightarrow H_{k-1}(X^{k-1},X^{k-2}).
$$

The [long exact sequences](../../../homology.md#long-exact-sequence) of skeleton pairs imply $d_{k-1}d_k=0$. The [cellular boundary formula](../../../homology.md#cellular-boundary-formula) describes its coefficient at a $(k-1)$-cell as the [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) of the attaching [sphere](../../../geometry-and-topology.md#sphere) after all other $(k-1)$-cells are collapsed. In degree one this is the signed difference of the two endpoints. The [cellular homology theorem](../../../homology.md#cellular-homology-theorem) identifies the [homology](../../../homology.md) of this complex with [singular homology](../../../homology.md#singular-homology): relative [homology](../../../homology.md) of successive skeletons is concentrated in their cell dimension, and the exact skeleton sequences leave precisely these kernels modulo images. This is the construction, rather than merely a count of cells.

The filtration $\mathbb{CP}^0\subset\mathbb{CP}^1\subset\mathbb{CP}^2$ gives one cell in each of dimensions zero, two and four, since $\mathbb{CP}^k\setminus\mathbb{CP}^{k-1}\cong\mathbb C^k$. There are no odd-dimensional cells, so every cellular differential vanishes. Thus

$$
H_k(\mathbb{CP}^2;\mathbb Z)\cong\begin{cases}\mathbb Z,&k=0,2,4,\\0,&\text{otherwise}.\end{cases}
$$

The [complex projective line](../../../algebraic-topology.md#complex-projective-line) has one zero-cell and one two-cell. Its product with itself has one zero-cell, two two-cells and one four-cell. Its [cellular chain complex](../../../homology.md#cellular-chain-complex) again has zero differentials, giving

$$
H_k(\mathbb{CP}^1\times\mathbb{CP}^1;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,4,\\\mathbb Z^2,&k=2,\\0,&\text{otherwise}.
\end{cases}
$$

A [homeomorphism](../../../topology.md#homeomorphism) induces [isomorphisms](../../../algebra.md#isomorphism) on [homology groups](../../../homology.md#homology-group). The second groups have different ranks, and therefore

$$
\boxed{\mathbb{CP}^2\not\cong\mathbb{CP}^1\times\mathbb{CP}^1.}
$$

Now orient the [Complex projective plane](../../../algebraic-topology.md#complex-projective-plane) by its complex coordinates. The inclusion of its two-skeleton $\mathbb{CP}^1$ identifies the [fundamental class](../../../cohomology.md#fundamental-class) of a projective line with a generator $h$ of $H_2(\mathbb{CP}^2;\mathbb Z)\cong\mathbb Z$: the cellular generator has no incoming three-cell boundary and no outgoing boundary.

Take the projective lines $L_0=\{z_2=0\}$ and $L_1=\{z_1=0\}$. A path of unitary coordinate transformations takes one to the other, so their oriented [homology classes](../../../homology.md#homology-class) are both $h$. They meet in the single point $[1:0:0]$. In its affine chart, let $w=z_1/z_0$ and $v=z_2/z_0$. Their [tangent spaces](../../../differential-geometry.md#tangent-space) are the complex $w$-axis and complex $v$-axis, so the intersection is a [transverse intersection](../../../differential-geometry.md#transverse-intersection). The ordered real bases

$$
(\partial_{\operatorname{Re}w},\partial_{\operatorname{Im}w}),
\qquad(\partial_{\operatorname{Re}v},\partial_{\operatorname{Im}v})
$$

concatenate to the complex [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) of the ambient four-manifold. Thus the local sign is $+1$, and

$$
\boxed{h\cdot h=[L_0]\cdot[L_1]=1.}
$$

This computes the [intersection form](../../../homology.md#intersection-form) using distinct representatives of the same class, avoiding an ill-defined attempt to count a line intersecting itself as a set. Bilinearity now gives

$$
\lambda(ah,bh)=ab,\qquad [\lambda]_{h}=(1),\qquad\det[\lambda]=1.
$$

Equivalently, the map $H_2\to\operatorname{Hom}(H_2,\mathbb Z)$ sending $a$ to $\lambda(a,-)$ is an [isomorphism](../../../algebra.md#isomorphism). This is exactly a [unimodular intersection pairing](../../../homology.md#unimodular-intersection-pairing), and proves [projective lines generate a unimodular intersection form](../../../algebraic-topology.md#projective-lines-generate-a-unimodular-intersection-form). Reversing the ambient [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) would change the matrix to $(-1)$ and would still be unimodular.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The multiplicative [norm](../../../functional-analysis.md#norm) first rules out [zero divisors](../../../mathematics.md#zero-divisor): if $xy=0$ and $x\neq0$, then $0=|x||y|$ forces $y=0$. If the dimension is zero the claimed bound already holds, so suppose it is positive.

It is worth checking that the printed description of a ring with an underlying real [vector space](../../../vector-space.md) really permits differentiation of multiplication. This follows from the norm identity even if compatibility with real scalars is not separately stated. For fixed $x$, the map $L_x(y)=xy$ is additive by distributivity, and

$$
|L_x(y)-L_x(z)|=|x(y-z)|=|x||y-z|.
$$

It is therefore [continuous](../../../calculus.md#continuous-function). Additivity gives rational linearity. Approximating a real number by rationals and using continuity proves $L_x(ty)=tL_x(y)$ for every real $t$. The same argument holds in the other variable. This is [automatic real bilinearity from a multiplicative norm](../../../algebra.md#automatic-real-bilinearity-from-a-multiplicative-norm), so multiplication is a [bilinear map](../../../linear-algebra.md#bilinear-map) between finite-dimensional [vector spaces](../../../vector-space.md), and hence is smooth.

Let $S=\{x\in A:|x|=1\}$ be the [unit sphere](../../../topology.md#unit-sphere) of the given [positive-definite bilinear form](../../../linear-algebra.md#positive-definite-bilinear-form). It is a copy of $S^{n-1}$. The squaring map

$$
Q:S\to S,\qquad Q(x)=x^2,
$$

is well defined because $|x^2|=|x|^2=1$, and is smooth. [Commutativity](../../../algebra.md#commutativity) gives its derivative

$$
DQ_x(v)=xv+vx=2xv.
$$

For $x\in S$ and $v\neq0$, the norm identity gives $|DQ_x(v)|=2|v|$, so the derivative is injective, including on the [tangent space](../../../differential-geometry.md#tangent-space) $T_xS=x^\perp$. It takes tangent vectors into $T_{x^2}S$ since $Q$ maps the [sphere](../../../geometry-and-topology.md#sphere) to itself. Alternatively, polarization of $|xy|^2=|x|^2|y|^2$ gives $\langle xy,xz\rangle=|x|^2\langle y,z\rangle$, so $\langle x^2,2xv\rangle=2\langle x,v\rangle=0$ directly.

The only identifications under squaring are antipodal:

$$
Q(x)=Q(y)\ \Longrightarrow\ (x-y)(x+y)=0\ \Longrightarrow\ y=x\text{ or }y=-x.
$$

The factorization uses [commutativity](../../../algebra.md#commutativity), and the last implication uses the absence of [zero divisors](../../../mathematics.md#zero-divisor). Conversely $Q(-x)=Q(x)$. It follows that $Q$ induces an injective smooth map

$$
q:\mathbb{RP}^{n-1}=S/(x\sim-x)\longrightarrow S^{n-1}.
$$

The antipodal [quotient map](../../../topology.md#quotient-map) is a local [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), so the injectivity of $DQ$ implies injectivity of $Dq$. Since [Real projective space](../../../algebraic-topology.md#real-projective-space) is [compact](../../../topology.md#compact-space), the stated [compact injective immersion is an embedding](../../../differential-geometry.md#compact-injective-immersion-is-an-embedding) theorem makes $q$ a closed embedding.

For $n\geq2$ its source and target have the same dimension $n-1$. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes its image open as well as closed in the connected [sphere](../../../geometry-and-topology.md#sphere) $S^{n-1}$. It is nonempty, so the image is the whole [sphere](../../../geometry-and-topology.md#sphere); consequently $q$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism). But for $n\geq3$ this is impossible:

$$
\pi_1(\mathbb{RP}^{n-1})\cong\mathbb Z/2,
\qquad \pi_1(S^{n-1})=0.
$$

Indeed, the antipodal two-sheeted [covering map](../../../algebraic-topology.md#covering-space) $S^{n-1}\to\mathbb{RP}^{n-1}$ has simply connected total space in this range, and is its [universal cover](../../../algebraic-topology.md#universal-cover), with deck group $\mathbb Z/2$. A [sphere](../../../geometry-and-topology.md#sphere) of dimension at least two is [simply connected](../../../algebraic-topology.md#simply-connected-space). These [fundamental groups](../../../algebraic-topology.md#fundamental-group) cannot be those of homeomorphic spaces.

We have obtained the [dimension bound for a commutative Euclidean normed algebra](../../../algebra.md#dimension-bound-for-a-commutative-euclidean-normed-algebra):

$$
\boxed{\dim_{\mathbb R}A\leq2.}
$$

The real numbers and complex numbers with their usual products and Euclidean norms attain dimensions one and two. In dimension two, the induced map $\mathbb{RP}^1\to S^1$ is entirely compatible with the argument: the [circle](../../../topology.md#circle) squaring map identifies exactly the two antipodal preimages. We neither assume a multiplicative identity nor use a classification of real division algebras; the squaring argument proves the bound from the supplied hypotheses.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
