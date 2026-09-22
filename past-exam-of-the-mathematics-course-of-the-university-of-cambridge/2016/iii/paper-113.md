# Paper 113

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_113.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_113.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)

## 1

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The points of the [spectrum of a commutative ring](../../../ringed-space.md#spectrum-of-a-commutative-ring) $A$ are its [prime ideals](../../../commutative-algebra.md#prime-ideal). Its [Zariski topology](../../../algebraic-geometry.md#zariski-topology) has closed sets $V(I)=\{\mathfrak p:I\subseteq\mathfrak p\}$ and basis $D(f)=\{\mathfrak p:f\notin\mathfrak p\}$. The [structure sheaf of a scheme](../../../ringed-space.md#structure-sheaf-of-a-scheme) can be defined as follows: a section over $U$ assigns an element of $A_{\mathfrak q}$ to every $\mathfrak q\in U$, and locally that assignment is represented by one fraction $a/s$, with $s$ outside every prime in the neighbourhood. Restrictions forget values. Local representability and equality can be checked on an [open cover](../../../topology.md#open-cover), so these assignments satisfy the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom). On $D(f)$ the sections identify with the [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) $A_f$.

Evaluation at $\mathfrak p$ induces the [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) $\mathcal O_{X,\mathfrak p}\to A_{\mathfrak p}$. It is surjective because $a/s\in A_{\mathfrak p}$ is represented by a section on $D(s)$. For injectivity, represent a germ by $a/s$ on a neighbourhood of $\mathfrak p$. If its value in $A_{\mathfrak p}$ vanishes, there is $t\notin\mathfrak p$ with $ta=0$. The section is then zero after restricting to $D(st)$ inside that neighbourhood. Its [germ](../../../ringed-space.md#germ-of-a-sheaf-section) is zero. Thus

$$
\boxed{\mathcal O_{X,\mathfrak p}\cong A_{\mathfrak p}.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Put $A=k[t_1,t_2]$. The [punctured affine plane](../../../ringed-space.md#punctured-affine-plane) is covered by the [principal open subschemes](../../../ringed-space.md#principal-open-subscheme) $D(t_1)$ and $D(t_2)$. Since $A$ is an [integral domain](../../../commutative-algebra.md#integral-domain), restriction identifies its [global sections](../../../ringed-space.md#global-section) with

$$
\Gamma(X,\mathcal O_X)=A_{t_1}\cap A_{t_2}\subset k(t_1,t_2).
$$

This intersection is $A$: if $a/t_1^r=b/t_2^s$, then $t_2^sa=t_1^rb$, and [unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain) forces $t_1^r$ to divide $a$. Therefore the inclusion $j:X\hookrightarrow\operatorname{Spec}A$ induces the identity on [global regular functions](../../../ringed-space.md#global-regular-function).

If $X$ were an [affine scheme](../../../ringed-space.md#affine-scheme), [affine scheme reconstruction from global sections](../../../ringed-space.md#affine-scheme-reconstruction-from-global-sections) would make $j$ an [isomorphism of schemes](../../../ringed-space.md#isomorphism-of-schemes), because its global-section map is an isomorphism. But its image omits the closed point $(t_1,t_2)$. **The punctured affine plane is therefore not affine.** This is a useful example of global regular functions failing to distinguish a nonaffine open subscheme from its affine ambient space.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

An [isomorphism of schemes](../../../ringed-space.md#isomorphism-of-schemes) over $\mathbb R$ induces a bijection on [rational points](../../../algebraic-geometry.md#rational-point). A real point of this [projective plane curve](../../../algebraic-geometry.md#projective-plane-curve) would be represented by a nonzero real triple with $t_0^2+t_1^2+t_2^2=0$. Each summand is nonnegative, so every coordinate would vanish. Thus $X(\mathbb R)=\varnothing$, whereas $[1:0]\in\mathbb P^1(\mathbb R)$. **The two real schemes are not isomorphic.** The obstruction is the [real conic without real rational points](../../../algebraic-geometry.md#real-conic-without-real-rational-points); nonsingularity alone does not make a real conic a projective line over its ground field.

## 2

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [fibre product of schemes](../../../ringed-space.md#fiber-product-of-schemes) $Z=X\times_SY$ has projection morphisms to $X$ and $Y$ with equal composites to $S$, and for every [scheme](../../../ringed-space.md#scheme) $T$ the induced map is a bijection

$$
\operatorname{Hom}(T,Z)\cong\operatorname{Hom}(T,X)\times_{\operatorname{Hom}(T,S)}\operatorname{Hom}(T,Y).
$$

This [universal property](../../../category-theory.md#universal-property) determines $Z$ uniquely up to unique isomorphism. On affine charts over $\operatorname{Spec}R$, take

$$
\operatorname{Spec}A\times_{\operatorname{Spec}R}\operatorname{Spec}B
=\operatorname{Spec}(A\otimes_RB).
$$

The [tensor product of commutative algebras](../../../module-theory.md#tensor-product-of-commutative-algebras) has the required universal property for ring maps. Localization identifies these constructions on principal-open overlaps. Cover the base and its two inverse images by affine charts and glue the resulting affine products along those overlaps; their local universal properties give the global one.

For a counterexample to preservation of irreducibility, take $X=Y=\operatorname{Spec}\mathbb C$ and $S=\operatorname{Spec}\mathbb R$ with their usual structure morphisms. All three are [integral schemes](../../../ringed-space.md#integral-scheme), but the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives

$$
\mathbb C\otimes_{\mathbb R}\mathbb C
\cong\mathbb C[z]/(z^2+1)\cong\mathbb C\times\mathbb C.
$$

**The product scheme is the disjoint union of two points**, so it is not irreducible.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Work first over an affine neighbourhood $\operatorname{Spec}A$ of $y=\mathfrak p$, with an affine chart $\operatorname{Spec}B$ in its inverse image. The [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) on this chart has ring

$$
B\otimes_A\kappa(\mathfrak p)
\cong S^{-1}B/\mathfrak p S^{-1}B,\qquad S=A\setminus\mathfrak p,
$$

where $\kappa(\mathfrak p)$ is the [residue field](../../../commutative-algebra.md#residue-field). The [prime ideal correspondence for localization](../../../commutative-algebra.md#prime-ideal-correspondence-for-localization) and the correspondence for a quotient identify its points with primes $\mathfrak q\subset B$ containing $\mathfrak p B$ and disjoint from $S$. These two conditions are exactly $\mathfrak q\cap A=\mathfrak p$.

Under this bijection, each principal open $D(b\otimes1)$ corresponds to $D(b)\cap f^{-1}\{y\}$. These are bases for the two topologies: every element of the fibre ring is represented by $b/s$, with the image of $s$ invertible. Thus the bijection is a [homeomorphism](../../../topology.md#homeomorphism). The identifications agree on overlapping charts and glue, proving

$$
\boxed{|X_y|\cong f^{-1}\{y\}\text{ with its subspace topology}.}
$$

The [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) may nevertheless carry nilpotents, so this topological statement does not identify its structure sheaf with a naive restriction of $\mathcal O_X$.

## 3

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [degree-one generation condition for Proj](../../../ringed-space.md#degree-one-generation-condition-for-proj) ensures that the opens $D_+(f)$ for $f\in S_1$ cover $X$. Put $B=S_f$ and $R=B_0$. Multiplication by $f^n$ is an $R$-linear bijection $R\to B_n$ for every integer $n$, because $f$ is an invertible degree-one element. The convention $S(n)_d=S_{n+d}$ therefore identifies $\widetilde{S(n)}$ on this chart with the free rank-one $R$-module $B_n$, generated by $f^n$. Hence **every twisting sheaf $\mathcal O_X(n)$ is invertible**, including negative twists.

For the [tensor product of sheaves](../../../ringed-space.md#tensor-product-of-sheaves), consider the natural map

$$
(M_f)_0\otimes_R(N_f)_0\longrightarrow(M_f\otimes_BN_f)_0.
$$

It is an isomorphism by [degree-one localization of a graded module](../../../commutative-algebra.md#degree-one-localization-of-a-graded-module). Explicitly, a homogeneous tensor $m_a\otimes n_{-a}$ of total degree zero is represented on the left by $f^{-a}m_a\otimes f^a n_{-a}$. Multiplying a tensor factor by a homogeneous element of $B$ gives the same result after using the tensor relation, since that element is a degree-zero coefficient times a power of $f$. This defines the inverse. Since [localization commutes with tensor products](../../../commutative-algebra.md#localization-commutes-with-tensor-products), the target is $((M\otimes_SN)_f)_0$. These natural chart maps agree on overlaps, so

$$
\boxed{\widetilde M\otimes_{\mathcal O_X}\widetilde N\cong\widetilde{M\otimes_SN}.}
$$

The degree-one hypothesis matters: on general [Proj constructions](../../../ringed-space.md#proj-construction), twisting sheaves need not be line bundles. The local trivializations are also recorded in [Stacks Project, Section 27.10](https://stacks.math.columbia.edu/tag/01MM).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Take the [hyperplane divisor](../../../cartier-divisor.md#hyperplane-divisor) $D=(t_0=0)$. On $U_i=D_+(t_i)$ its local equation is $g_i=t_0/t_i$, a non-zero-divisor; on $U_0$ it is the unit one. Thus it is an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor). On overlaps, $g_i/g_j=t_j/t_i$ is a unit.

The [divisor line bundle](../../../cartier-divisor.md#divisor-line-bundle) $\mathcal O_X(D)$ is locally generated by $1/g_i=t_i/t_0$. Map this generator to the local generator $t_i$ of the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) $\mathcal O_X(1)$. On overlaps both generators transform by $t_i/t_j$, so the maps glue and give

$$
\boxed{\mathcal O_X(D)\cong\mathcal O_X(1).}
$$

For $n=0$ the hyperplane is empty and this is the zero Cartier divisor; the conclusion still holds.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

**The first implication is false.** On the [Noetherian scheme](../../../ringed-space.md#noetherian-scheme) $\operatorname{Spec}k[t]$, the [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\longrightarrow\mathcal O_X\xrightarrow{\,t\,}\mathcal O_X\longrightarrow\widetilde{k[t]/(t)}\longrightarrow0
$$

has locally free first and middle terms. The quotient is not [locally free](../../../ringed-space.md#locally-free-sheaf): at $(t)$ it is a nonzero module annihilated by $t$, whereas a free module over the [integral domain](../../../commutative-algebra.md#integral-domain) $k[t]_{(t)}$ has no such element.

**The second implication is true.** Near any point trivialize $\mathcal F$ and $\mathcal H$. Choose a finite local basis of $\mathcal H$. Surjectivity as a sheaf gives local lifts of its basis sections; shrink to the intersection of their finitely many neighbourhoods. The lifts define a splitting $\mathcal H\to\mathcal G$ on that neighbourhood. Thus $\mathcal G\cong\mathcal F\oplus\mathcal H$ there and is [locally free](../../../ringed-space.md#locally-free-sheaf). This is [local splitting when a quotient sheaf is locally free](../../../ringed-space.md#local-splitting-when-a-quotient-sheaf-is-locally-free); no global splitting is asserted.

## 4

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [flasque sheaf](../../../ringed-space.md#flasque-sheaf) has surjective restriction maps $\mathcal F(V)\to\mathcal F(U)$ for every pair of opens $U\subseteq V$. To prove the claim for an [injective sheaf of modules](../../../ringed-space.md#injective-sheaf-of-modules), let $j_U:U\hookrightarrow X$ and $j_V:V\hookrightarrow X$. The natural map

$$
(j_U)_!\mathcal O_U\longrightarrow(j_V)_!\mathcal O_V
$$

is a monomorphism: its [stalks](../../../ringed-space.md#stalk-of-a-sheaf) are either the identity on $\mathcal O_{X,x}$, the map from zero to that stalk, or the zero-to-zero map. Here $j_!$ is [extension by zero](../../../ringed-space.md#extension-by-zero) for module sheaves.

The extension-by-zero adjunction identifies

$$
\operatorname{Hom}_{\mathcal O_X}((j_U)_!\mathcal O_U,I)\cong\Gamma(U,I).
$$

The [injective object](../../../category-theory.md#injective-object) property extends every morphism from $(j_U)_!\mathcal O_U$ to one from $(j_V)_!\mathcal O_V$. Under the displayed identification this is exactly surjectivity of $I(V)\to I(U)$. **Injective module sheaves are therefore flasque.** This argument works on an arbitrary [ringed space](../../../ringed-space.md), without Noetherian or separation assumptions.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For the closed inclusion $f$, the [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) has stalk $\mathcal F_x$ at $x\in X$ and zero stalk at points outside $X$: outside the closed set there is an open neighbourhood disjoint from $X$. Hence $f_*$ is exact, since [exact sequences of sheaves](../../../algebraic-geometry.md#exact-sequence-of-sheaves) are detected on stalks.

Take a [flasque resolution](../../../ringed-space.md#flasque-resolution) $\mathcal F\to\mathcal I^\bullet$. Direct image preserves flasqueness, because restrictions are the restrictions on inverse-image opens. Exactness makes $f_*\mathcal I^\bullet$ a flasque resolution of $f_*\mathcal F$. Moreover

$$
\Gamma(Y,f_*\mathcal I^\bullet)=\Gamma(X,\mathcal I^\bullet).
$$

The complexes computing [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) are identical. Therefore

$$
\boxed{H^i(Y,f_*\mathcal F)\cong H^i(X,\mathcal F)\quad(i\geq0).}
$$

This is [sheaf cohomology under a closed inclusion](../../../ringed-space.md#sheaf-cohomology-under-a-closed-inclusion); the closedness hypothesis is used in the exactness of direct image.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

For a point $x\in X$ and an [abelian group](../../../group.md#abelian-group) $A$, the [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) $i_*A$, with $i:\{x\}\hookrightarrow X$, is

$$
(i_*A)(U)=\begin{cases}A,&x\in U,\\0,&x\notin U.\end{cases}
$$

Restrictions are identities or the map to zero, so it is a [flasque sheaf](../../../ringed-space.md#flasque-sheaf). The global sections equal $A$ and higher cohomology vanishes:

$$
\boxed{H^0(X,i_*A)=A,\qquad H^i(X,i_*A)=0\quad(i>0).}
$$

No closed-point assumption is needed for this calculation of [skyscraper sheaf cohomology](../../../ringed-space.md#skyscraper-sheaf-cohomology). On an arbitrary [topological space](../../../topology.md#topological-space), its nonzero stalks are at points of $\overline{\{x\}}$ when $A\ne0$; only for a closed point is the nonzero stalk confined to $x$.

## 5

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The [direct image of a coherent sheaf under a closed immersion](../../../ringed-space.md#direct-image-of-a-coherent-sheaf-under-a-closed-immersion) puts $\mathcal G=f_*\mathcal F$ in the category of coherent sheaves on $\mathbb P_k^n$. By [sheaf cohomology under a closed inclusion](../../../ringed-space.md#sheaf-cohomology-under-a-closed-inclusion) and the supplied compatibility of twisting with direct image,

$$
H^p(X,\mathcal F(d))\cong H^p(\mathbb P_k^n,\mathcal G(d)).
$$

Here is a proof of the required [Serre vanishing](../../../ringed-space.md#serre-vanishing) on projective space. A [coherent sheaf](../../../ringed-space.md#coherent-sheaf) on $\mathbb P_k^n$ is the [sheaf associated with a graded module](../../../ringed-space.md#sheaf-associated-with-a-graded-module) for a finite graded $k[t_0,\ldots,t_n]$-module. Equivalently, it has a presentation by finite sums of twisting sheaves. Use a [finite twisting resolution of a coherent sheaf on projective space](../../../ringed-space.md#finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space): resolve the graded module by a finite graded [free resolution](../../../algebra.md#free-resolution), using the [Hilbert syzygy theorem](../../../algebra.md#hilbert-s-syzygy-theorem), and sheafify; [exactness of localization](../../../commutative-algebra.md#exactness-of-localization) preserves the resolution. Its terms are finite sums of $\mathcal O(a)$.

Choose $d$ sufficiently large that all twists $a+d$ occurring in these finitely many terms are nonnegative. The [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) then vanishes in every positive degree for every resolution term. In a short exact sequence $0\to\mathcal K_{j+1}\to\mathcal E_j\to\mathcal K_j\to0$, with $\mathcal K_0=\mathcal G$, the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) identifies $H^p(\mathcal K_j(d))$ with $H^{p+1}(\mathcal K_{j+1}(d))$ for $p>0$. Iterating to the final acyclic term proves

$$
\boxed{H^p(X,\mathcal F(d))=0\quad(p>0,\ d\gg0).}
$$

The standard graded-module description used here is given in [Stacks Project, Section 30.15](https://stacks.math.columbia.edu/tag/0BXE); the vanishing follows from the displayed finite-resolution argument.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Choose the rational point $x=[1:0:\cdots:0]$ and the [coherent sheaf](../../../ringed-space.md#coherent-sheaf) $\mathcal F=i_*k$ supported there. By [skyscraper sheaf cohomology](../../../ringed-space.md#skyscraper-sheaf-cohomology), $H^0(X,\mathcal F)=k$.

Its [dual of a sheaf](../../../ringed-space.md#dual-of-a-sheaf) $\mathcal F^\vee=\mathcal H om(\mathcal F,\mathcal O_X)$ is zero. Away from $x$ its source is zero. At $x$, a homomorphism $k\to\mathcal O_{X,x}$ must send one to an element annihilated by the maximal ideal. Since $n>0$, that ideal contains a nonzero coordinate parameter; the local ring is an [integral domain](../../../commutative-algebra.md#integral-domain), so the image must vanish. This proves that every local homomorphism vanishes. Consequently

$$
\boxed{\dim_kH^0(X,\mathcal F)=1,\qquad\dim_kH^n(X,\mathcal F^\vee(-n-1))=0.}
$$

There is no contradiction with [Serre duality](../../../ringed-space.md#serre-duality): the ordinary sheaf dual suffices for locally free sheaves, but general coherent sheaves require an [Ext functor](../../../algebra.md#ext-functor). This example illustrates [failure of ordinary sheaf-dual Serre duality for a skyscraper sheaf](../../../ringed-space.md#failure-of-ordinary-sheaf-dual-serre-duality-for-a-skyscraper-sheaf).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Eliminate $t_3$ using the linear equation. The homogeneous coordinate ring becomes

$$
B=\mathbb C[t_0,t_1,t_2]/(t_1^3+t_0t_2^2).
$$

The cubic is a nonzero element of a polynomial [integral domain](../../../commutative-algebra.md#integral-domain), hence a non-zero-divisor. It gives the exact sequence of [graded modules](../../../commutative-algebra.md#graded-module)

$$
0\longrightarrow S(-3)\xrightarrow{\,t_1^3+t_0t_2^2\,}S\longrightarrow B\longrightarrow0,
\qquad S=\mathbb C[t_0,t_1,t_2].
$$

Thus $\dim B_m=\binom{m+2}{2}-\binom{m-1}{2}$ for $m\ge3$. Equivalently, use the [Hilbert series](../../../commutative-algebra.md#hilbert-series) $(1-z^3)/(1-z)^3$, or the sheafified exact sequence on $\mathbb P^2$. The [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial) of the [plane cubic](../../../algebraic-geometry.md#plane-cubic) is

$$
\boxed{\Phi_{\mathcal O_X}(m)=3m.}
$$

Its degree is three and its [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) is one, although the curve is singular: its affine equation near $[1:0:0]$ is the cusp $t_2^2+t_1^3=0$. The Hilbert polynomial records the arithmetic genus, rather than the genus of the normalization.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
