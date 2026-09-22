# Paper 114

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_114.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_114.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
    - [2](#1/1/2)
      - [Solution](#1/1/2/solution)
    - [3](#1/1/3)
      - [Solution](#1/1/3/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
    - [3](#2/2/3)
      - [Solution](#2/2/3/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Let $x,y\in H^n(S^n\times S^n;\mathbb Z)$ be the pullbacks of the two orientation classes. The [cohomology ring of a product of two spheres](../../../cohomology.md#cohomology-ring-of-a-product-of-two-spheres) has

$$
x^2=y^2=0,
\qquad xy=(-1)^nyx,
$$

and $xy$ generates $H^{2n}\cong\mathbb Z$. Write

$$
f^*x=ax+by,
\qquad f^*y=cx+dy.
$$

The matrix $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ lies in $GL_2(\mathbb Z)$ because a [homeomorphism](../../../topology.md#homeomorphism) induces a [cohomology ring](../../../cohomology.md#cohomology-ring) automorphism.

If $n$ is even, graded commutativity gives

$$
0=(f^*x)^2=2ab\,xy,
\qquad
0=(f^*y)^2=2cd\,xy.
$$

Thus $ab=cd=0$. Invertibility forces $A$ to be diagonal or anti-diagonal, and its two nonzero entries must each be $\pm1$. Hence **there are exactly eight possible actions: the signed permutation matrices**.

Evenness is necessary. For $n=1$, the product is the [torus](../../../topology.md#torus), and every $A\in GL_2(\mathbb Z)$ is induced by an [integral linear automorphism of the torus](../../../topology.md#integral-linear-automorphism-of-the-torus). For example, the infinitely many matrices $\begin{pmatrix}1&m\\0&1\end{pmatrix}$ give distinct actions on $H^1$.

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

The [cellular chain complex](../../../homology.md#cellular-chain-complex) for either space has one cell in dimensions $0,2,3,4$, with the only nonzero differential equal to multiplication by $p$ from degree three to degree two. The [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology) therefore gives, for both $X$ and $Y$,

$$
H^j(-;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&j=0,4,\\
\mathbb Z/p,&j=3,\\
0,&\text{otherwise}.
\end{cases}
$$

Every product of positive-degree classes vanishes for dimensional reasons, so

$$
\boxed{H^*(X;\mathbb Z)\cong H^*(Y;\mathbb Z)\text{ as graded rings}.}
$$

Their modulo-$p$ [cohomology rings](../../../cohomology.md#cohomology-ring) distinguish them. Let $u\in H^2(X;\mathbb F_p)$ be the class restricting to the standard generator on $\mathbb{CP}^2$. The attaching map has degree $p$, so its cellular coboundary vanishes modulo $p$; the classes in degrees two and four restrict isomorphically to those of $\mathbb{CP}^2$. Hence $u^2\ne0$ in $H^4(X;\mathbb F_p)$. In $Y=M(\mathbb Z/p,2)\vee S^4$, the degree-two class comes from the three-dimensional [Moore space](../../../algebraic-topology.md#moore-space-algebraic-topology), so its square is zero; products between distinct wedge summands also vanish. The [mod-p cup-square obstruction to a homotopy equivalence](../../../cohomology.md#mod-p-cup-square-obstruction-to-a-homotopy-equivalence) now proves

$$
\boxed{X\not\simeq Y.}
$$

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/solution">Solution</h5>

↑ **Parent:** [3](#1/1/3)

The standard [cellular chain complex](../../../homology.md#cellular-chain-complex) of the [Klein bottle](../../../topology.md#klein-bottle) gives

$$
H_0(K;\mathbb Z)=\mathbb Z,
\qquad H_1(K;\mathbb Z)=\mathbb Z\oplus\mathbb Z/2,
\qquad H_2(K;\mathbb Z)=0.
$$

The [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology) therefore yields $H^0=\mathbb Z$, $H^1=\mathbb Z$, and $H^2=\mathbb Z/2$. The degree-one generator is pulled back from the base circle in the circle-bundle description of $K$, so its square is zero. Thus every positive-degree product vanishes. The same calculation for $\mathbb{RP}^2\vee S^1$ gives the [integral cohomology ring of the wedge of the real projective plane and a circle](../../../topology.md#integral-cohomology-ring-of-the-wedge-of-the-real-projective-plane-and-a-circle), and hence

$$
\boxed{H^*(K;\mathbb Z)\cong H^*(\mathbb{RP}^2\vee S^1;\mathbb Z).}
$$

There is no map $Y\to K$ inducing this isomorphism. The Klein bottle is an [aspherical space](../../../algebraic-topology.md#aspherical-space), and its [fundamental group](../../../algebraic-topology.md#fundamental-group) is torsion-free. Any map $\mathbb{RP}^2\to K$ therefore induces the trivial homomorphism $\mathbb Z/2\to\pi_1(K)$ and is [null-homotopic](../../../algebraic-topology.md#null-homotopic-map). Its pullback on $H^2$ is zero, while the circle summand has no degree-two cohomology. Consequently every map $Y\to K$ is zero on $H^2(K;\mathbb Z)$ and cannot be a cohomology isomorphism.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

A [direct system of abelian groups](../../../module-theory.md#direct-system-of-abelian-groups) over the directed poset $A$ consists of groups $G_a$ and maps $\phi_{ab}:G_a\to G_b$ for $a\leq b$, satisfying $\phi_{aa}=1$ and $\phi_{bc}\phi_{ab}=\phi_{ac}$. Its [direct limit](../../../module-theory.md#direct-limit-of-abelian-groups) is the quotient of $\bigoplus_aG_a$ by the relations $g_a\sim\phi_{ab}(g_a)$.

For the displayed sequence, put $P_0=1$ and $P_n=a_0a_1\cdots a_{n-1}$. Map the copy of $\mathbb Z$ at stage $n$ to $\mathbb Q$ by

$$
m\longmapsto \frac{m}{P_n}.
$$

This is compatible with the next transition because $a_nm/P_{n+1}=m/P_n$. The universal property of the [direct limit](../../../module-theory.md#direct-limit-of-abelian-groups) therefore identifies it with

$$
\boxed{\bigcup_{n\geq0}\frac1{P_n}\mathbb Z.}
$$

In reduced form, these are exactly the rationals whose denominator divides one of the finite products $P_n$. This is the [sequential direct limit of multiplication maps on the integers](../../../module-theory.md#sequential-direct-limit-of-multiplication-maps-on-the-integers).

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

Every [singular simplex](../../../homology.md#singular-simplex) has compact image, and a [singular chain](../../../homology.md#singular-chain) is a finite sum of simplices. The image of any chain is therefore compact and lies in some $X_a$. Directedness puts any finite collection of chains into one common $X_b$, so

$$
C_*(X;\mathbb Z)=\varinjlim_aC_*(X_a;\mathbb Z).
$$

Because [filtered colimits](../../../module-theory.md#filtered-colimit-of-modules) of [abelian groups](../../../group.md#abelian-group) are exact, kernels and images commute with this colimit. Taking homology gives the [homology of a directed union](../../../homology.md#homology-of-a-directed-union):

$$
\boxed{H_i(X;\mathbb Z)\cong\varinjlim_aH_i(X_a;\mathbb Z).}
$$

For an open $U\subseteq\mathbb R^N$, use the directed family of finite unions of closed rational cubes contained in $U$. Every compact subset of $U$ lies in one such finite polyhedron, and each polyhedron has finitely generated [cellular homology](../../../homology.md#cellular-chain-complex). There are only countably many of them, so their direct limit is countable. Thus **every $H_i(U;\mathbb Z)$ is countable**.

Cohomology behaves differently because $\operatorname{Hom}$ turns a direct sum into a direct product. The connected open set

$$
U=\mathbb R^2\setminus\{(n,0):n\geq1\}
$$

has one independent loop around each puncture, so $H_1(U;\mathbb Z)\cong\bigoplus_{n\geq1}\mathbb Z$. Since $H_0(U;\mathbb Z)=\mathbb Z$, the [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology) gives

$$
\boxed{H^1(U;\mathbb Z)\cong\operatorname{Hom}\left(\bigoplus_{n\geq1}\mathbb Z,\mathbb Z\right)
\cong\prod_{n\geq1}\mathbb Z,}
$$

which is uncountable. This is the [first cohomology of the countably punctured plane](../../../cohomology.md#first-cohomology-of-the-countably-punctured-plane).

<h4 id="2/2/3">3</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/3/solution">Solution</h5>

↑ **Parent:** [3](#2/2/3)

List the prime numbers without repetition as $p_0,p_1,p_2,\ldots$. Choose maps

$$
S^n\xrightarrow{f_i}S^n,
\qquad \deg f_i=p_i,
$$

and let $T$ be their [mapping telescope](../../../algebraic-topology.md#mapping-telescope). A finite initial telescope deformation retracts onto its last sphere. The inclusions of successive finite telescopes induce multiplication by $p_i$ on degree-$n$ reduced homology. The [homology of a directed union](../../../homology.md#homology-of-a-directed-union) and the [sequential direct limit of multiplication maps on the integers](../../../module-theory.md#sequential-direct-limit-of-multiplication-maps-on-the-integers) therefore give

$$
\widetilde H_j(T;\mathbb Z)
\cong
\begin{cases}
\varinjlim(\mathbb Z\xrightarrow{p_0}\mathbb Z\xrightarrow{p_1}\cdots),&j=n,\\
0,&j\ne n.
\end{cases}
$$

Every finite product $p_0\cdots p_r$ is square-free, and every square-free denominator divides one such product. Hence

$$
\boxed{\widetilde H_j(T;\mathbb Z)\cong
\begin{cases}
\mathbb Q_{\mathrm{sq}},&j=n,\\
0,&j\ne n,
\end{cases}}
$$

as in the [mapping-telescope realization of the rational group with square-free denominators](../../../algebraic-topology.md#mapping-telescope-realization-of-the-rational-group-with-square-free-denominators).

<h2 id="3">3</h2>

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An $R$-orientation of a rank-$d$ real [vector bundle](../../../fiber-bundle.md#vector-bundle) $E\to B$ is a locally coherent choice of generator of $H^d(E_b,E_b\setminus\{0\};R)$ in every fibre. Equivalently, it is represented by a [Thom class](../../../fiber-bundle.md#thom-class) $u_E\in H^d(D(E),S(E);R)$ restricting to the chosen generator on each fibre pair. If $e(E)\in H^d(B;R)$ is the [Euler class](../../../fiber-bundle.md#euler-class-of-a-vector-bundle), the [Gysin sequence](../../../fiber-bundle.md#gysin-sequence-of-a-sphere-bundle) of its unit sphere bundle contains

$$
\cdots\to H^{q-d}(B;R)\xrightarrow{\smile e(E)}H^q(B;R)
\to H^q(S(E);R)\to H^{q-d+1}(B;R)\xrightarrow{\smile e(E)}H^{q+1}(B;R)\to\cdots.
$$

The diagonal quotient defining $L(p)$ is the [three-dimensional lens space as a circle bundle](../../../fiber-bundle.md#three-dimensional-lens-space-as-a-circle-bundle) $S^1\to L(p)\to S^2$ with Euler class $p$ times a generator. With integral coefficients, the only nontrivial Euler-class map is multiplication by $p:H^0(S^2;\mathbb Z)\to H^2(S^2;\mathbb Z)$. Exactness gives

$$
\boxed{H^j(L(p);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&j=0,3,\\
\mathbb Z/p,&j=2,\\
0,&\text{otherwise}.
\end{cases}}
$$

Modulo $p$, the Euler class vanishes, so the same [Gysin sequence](../../../fiber-bundle.md#gysin-sequence-of-a-sphere-bundle) gives

$$
\boxed{H^j(L(p);\mathbb F_p)\cong\mathbb F_p\quad(0\leq j\leq3),}
$$

with all other groups zero.

For the coefficient sequence $0\to\mathbb Z\xrightarrow{p}\mathbb Z\to\mathbb F_p\to0$, the [long exact sequence from a coefficient sequence](../../../homology.md#long-exact-sequence-from-a-coefficient-sequence) contains

$$
0=H^1(L(p);\mathbb Z)\to H^1(L(p);\mathbb F_p)
\xrightarrow{\delta}H^2(L(p);\mathbb Z)
\xrightarrow{p}H^2(L(p);\mathbb Z).
$$

The last map is zero and both middle groups have order $p$, so $\delta$ is an isomorphism. Reduction $H^2(L(p);\mathbb Z)\to H^2(L(p);\mathbb F_p)$ is likewise an isomorphism. Their composite is the [Bockstein isomorphism for a three-dimensional lens space](../../../homology.md#bockstein-isomorphism-for-a-three-dimensional-lens-space)

$$
\boxed{\beta:H^1(L(p);\mathbb F_p)\xrightarrow{\sim}H^2(L(p);\mathbb F_p).}
$$

If $a'=na$ is another generator, linearity of the [Bockstein homomorphism](../../../homology.md#bockstein-homomorphism) and bilinearity of the [cup product](../../../cohomology.md#cup-product) give

$$
\boxed{t(a')=n^2t(a).}
$$

Moreover $t(a)\ne0$: $\beta(a)$ is nonzero, and the [Poincare duality](../../../cohomology.md#poincare-duality) pairing $H^1\times H^2\to H^3\cong\mathbb F_p$ is nondegenerate. If $h:L(p)\to L(p)$ is an orientation-reversing [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence) and $h^*a=na$, naturality gives

$$
n^2t(a)=t(h^*a)
=\langle h^*(a\smile\beta a),[L(p)]\rangle
=\langle a\smile\beta a,h_*[L(p)]\rangle
=-t(a).
$$

Cancelling the nonzero $t(a)$ yields $n^2\equiv-1\pmod p$. Thus **$-1$ must be a [quadratic residue](../../../number-theory.md#quadratic-residue) modulo $p$**.

## 4

↑ **Parent:** [Paper 114](paper-114.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $m=\dim M$. Choose a homogeneous basis $e_{q,i}$ of $H^q(M;\mathbb Q)$ and its [Poincare dual](../../../cohomology.md#poincare-dual) basis $e_{q,i}^*\in H^{m-q}(M;\mathbb Q)$, normalized by

$$
\langle e_{q,i}\smile e_{q,j}^*,[M]\rangle=\delta_{ij}.
$$

With the product orientation, the [cohomology class of the diagonal](../../../algebraic-topology.md#cohomology-class-of-the-diagonal) is

$$
\boxed{\varepsilon_\Delta=\sum_{q,i}(-1)^{mq}e_{q,i}^*\times e_{q,i}.}
$$

Indeed, multiplying this class by $\alpha\times\gamma$ and evaluating on $[M\times M]$ gives $\langle\alpha\smile\gamma,[M]\rangle$, which characterizes the [Poincare dual](../../../cohomology.md#poincare-dual) of $\Delta$.

Pulling back along the graph map $(1,f):M\to M\times M$ and evaluating gives the [graph-diagonal formula for the Lefschetz number](../../../algebraic-topology.md#graph-diagonal-formula-for-the-lefschetz-number):

$$
\left\langle(1,f)^*\varepsilon_\Delta,[M]\right\rangle
=\sum_q(-1)^q\operatorname{tr}(f^*|H^q(M;\mathbb Q))
=L(f).
$$

If $f$ has no fixed point, its graph is disjoint from $\Delta$. Represent $\varepsilon_\Delta$ with support in a tubular neighbourhood disjoint from the graph; its pullback is zero, so $L(f)=0$. Contrapositively, **$L(f)\ne0$ implies that $f$ has a fixed point**, the [Lefschetz fixed-point theorem](../../../algebraic-topology.md#lefschetz-fixed-point-theorem).

Now let $M$ be three disjoint circles. A homeomorphism permutes their three components. Its action on $H^1(M;\mathbb Z)\cong\mathbb Z^3$ is a signed permutation matrix. A component fixed setwise contributes to the trace by the degree of the corresponding circle homeomorphism. An orientation-reversing circle homeomorphism has a fixed point, so fixed-point-freeness forces that degree to be $+1$. Nonfixed components contribute zero. The trace is therefore the number of fixed points of a permutation of three objects, and

$$
\boxed{\operatorname{tr}(f^*|H^1(M;\mathbb Z))\in\{0,1,3\}.}
$$

For a compact manifold $N$ with boundary, let $D(N)=N_+\cup_{\partial N}N_-$ be its double and define $F$ by applying $f$ on both copies. The [Mayer–Vietoris sequence](../../../algebraic-topology.md#mayer-vietoris-sequence) for this decomposition is natural under $F$. Alternating traces in a finite-dimensional exact sequence sum to zero, so the two copies of $N$ contribute twice and their intersection contributes with the opposite sign:

$$
\boxed{L(F)=2L(f)-L(f|_{\partial N}).}
$$

This is the [Lefschetz number of a doubled map](../../../algebraic-topology.md#lefschetz-number-of-a-doubled-map).

Finally let $N$ be a [pair of pants](../../../topology.md#pair-of-pants-mathematics). If $f$ is fixed-point-free, so are its double $F$ and its boundary restriction. The [Lefschetz fixed-point theorem](../../../algebraic-topology.md#lefschetz-fixed-point-theorem) and the displayed identity give $L(F)=L(f|_{\partial N})=0$, hence $L(f)=0$. Since $N$ is connected and $H^i(N;\mathbb Q)$ is nonzero only for $i=0,1$,

$$
\operatorname{tr}(f^*|H^1(N;\mathbb Q))=1.
$$

Suppose the boundary permutation $\sigma$ had a fixed component. The restriction there is a fixed-point-free circle homeomorphism and thus has degree $+1$, forcing $f$ to preserve the surface orientation. The [homology action of a pair-of-pants homeomorphism](../../../topology.md#homology-action-of-a-pair-of-pants-homeomorphism) would then have trace $\#\operatorname{Fix}(\sigma)-1$, which is $2$ for the identity permutation and $0$ for a transposition. Neither is $1$. Therefore $\sigma$ has no fixed component; a permutation of three objects with no fixed point is a three-cycle. Thus

$$
\boxed{f\text{ cyclically permutes the three boundary components}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
