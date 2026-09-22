# Paper 16

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_16.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_16.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Construct the [tensor product of sheaves](../../../ringed-space.md#tensor-product-of-sheaves) by first forming the [presheaf](../../../algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) $U\mapsto\mathcal F(U)\otimes_{\mathcal O_X(U)}\mathcal G(U)$, with restriction maps induced by those of the two [sheaves of modules](../../../ringed-space.md#sheaf-of-modules), and then applying [sheafification](../../../ringed-space.md#sheafification). The local [module](../../../module-theory.md#module-mathematics) actions are compatible with restrictions and therefore give the sheaf an $\mathcal O_X$-module structure. Its [stalks](../../../ringed-space.md#stalk-of-a-sheaf) are

$$
(\mathcal F\otimes_{\mathcal O_X}\mathcal G)_x\cong\mathcal F_x\otimes_{\mathcal O_{X,x}}\mathcal G_x.
$$

Indeed, a finite collection of [germs of sheaf sections](../../../ringed-space.md#germ-of-a-sheaf-section) can be represented on a common neighbourhood, and every finite tensor relation holds on a sufficiently small neighbourhood. Equivalently, this construction represents [bilinear maps](../../../linear-algebra.md#bilinear-map) of [sheaves of modules](../../../ringed-space.md#sheaf-of-modules) that are balanced over the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme). Sections of the resulting sheaf need not themselves be tensors of [global sections](../../../ringed-space.md#global-section): that is why the [sheafification](../../../ringed-space.md#sheafification) step matters.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) is defined on an [open set](../../../topology.md#open-set) $V\subseteq Y$ by

$$
(\phi_*\mathcal F)(V)=\mathcal F(\phi^{-1}V).
$$

Restrictions are those of $\mathcal F$, and the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) follows by taking inverse images of an [open cover](../../../topology.md#open-cover). The [morphism of ringed spaces](../../../ringed-space.md#morphism-of-ringed-spaces) supplies $\phi^\#: \mathcal O_Y\to\phi_*\mathcal O_X$. Thus $a\in\mathcal O_Y(V)$ acts on $s\in\mathcal F(\phi^{-1}V)$ by $\phi^\#(a)s$, making $\phi_*\mathcal F$ a [sheaf of modules](../../../ringed-space.md#sheaf-of-modules) over $\mathcal O_Y$. This definition uses no [quasi-coherence](../../../ringed-space.md#quasi-coherent-sheaf).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

First form the [inverse image sheaf](../../../ringed-space.md#inverse-image-sheaf) $\phi^{-1}\mathcal H$ by applying [sheafification](../../../ringed-space.md#sheafification) to

$$
U\longmapsto\varinjlim_{V\supseteq\phi(U)}\mathcal H(V).
$$

It is a [sheaf of modules](../../../ringed-space.md#sheaf-of-modules) over $\phi^{-1}\mathcal O_Y$. The [morphism of ringed spaces](../../../ringed-space.md#morphism-of-ringed-spaces) gives a ring map $\phi^{-1}\mathcal O_Y\to\mathcal O_X$, so the [pullback of a sheaf of modules](../../../ringed-space.md#pullback-of-a-sheaf-of-modules) is

$$
\boxed{\phi^*\mathcal H=\mathcal O_X\otimes_{\phi^{-1}\mathcal O_Y}\phi^{-1}\mathcal H.}
$$

At $x\in X$, writing $y=\phi(x)$, its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) is $\mathcal O_{X,x}\otimes_{\mathcal O_{Y,y}}\mathcal H_y$. The tensor construction makes the action of the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme) explicit; taking the inverse image alone would not give the requested $\mathcal O_X$-module.

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The opening [change-of-rings tensor quotient](../../../module-theory.md#change-of-rings-tensor-quotient) sends $m\otimes_Rn$ to $m\otimes_An$. The target pairing is [bilinear](../../../linear-algebra.md#bilinear-map) and $R$-balanced because $\theta(r)m\otimes_An=m\otimes_A\theta(r)n$. On the source, let $A$ act through the first factor; commutativity makes that action compatible with the $R$-balancing relations, and the map is $A$-linear. It is [surjective](../../../algebra.md#surjective-function): the target is the quotient imposing the additional relations $am\otimes_Rn=m\otimes_Ran$ for every $a\in A$. The construction commutes with [module homomorphisms](../../../module-theory.md#module-homomorphism) in both variables.

The [pullback-direct-image adjunction unit](../../../ringed-space.md#pullback-direct-image-adjunction-unit) is obtained locally by pulling a section $h\in\mathcal H(V)$ to $\phi^{-1}V$ and sending it to $1\otimes h$ in $\phi^*\mathcal H(\phi^{-1}V)$. These maps respect restrictions and the $\mathcal O_Y$-actions, hence define

$$
\eta_{\mathcal H}:\mathcal H\longrightarrow\phi_*\phi^*\mathcal H.
$$

For $\mathcal H=\mathcal O_Y$, multiplication identifies $\phi^*\mathcal O_Y$ with $\mathcal O_X$, and $\eta_{\mathcal O_Y}$ is precisely the structure morphism $\phi^\#: \mathcal O_Y\to\phi_*\mathcal O_X$.

To construct the [direct-image tensor comparison](../../../ringed-space.md#direct-image-tensor-comparison), on $V\subseteq Y$ send $s\otimes t$, with $s\in\mathcal F(\phi^{-1}V)$ and $t\in\mathcal G(\phi^{-1}V)$, to its tensor section of $\mathcal F\otimes_{\mathcal O_X}\mathcal G$. This pairing is $\mathcal O_Y(V)$-balanced through $\phi^\#$ and is compatible with restrictions. The [universal property of the tensor product of modules](../../../module-theory.md#universal-property-of-the-tensor-product-of-modules) and [sheafification](../../../ringed-space.md#sheafification) therefore give

$$
\phi_*\mathcal F\otimes_{\mathcal O_Y}\phi_*\mathcal G\longrightarrow\phi_*(\mathcal F\otimes_{\mathcal O_X}\mathcal G).
$$

Apply this with $\mathcal G=\phi^*\mathcal H$ after tensoring the unit $\eta_{\mathcal H}$ with $\phi_*\mathcal F$. The composite is the map in the [projection formula for sheaves](../../../ringed-space.md#projection-formula). If $\mathcal H|_V\cong\mathcal O_V^r$, then $\phi^*\mathcal H|_{\phi^{-1}V}\cong\mathcal O_{\phi^{-1}V}^r$, and the composite identifies with

$$
(\phi_*\mathcal F|_V)^{\oplus r}\longrightarrow\phi_*(\mathcal F^{\oplus r})|_V,
$$

the identity on the $r$ components. Thus it is an [isomorphism](../../../algebra.md#isomorphism) for a [locally free sheaf](../../../ringed-space.md#locally-free-sheaf) of finite rank. Neither $\mathcal F$ nor $\mathcal G$ was assumed [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf).

## 2

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $r=1$, the assertion is the assumed vanishing for [coherent ideal sheaves](../../../ringed-space.md#coherent-ideal-sheaf). For $r>1$, project $\mathcal F\subseteq\mathcal O_X^r$ onto the last component. Its image $\mathcal I\subseteq\mathcal O_X$ is a [coherent ideal sheaf](../../../ringed-space.md#coherent-ideal-sheaf), and its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $\mathcal F'$ is a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) contained in $\mathcal O_X^{r-1}$. Here images and kernels are coherent because a [variety](../../../algebraic-geometry.md#algebraic-variety) is [Noetherian](../../../algebra.md#noetherian-ring). The [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow\mathcal F'\longrightarrow\mathcal F\longrightarrow\mathcal I\longrightarrow0
$$

gives an exact segment $H^1(X,\mathcal F')\to H^1(X,\mathcal F)\to H^1(X,\mathcal I)$ in the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology). The outer terms vanish by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) and the hypothesis, so the middle term vanishes. This is [ideal-sheaf vanishing for a coherent submodule of a trivial bundle](../../../ringed-space.md#ideal-sheaf-vanishing-for-a-coherent-submodule-of-a-trivial-bundle).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\mathcal I_Y$ be the [coherent ideal sheaf](../../../ringed-space.md#coherent-ideal-sheaf) of $Y$, and let $\mathfrak m_P$ be the [ideal sheaf of a closed point](../../../ringed-space.md#ideal-sheaf-of-a-closed-point). Because $P\notin Y$, the [stalk](../../../ringed-space.md#stalk-of-a-sheaf) $(\mathcal I_Y)_P$ is $\mathcal O_{X,P}$. Evaluation at $P$ therefore gives a [surjective morphism of sheaves](../../../algebraic-geometry.md#surjective-morphism-of-sheaves) $\mathcal I_Y\to k_P$ to the [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) at $P$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $\mathcal J=\mathcal I_Y\cap\mathfrak m_P$ is again a [coherent ideal sheaf](../../../ringed-space.md#coherent-ideal-sheaf). From

$$
0\to\mathcal J\to\mathcal I_Y\to k_P\to0
$$

and $H^1(X,\mathcal J)=0$, the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) shows that $\Gamma(X,\mathcal I_Y)\to k$ is onto. Choose $f$ mapping to $1$. It vanishes on $Y$ and satisfies $f(P)=1$. Hence $X_f\subseteq U$, and inside the [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) $U$ it is the [principal open subset](../../../ringed-space.md#principal-open-subscheme) defined by $f|_U$. A principal open of an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) is affine. This gives [affine principal neighbourhoods from ideal-sheaf vanishing](../../../ringed-space.md#affine-principal-neighbourhoods-from-ideal-sheaf-vanishing).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [quasi-compactness](../../../topology.md#compact-space) of $X$ gives a finite cover by the affine principal neighbourhoods constructed above. Because at every point some $f_i$ is a unit in the [local ring](../../../commutative-algebra.md#local-ring), the map of [coherent sheaves](../../../ringed-space.md#coherent-sheaf)

$$
\mathcal O_X^r\longrightarrow\mathcal O_X,\qquad(h_i)\longmapsto\sum_i f_ih_i
$$

is [surjective](../../../algebra.md#surjective-function). Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $\mathcal F$ is a coherent submodule of the trivial bundle, so $H^1(X,\mathcal F)=0$ by part (a). The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) makes the map on [global sections](../../../ringed-space.md#global-section) surjective. Lifting $1$ supplies

$$
\boxed{\sum_{i=1}^r g_if_i=1,\qquad g_i\in A.}
$$

This is the [unit-ideal certificate from a principal affine cover](../../../ringed-space.md#unit-ideal-certificate-from-a-principal-affine-cover).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [localization of global sections on a principal open](../../../ringed-space.md#localization-of-global-sections-on-a-principal-open) gives $A_{f_i}=\Gamma(X_{f_i},\mathcal O_X)$. Each of these rings is a [finitely generated algebra](../../../algebra.md#finitely-generated-algebra) because $X_{f_i}$ is an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set). Choose finite generators of every $A_{f_i}$ and write them as $a_{ij}/f_i^{e_{ij}}$ with $a_{ij}\in A$. Let $B$ be the $k$-subalgebra of $A$ generated by all $f_i,g_i,a_{ij}$. It is a [finitely generated algebra](../../../algebra.md#finitely-generated-algebra), and $B_{f_i}=A_{f_i}$ since these localizations contain the chosen generators and $f_i^{-1}$.

For any integer $N\geq1$, raise $\sum_i g_if_i=1$ to the power $r(N-1)+1$. Every resulting monomial contains some $f_i^N$, so it gives a [unit-ideal identity for powers](../../../commutative-algebra.md#unit-ideal-identity-for-powers)

$$
1=\sum_i c_if_i^N,\qquad c_i\in B.
$$

For an arbitrary $a\in A$, equality $A_{f_i}=B_{f_i}$ implies $f_i^{N_i}a\in B$ for some $N_i$: multiply by an additional power if equality of localized fractions requires it. Choose a common $N$ and the identity above. Then $a=\sum_i c_i(f_i^Na)\in B$. Consequently $A=B$, so $A$ is a [finitely generated algebra](../../../algebra.md#finitely-generated-algebra). It is a [reduced ring](../../../commutative-algebra.md#reduced-ring), since a [nilpotent element](../../../commutative-algebra.md#nilpotent) global [regular function](../../../ringed-space.md#regular-function) has zero germ everywhere on the reduced [variety](../../../algebraic-geometry.md#algebraic-variety) $X$. This is [finite generation from finitely many principal localizations](../../../algebra.md#finite-generation-from-finitely-many-principal-localizations).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Let $Y$ be the [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) with [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $A$. Its principal opens $D(f_i)$ cover $Y$ because $\sum_i g_if_i=1$. On $X_{f_i}$, the [localization of global sections on a principal open](../../../ringed-space.md#localization-of-global-sections-on-a-principal-open) identifies its [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) with $A_{f_i}$, giving an [isomorphism](../../../algebra.md#isomorphism)

$$
\phi_i:X_{f_i}\xrightarrow{\sim}D(f_i)\subseteq Y.
$$

On an overlap the two maps are induced by the same elements of $A$, or equivalently by the same identification with $A_{f_if_j}$, so they agree. Glue them to $\phi:X\to Y$. The inverses agree on the overlaps as well and glue to its inverse. At a [closed point](../../../topology.md#closed-point) $P$, this is the map corresponding to the evaluation [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) $A\to k$, $a\mapsto a(P)$. This proves the [cohomological criterion for affineness](../../../ringed-space.md#cohomological-criterion-for-affineness) by an explicit global [isomorphism](../../../algebra.md#isomorphism).

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), every [coherent ideal sheaf](../../../ringed-space.md#coherent-ideal-sheaf) is [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf); [vanishing of quasi-coherent cohomology on an affine scheme](../../../ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme) therefore gives $H^1(X,\mathcal I)=0$.

For the projective-space complement, assume $n\geq1$ and choose two distinct [closed points](../../../topology.md#closed-point) $P,Q\in X$. Take the [ideal sheaf of two closed points](../../../ringed-space.md#ideal-sheaf-of-two-closed-points) $\mathcal I=\mathfrak m_P\cap\mathfrak m_Q$ on $X$. The [codimension-two extension of regular functions on a normal variety](../../../ringed-space.md#codimension-two-extension-of-regular-functions-on-a-normal-variety) gives

$$
\Gamma(X,\mathcal O_X)=\Gamma(\mathbb P^n,\mathcal O_{\mathbb P^n})=k.
$$

One can see this directly: on every standard [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) of $\mathbb P^n$, a [rational function](../../../isolated-singularity.md#rational-function) written in lowest terms cannot have a nonconstant denominator, because an [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) factor of the denominator would define a pole along a codimension-one [hypersurface](../../../differential-geometry.md#hypersurface), and such a hypersurface is not removed by $Z$. The extended function is constant because every global [regular function](../../../ringed-space.md#regular-function) on [projective space](../../../projective-space.md) is constant. Now the [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\to\mathcal I\to\mathcal O_X\to k_P\oplus k_Q\to0
$$

sends $k$ diagonally into $k^2$ on [global sections](../../../ringed-space.md#global-section). Its [cokernel](../../../linear-algebra.md#cokernel) is $k$, and the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) injects that [cokernel](../../../linear-algebra.md#cokernel) into $H^1(X,\mathcal I)$. Thus

$$
\boxed{H^1(X,\mathcal I)\ne0.}
$$

The assumption $n\geq1$ is necessary: $\mathbb P^0$ is already affine and has no such example.

## 3

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $U_{i_0\dots i_q}=U_{i_0}\cap\cdots\cap U_{i_q}$, the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) has groups

$$
C^q(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0\dots i_q}),\qquad
(\delta c)_{i_0\dots i_{q+1}}=\sum_{j=0}^{q+1}(-1)^j c_{i_0\dots\widehat{i_j}\dots i_{q+1}}|_{U_{i_0\dots i_{q+1}}}.
$$

Terms in $\delta^2$ cancel in pairs, and [Čech cohomology](../../../ringed-space.md#cech-cohomology) is $\ker\delta/\operatorname{im}\delta$. A degree-zero [cocycle](../../../algebra.md#cocycle) is exactly a family of compatible local sections. The [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) gives their unique [global section](../../../ringed-space.md#global-section), proving $\check H^0(\mathcal U,\mathcal F)\cong\mathcal F(X)$. If the cover has affine finite intersections, a [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf) has no higher [cohomology](../../../cohomology.md) on those intersections by [vanishing of quasi-coherent cohomology on an affine scheme](../../../ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme). The [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem) then identifies all Čech groups with [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology). In particular, a finite affine [open cover](../../../topology.md#open-cover) of a [separated variety](../../../ringed-space.md#separated-variety) has this property.

For the [sheaf of units of the structure sheaf](../../../ringed-space.md#sheaf-of-units-of-the-structure-sheaf), a multiplicative degree-one [cocycle](../../../algebra.md#cocycle) is a family $g_{ij}\in\mathcal O_X^*(U_i\cap U_j)$ satisfying $g_{ij}g_{jk}=g_{ik}$, with $g_{ji}=g_{ij}^{-1}$. It glues trivial rank-one [free modules](../../../module-theory.md#free-module) into an [invertible sheaf](../../../ringed-space.md#line-bundle). Changing the local frames multiplies $g_{ij}$ by a [coboundary](../../../algebra.md#coboundary), and two sets of transition data give isomorphic [line bundles](../../../ringed-space.md#line-bundle) precisely when their [cocycles](../../../algebra.md#cocycle) differ this way. Tensoring [line bundles](../../../ringed-space.md#line-bundle) multiplies their [cocycles](../../../algebra.md#cocycle). Thus [line bundles trivialized by an open cover](../../../ringed-space.md#line-bundles-trivialized-by-an-open-cover) give the group [isomorphism](../../../algebra.md#isomorphism)

$$
\operatorname{Pic}(X)_{\mathcal U}\cong\check H^1(\mathcal U,\mathcal O_X^*).
$$

For the remaining arguments, work over the algebraically closed ground field. On the [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) $V$, put $\mathcal Q=\mathcal K^*/\mathcal O_V^*$, a quotient of [sheaves of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups). A [global section](../../../ringed-space.md#global-section) of $\mathcal Q$ is locally represented by [rational functions](../../../isolated-singularity.md#rational-function) $f_i$ whose ratios are regular units. The corresponding unit [cocycle](../../../algebra.md#cocycle) $f_j/f_i$ defines an [invertible sheaf](../../../ringed-space.md#line-bundle). A single global [rational function](../../../isolated-singularity.md#rational-function) has trivial [cocycle](../../../algebra.md#cocycle). Conversely, every [line bundle](../../../ringed-space.md#line-bundle) has a nonzero rational section: choose a nonzero vector in its one-dimensional fibre at the [generic point](../../../algebraic-geometry.md#generic-point) and express it in local frames. This supplies such local $f_i$. If the associated [line bundle](../../../ringed-space.md#line-bundle) is trivial, changing frames makes all $f_i$ restrictions of one [rational function](../../../isolated-singularity.md#rational-function). Therefore

$$
 k(V)^*\longrightarrow\Gamma(V,\mathcal K^*/\mathcal O_V^*)\longrightarrow\operatorname{Pic}(V)\longrightarrow0
$$

is exact. This is the [Cartier-divisor description of the Picard group](../../../ringed-space.md#cartier-divisor-description-of-the-picard-group). The [sheaf of nonzero rational functions on an irreducible variety](../../../algebraic-geometry.md#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety) is [flasque](../../../ringed-space.md#flasque-sheaf), since all restrictions between nonempty [open sets](../../../topology.md#open-set) are the identity on $k(V)^*$. Apply the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) to $1\to\mathcal O_V^*\to\mathcal K^*\to\mathcal Q\to1$. Since $H^1(V,\mathcal K^*)=0$, its connecting map has exactly the [cokernel](../../../linear-algebra.md#cokernel) just computed, proving

$$
\boxed{\operatorname{Pic}(V)\cong H^1(V,\mathcal O_V^*).}
$$

Finally the [Segre description of a smooth quadric surface](../../../projective-space.md#segre-description-of-a-smooth-quadric-surface) identifies $V$ with $\mathbb P^1\times\mathbb P^1$. The two [rulings of a smooth quadric surface](../../../projective-space.md#rulings-of-a-smooth-quadric-surface) have classes $F_1,F_2$ generating $\operatorname{Pic}(V)\cong\mathbb Z^2$. For completeness, remove one line in each ruling: the remaining chart is the [affine plane](../../../ringed-space.md#affine-plane), with factorial [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $k[s,t]$ and trivial [divisor class group](../../../algebraic-geometry.md#divisor-class-group). The [localization sequence for the divisor class group](../../../algebraic-geometry.md#localization-sequence-for-the-divisor-class-group) makes $F_1,F_2$ generators, and their degrees on the two ruling lines prove independence. The hyperplane class, and hence the conic $C$, has bidegree $(1,1)$. By [Picard-group localization on a smooth variety](../../../ringed-space.md#picard-group-localization-on-a-smooth-variety), the [Picard group of a smooth affine quadric surface](../../../projective-space.md#picard-group-of-a-smooth-affine-quadric-surface) is

$$
\boxed{\operatorname{Pic}(U)\cong\mathbb Z^2/\mathbb Z(1,1)\cong\mathbb Z.}
$$

Explicitly, the restriction of $\mathcal O_V(1,0)$ is nontrivial: if it were trivial on $U$, its rational trivialization would have divisor supported on $C$, forcing $(1,0)$ to be an integer multiple of $(1,1)$, which is impossible.

## 4

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

On an [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) $\operatorname{Spec}A\subseteq V$, the [module of Kähler differentials](../../../ringed-space.md#kahler-differential) $\Omega_{A/k}$ is generated by symbols $da$ subject to $k$-linearity and $d(ab)=a\,db+b\,da$. It represents $k$-[derivations](../../../associative-algebra.md#derivation-of-an-algebra). These [modules](../../../module-theory.md#module-mathematics) commute with [localization](../../../commutative-algebra.md#localization-of-a-ring), so their associated [quasi-coherent sheaves](../../../ringed-space.md#quasi-coherent-sheaf) glue to the [Kähler differential sheaf](../../../ringed-space.md#sheaf-of-kahler-differentials-over-a-field) $\Omega^1_{V/k}$. It is coherent: if $A=k[x_1,\dots,x_N]/I$ and $I=(f_1,\dots,f_s)$, then it has the [finite presentation of a module](../../../module-theory.md#finite-presentation-of-a-module)

$$
A^s\xrightarrow{(\partial f_j/\partial x_i)}A^N\longrightarrow\Omega_{A/k}\longrightarrow0.
$$

For a [closed point](../../../topology.md#closed-point) $P$, put $R=\mathcal O_{V,P}$ with [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $\mathfrak m$ and residue field $k$. The [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space) is $\operatorname{Hom}_k(\mathfrak m/\mathfrak m^2,k)$, equivalently $\operatorname{Der}_k(R,k)$. A derivation kills constants and $\mathfrak m^2$, so it factors through $a\mapsto a-a(P)$; conversely every [linear functional](../../../linear-algebra.md#linear-functional) on $\mathfrak m/\mathfrak m^2$ defines such a derivation by the product rule. The [universal property of Kähler differentials](../../../ringed-space.md#universal-property-of-kahler-differentials) therefore identifies this space with

$$
\boxed{T_{V,P}=\operatorname{Hom}_k(\Omega^1_{V,P}/\mathfrak m_P\Omega^1_{V,P},k).}
$$

In particular, $\Omega^1_{V,P}/\mathfrak m_P\Omega^1_{V,P}\cong\mathfrak m_P/\mathfrak m_P^2$, the [algebraic cotangent space](../../../algebraic-geometry.md#algebraic-cotangent-space).

A point is a [smooth point of a variety](../../../algebraic-geometry.md#smooth-point-of-a-variety) when its [local ring](../../../commutative-algebra.md#local-ring) is a [regular local ring](../../../commutative-algebra.md#regular-local-ring); over this algebraically closed field this says $\dim_kT_{V,P}=n=\dim V$. Tensor the [finite presentation of a module](../../../module-theory.md#finite-presentation-of-a-module) above with $k(P)$. The tangent space is the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of the [Jacobian matrix](../../../calculus.md#jacobian-matrix) $J(P)$, hence has dimension $N-\operatorname{rank}J(P)$. This proves the [Jacobian criterion](../../../algebraic-geometry.md#jacobian-criterion)

$$
\boxed{P\text{ smooth}\iff\operatorname{rank}J(P)=N-n.}
$$

For a smooth [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) $V$, choose at each point an invertible $(N-n)$-minor and shrink the [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) so that it remains invertible. Its relations eliminate $N-n$ of the generators of $\Omega_{A/k}$, yielding a surjection $A^n\to\Omega_{A/k}$. At the [generic point](../../../algebraic-geometry.md#generic-point), its target has dimension $n$: over a perfect ground field, a separating transcendence basis of the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) has differentials forming a basis. Equivalently this follows from the assumed [density of the smooth locus](../../../algebraic-geometry.md#density-of-the-smooth-locus). The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) therefore becomes zero over the [fraction field](../../../commutative-algebra.md#field-of-fractions) of the [integral domain](../../../commutative-algebra.md#integral-domain) $A$. As a submodule of $A^n$, it is a [torsion-free module](../../../module-theory.md#torsion-free-module), so it is already zero. Thus these maps give local [isomorphisms](../../../algebra.md#isomorphism) with $\mathcal O_V^n$, proving [local freeness of differentials on a smooth variety](../../../ringed-space.md#local-freeness-of-differentials-on-a-smooth-variety) with rank $n$.

For an [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) $\operatorname{Spec}A\subseteq V$, write $W\cap\operatorname{Spec}A=\operatorname{Spec}(A/I)$ and $\mathcal M=\widetilde M$. The [restriction of a module sheaf to a closed subvariety](../../../ringed-space.md#restriction-of-a-module-sheaf-to-a-closed-subvariety) is $\widetilde{M\otimes_AA/I}=\widetilde{M/IM}$. The [Conormal exact sequence for Kähler differentials](../../../ringed-space.md#conormal-exact-sequence-for-kahler-differentials) is

$$
I/I^2\xrightarrow{\bar f\mapsto df\otimes1}\Omega_{A/k}\otimes_AA/I\longrightarrow\Omega_{(A/I)/k}\longrightarrow0.
$$

It follows from the generators and relations: passing to $A/I$ imposes precisely the additional relations $df=0$ for $f\in I$. The first map is well defined because $d(I^2)$ lies in $I\Omega_{A/k}$. Glue these exact [module](../../../module-theory.md#module-mathematics) sequences, using [exactness of localization](../../../commutative-algebra.md#exactness-of-localization), to obtain

$$
\mathcal I_W/\mathcal I_W^2\longrightarrow\Omega_V^1|_W\longrightarrow\Omega_W^1\longrightarrow0.
$$

In the final assertion, interpret [locally principal subvariety](../../../cartier-divisor.md#locally-principal-subvariety) as a proper local hypersurface. Its ideal on each chart is $(f)$ with $f\ne0$. Since $V$ is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) and reduced, $f$ is a [non-zero-divisor](../../../mathematics.md#non-zero-divisor), and $A/(f)\to(f)/(f^2)$, $\bar a\mapsto af$, is an [isomorphism](../../../algebra.md#isomorphism). These local rank-one descriptions make the [conormal sheaf](../../../ringed-space.md#conormal-sheaf) $\mathcal I_W/\mathcal I_W^2$ invertible.

Because $W$ is not contained in the singular locus of $V$, there is a dense open subset of $W$ where both $V$ and $W$ are [smooth varieties](../../../algebraic-geometry.md#smooth-algebraic-variety). At a [closed point](../../../topology.md#closed-point) there, $\dim W=\dim V-1$ by the [Krull principal ideal theorem](../../../commutative-algebra.md#krull-principal-ideal-theorem). The tangent description $T_{W,P}=\ker(df:T_{V,P}\to k)$ then forces $df\ne0$. Hence the conormal map is injective at the [generic point](../../../algebraic-geometry.md#generic-point) of $W$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is a subsheaf of a [line bundle](../../../ringed-space.md#line-bundle) on the integral [variety](../../../algebraic-geometry.md#algebraic-variety) $W$, so it is a [torsion-free sheaf](../../../ringed-space.md#torsion-free-sheaf); a [torsion-free sheaf](../../../ringed-space.md#torsion-free-sheaf) with zero generic fibre is zero. This proves [conormal injectivity for a generically smooth Cartier divisor](../../../ringed-space.md#conormal-injectivity-for-a-generically-smooth-cartier-divisor). If zero equations were allowed in the phrase locally principal, $W=V$ would be a counterexample to invertibility; the proper-hypersurface convention is essential.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
