# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper14.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $V\subseteq U$ be open subsets, and let $s\in\mathcal F_3(V)$. The assumed [flasque-kernel section-lifting lemma](../../../ringed-space.md#flasque-kernel-section-lifting-lemma) lifts $s$ to $\widetilde s\in\mathcal F_2(V)$. Since $\mathcal F_2$ is a [flabby sheaf](../../../ringed-space.md#flasque-sheaf), extend $\widetilde s$ to a section on $U$, then project to $\mathcal F_3(U)$. Its restriction is $s$. Thus every restriction map of $\mathcal F_3$ is [surjective](../../../algebra.md#surjective-function), proving that **the quotient of two [flabby sheaves](../../../ringed-space.md#flasque-sheaf) in a short exact sequence is flabby**.

For the construction of [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology), embed a [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups) $\mathcal F$ into the [sheaf](../../../algebraic-geometry.md#sheaf-mathematics)

$$
C(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P
$$

by sending a section to all its [germs](../../../ringed-space.md#germ-of-a-sheaf-section). This is [injective](../../../algebra.md#injective-function) because a section with every germ zero is zero. Arbitrary families of stalk elements glue point by point, and restriction maps are projections; hence $C(\mathcal F)$ is a [flabby sheaf](../../../ringed-space.md#flasque-sheaf). Set $\mathcal Q^0=\mathcal F$, $\mathcal I^j=C(\mathcal Q^j)$ and $\mathcal Q^{j+1}=\mathcal I^j/\mathcal Q^j$. Compose the quotient map with the next embedding to obtain the [flasque resolution](../../../ringed-space.md#flasque-resolution)

$$
0\longrightarrow\mathcal F\longrightarrow\mathcal I^0
\longrightarrow\mathcal I^1\longrightarrow\cdots.
$$

The [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) groups are the [cohomology groups](../../../cohomology.md#cohomology-group) of the resulting [cochain complex](../../../algebra.md#cochain-complex) of [global sections](../../../ringed-space.md#global-section):

$$
H^j(X,\mathcal F)=
\frac{\ker\bigl(\Gamma(X,\mathcal I^j)\to\Gamma(X,\mathcal I^{j+1})\bigr)}
{\operatorname{im}\bigl(\Gamma(X,\mathcal I^{j-1})\to\Gamma(X,\mathcal I^j)\bigr)}
\quad(j>0),
\qquad H^0(X,\mathcal F)=\Gamma(X,\mathcal F).
$$

The usual comparison of resolutions identifies this construction with the right derived functors of [global sections](../../../ringed-space.md#global-section); the construction above is the [Godement resolution](../../../ringed-space.md#godement-resolution).

If $\mathcal F$ is itself a [flabby sheaf](../../../ringed-space.md#flasque-sheaf), the quotient argument shows inductively that every $\mathcal Q^j$ is flabby. The assumed lifting result therefore makes

$$
0\to\Gamma(X,\mathcal Q^j)\to\Gamma(X,\mathcal I^j)
\to\Gamma(X,\mathcal Q^{j+1})\to0
$$

an [exact sequence](../../../homology.md#exact-sequence) for every $j$. The global-section complex is consequently exact in every positive degree. In particular,

$$
\boxed{H^j(X,\mathcal F)=0\quad(j>0)\qquad\text{if }\mathcal F\text{ is flabby}.}
$$

This establishes the vanishing from the section-lifting property rather than assuming it in advance.

For the [smooth algebraic curve](../../../algebraic-geometry.md#smooth-algebraic-curve) $X$, a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) is a finite formal sum $D=\sum_P n_PP$ of closed points with integer coefficients. At each closed point, the [local ring of a smooth algebraic curve](../../../projective-space.md#local-ring-of-a-smooth-algebraic-curve) is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring); write its normalized [discrete valuation](../../../commutative-algebra.md#discrete-valuation) as $v_P$. For $f\in k(X)^*$ the [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) is $\operatorname{div}(f)=\sum_Pv_P(f)P$. Only finitely many coefficients are nonzero: zeros and poles are proper closed subsets in the [Noetherian Zariski topology](../../../algebraic-geometry.md#noetherian-zariski-topology) of a curve. The [divisor class group](../../../algebraic-geometry.md#divisor-class-group) is the [abelian group](../../../group.md#abelian-group)

$$
\boxed{\operatorname{Cl}(X)=
\operatorname{Div}(X)/\{\operatorname{div}(f):f\in k(X)^*\}.}
$$

Equivalently, its elements are [divisors on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) modulo [linear equivalence of divisors](../../../algebraic-geometry.md#linear-equivalence-of-divisors).

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $\mathcal D=\mathcal K_X^*/\mathcal O_X^*$, the quotient [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups). At a closed point $P$, the [discrete valuation](../../../commutative-algebra.md#discrete-valuation) gives an [isomorphism](../../../algebra.md#isomorphism)

$$
\mathcal D_P=k(X)^*/\mathcal O_{X,P}^*
\xrightarrow{\;\sim\;}\mathbb Z,\qquad [f]\longmapsto v_P(f).
$$

Indeed, a [local parameter on a smooth algebraic curve](../../../projective-space.md#local-parameter-on-a-smooth-algebraic-curve) has valuation one, and the valuation kernel is precisely the [unit group](../../../algebra.md#unit-group) of the [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring). Thus a local section represented by $f$ determines its local [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve), and changing $f$ by a [regular function](../../../ringed-space.md#regular-function) which is a unit does not change those coefficients.

These local valuations identify $\Gamma(X,\mathcal D)$ with $\operatorname{Div}(X)$. To see that they give finite support, represent a section locally by finitely many [rational functions on an algebraic variety](../../../algebraic-geometry.md#rational-function-on-an-algebraic-variety), using [Noetherian Zariski topology](../../../algebraic-geometry.md#noetherian-zariski-topology) to take a finite cover. Each representative has only finitely many zeros and poles, so their combined support is finite. Conversely, for $D=\sum n_PP$, choose at each support point a [local parameter](../../../projective-space.md#local-parameter-on-a-smooth-algebraic-curve) $t_P$ and shrink its neighbourhood to exclude every other zero or pole of $t_P$ and every other support point. The local rational equation $t_P^{n_P}$ represents the desired valuations there; on the complement of the support use $1$. On overlaps these equations differ by units, so their classes glue in the quotient [sheaf](../../../algebraic-geometry.md#sheaf-mathematics). Finally, a section with every valuation zero has zero germ everywhere and is the identity section. Hence the identification is both [surjective](../../../algebra.md#surjective-function) and [injective](../../../algebra.md#injective-function).

The map on [global sections](../../../ringed-space.md#global-section) sends $f\in k(X)^*$ to $\operatorname{div}(f)$. Therefore its [cokernel](../../../linear-algebra.md#cokernel) is

$$
\boxed{\operatorname{coker}\bigl(H^0(X,\mathcal K_X^*)\to
H^0(X,\mathcal K_X^*/\mathcal O_X^*)\bigr)
=\operatorname{Div}(X)/\operatorname{Prin}(X)
\cong\operatorname{Cl}(X).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D=\sum n_PP$, define its [line bundle associated to a divisor](../../../cartier-divisor.md#line-bundle-associated-to-a-divisor) inside the [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) of rational functions by

$$
\mathcal O_X(D)(U)=
\{f\in k(X)^*:v_P(f)+n_P\ge0\text{ for every }P\in U\}\cup\{0\}.
$$

Locally choose a rational equation $f_i$ for $D$, as in the construction of the quotient [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) above. Then

$$
\mathcal O_X(D)|_{U_i}=f_i^{-1}\mathcal O_{U_i},
\qquad
\mathcal O_X(D)_P=t_P^{-n_P}\mathcal O_{X,P}.
$$

Consequently this is an [invertible sheaf](../../../ringed-space.md#line-bundle). Multiplication gives an [isomorphism](../../../algebra.md#isomorphism)

$$
\mathcal O_X(D)\otimes_{\mathcal O_X}\mathcal O_X(E)
\cong\mathcal O_X(D+E),
$$

as is checked on the displayed local generators. If $D=\operatorname{div}(f)$, multiplication by $f$ identifies $\mathcal O_X(D)$ with $\mathcal O_X$. Thus $D\mapsto[\mathcal O_X(D)]$ induces a [group homomorphism](../../../group-theory.md#group-homomorphism) from the [divisor class group](../../../algebraic-geometry.md#divisor-class-group) to the [Picard group](../../../ringed-space.md#picard-group).

For surjectivity, let $\mathcal L$ be an [invertible sheaf](../../../ringed-space.md#line-bundle). Trivialize its one-dimensional rational fibre over the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) $k(X)$; equivalently, choose a nonzero rational section and identify $\mathcal L$ with a subsheaf of the rational-function [sheaf](../../../algebraic-geometry.md#sheaf-mathematics). A finite trivializing cover gives

$$
\mathcal L|_{U_i}=a_i\mathcal O_{U_i},\qquad a_i\in k(X)^*.
$$

On overlaps $a_i/a_j$ is a regular unit. The integers $-v_P(a_i)$ therefore agree wherever two descriptions apply and define a finite [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$. Its local description gives $\mathcal L=\mathcal O_X(D)$. A different rational trivialization multiplies all $a_i$ by the same rational function, changing $D$ by a [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve), so the resulting [divisor class](../../../algebraic-geometry.md#divisor-class) is intrinsic.

For injectivity, an [isomorphism](../../../algebra.md#isomorphism) $\mathcal O_X(D)\to\mathcal O_X(E)$ becomes multiplication by some $g\in k(X)^*$ on the rational fibre. At each closed point its effect on the local free generators gives

$$
g\,t_P^{-n_P(D)}\mathcal O_{X,P}
=t_P^{-n_P(E)}\mathcal O_{X,P},
\qquad
v_P(g)=n_P(D)-n_P(E).
$$

Hence $D-E=\operatorname{div}(g)$. Conversely this equality gives the required [isomorphism](../../../algebra.md#isomorphism) by multiplication by $g$. We have proved the [group isomorphism](../../../algebra.md#group-isomorphism)

$$
\boxed{\operatorname{Cl}(X)\xrightarrow{\;\sim\;}
\operatorname{Pic}(X),\qquad[D]\longmapsto[\mathcal O_X(D)].}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Since $X$ is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety), every nonempty open subset is irreducible and the [sheaf of nonzero rational functions on an irreducible variety](../../../algebraic-geometry.md#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety) has value $k(X)^*$ there. All its restriction maps between nonempty opens are identities, and restriction to the empty set is [surjective](../../../algebra.md#surjective-function). Thus $\mathcal K_X^*$ is a [flabby sheaf](../../../ringed-space.md#flasque-sheaf), and the introductory argument gives $H^1(X,\mathcal K_X^*)=0$.

Apply the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) to the [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
1\longrightarrow\mathcal O_X^*\longrightarrow\mathcal K_X^*
\longrightarrow\mathcal D\longrightarrow1.
$$

Its relevant portion is

$$
H^0(X,\mathcal K_X^*)\longrightarrow H^0(X,\mathcal D)
\xrightarrow{\;\partial\;}H^1(X,\mathcal O_X^*)
\longrightarrow H^1(X,\mathcal K_X^*)=0.
$$

The [connecting homomorphism](../../../homology.md#connecting-homomorphism) is therefore [surjective](../../../algebra.md#surjective-function), with kernel the image of $k(X)^*$. The computation in part (a) now gives

$$
\boxed{\operatorname{Cl}(X)\cong H^1(X,\mathcal O_X^*).}
$$

Concretely, local rational equations $f_i$ of a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) differ by regular units on overlaps. Their ratios give the gluing data of an [invertible sheaf](../../../ringed-space.md#line-bundle); changing the local equations by units changes those data by a coboundary. This is the transition-function interpretation of the identification with the [Picard group](../../../ringed-space.md#picard-group). Reversing all transition ratios replaces a class by its inverse; either consistent convention gives the same group [isomorphism](../../../algebra.md#isomorphism).

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $X$ be an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) over an [algebraically closed field](../../../algebra.md#algebraically-closed-field) $k$, with reduced [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $A=k[X]$. On an open subset $U$, define $\mathcal O_X(U)$ to be the functions $h:U\to k$ which, near every point, have an expression $a/b$ with $a,b\in A$ and $b$ nowhere zero on that neighbourhood. Restriction is ordinary restriction of functions. Compatible local functions glue uniquely and remain locally quotients, so this defines the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme). On the [principal open subset](../../../ringed-space.md#principal-open-subscheme) $D(f)$ it gives $A_f$, and at $P$ it gives the [local ring](../../../commutative-algebra.md#local-ring) $A_{\mathfrak m_P}$. The principal-open identification can also be seen by identifying $D(f)$ with the affine algebraic set obtained by adjoining a coordinate $t$ and the equation $tf=1$; its [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) is $A[t]/(tf-1)\cong A_f$. This construction permits several [irreducible components](../../../algebraic-geometry.md#irreducible-component); no division by a function vanishing identically on a component is assumed.

An abstract [algebraic variety](../../../algebraic-geometry.md#algebraic-variety) is a [locally ringed space](../../../ringed-space.md#locally-ringed-space) locally isomorphic to such affine models, with a finite affine cover; we use the usual separated convention. Reducible [varieties](../../../algebraic-geometry.md#algebraic-variety) are allowed here. The separation condition says that the [diagonal morphism](../../../ringed-space.md#diagonal-morphism) is a [closed immersion](../../../ringed-space.md#closed-immersion). Two [varieties](../../../algebraic-geometry.md#algebraic-variety) are related by a [birational map](../../../algebraic-geometry.md#birational-map) with an inverse when some dense open subset of one is [isomorphic](../../../algebra.md#isomorphism) as a locally ringed space to a dense open subset of the other.

Define the [ring of rational functions on a reduced variety](../../../algebraic-geometry.md#ring-of-rational-functions-on-a-reduced-variety) by pairs $(U,h)$, where $U\subseteq X$ is dense open and $h\in\mathcal O_X(U)$, identifying two pairs when their restrictions agree on a common dense open subset. Finite intersections of dense open subsets are dense, so addition and multiplication on these intersections are well defined. For an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) this gives the usual [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety); for a reducible [variety](../../../algebraic-geometry.md#algebraic-variety) it need not be a [field](../../../algebra.md#field). Restriction to any dense open subset $V$ induces an [isomorphism](../../../algebra.md#isomorphism)

$$
\operatorname{Rat}(X)\cong\operatorname{Rat}(V).
$$

Indeed, intersecting domains with $V$ defines the restriction, and a dense open subset of $V$ is also dense open in $X$, which defines its inverse. An [isomorphism](../../../algebra.md#isomorphism) between dense opens therefore induces an [isomorphism](../../../algebra.md#isomorphism) of their rational rings. Thus **birational [varieties](../../../algebraic-geometry.md#algebraic-variety) have isomorphic rings of rational functions**, also in the reducible case.

For the finite-cover assertion, write the closed complement of $U$ as $V(I)$, where $I=(f_1,\ldots,f_r)$ is an [ideal](../../../commutative-algebra.md#ideal) of the [Noetherian ring](../../../algebra.md#noetherian-ring) $A$. Then

$$
U=D(f_1)\cup\cdots\cup D(f_r).
$$

Let $\mathfrak p_1,\ldots,\mathfrak p_t$ be the [minimal prime ideals](../../../commutative-algebra.md#minimal-prime-ideal) of $A$, corresponding to its [irreducible components](../../../algebraic-geometry.md#irreducible-component). Since $U$ is dense, it meets every component, so $I$ is contained in none of these primes. [Prime avoidance](../../../commutative-algebra.md#prime-avoidance) supplies $s\in I$ outside their union. Consequently $D(s)\subseteq U$ meets a dense open subset of every component and is dense in $X$. Add $D(s)$ to the finite cover if necessary. This proves that **a finite principal-open cover can be chosen with a dense member**. It does not say that every principal-open cover already has such a member: for $X=V(xy)$, the dense open $X\setminus\{(0,0)\}=D(x)\cup D(y)$ has neither displayed member dense, although adding $D(x+y)$ supplies a dense member.

For clarity, the [zero divisors](../../../mathematics.md#zero-divisor) in this reduced [Noetherian ring](../../../algebra.md#noetherian-ring) are exactly $\bigcup_i\mathfrak p_i$. If $ab=0$ and $a$ avoids every $\mathfrak p_i$, reduction in the domain $A/\mathfrak p_i$ forces $b\in\mathfrak p_i$ for all $i$, hence $b=0$. Conversely, if $a\in\mathfrak p_i$, choose for every $j\ne i$ an element $b_j\in\mathfrak p_j\setminus\mathfrak p_i$, possible because distinct minimal primes are incomparable. Their product $b$ is not in $\mathfrak p_i$ but belongs to all the other primes. Then $b\ne0$ and $ab\in\bigcap_j\mathfrak p_j=0$. For a single minimal prime, reducedness makes that prime zero and this argument uses $b=1$. It follows that

$$
s\text{ is a non-zero-divisor}\quad\Longleftrightarrow\quad D(s)\text{ is dense}.
$$

The [total quotient ring](../../../commutative-algebra.md#total-ring-of-fractions) $S^{-1}A$, where $S$ consists of these [non-zero-divisors](../../../mathematics.md#non-zero-divisor), maps to $\operatorname{Rat}(X)$ by

$$
a/s\longmapsto\text{the class of the regular function }a/s\text{ on }D(s).
$$

The equivalence relation for [localization](../../../commutative-algebra.md#localization-of-a-ring) makes this a well-defined $k$-algebra homomorphism. For surjectivity, a rational class represented on $U$ restricts to the dense principal open $D(s)\subseteq U$ constructed above. Its section there belongs to $A_s$, so it is $a/s^r$ and lies in the image. For injectivity, if such a fraction is zero on a dense open subset, its numerator vanishes on that dense subset. The numerator's zero set is closed, so it vanishes everywhere on $X$ and is zero in the reduced [coordinate ring](../../../algebraic-geometry.md#coordinate-ring). Thus

$$
\boxed{\operatorname{Rat}(X)\cong S^{-1}A.}
$$

In particular $A\to S^{-1}A$ is canonically [injective](../../../algebra.md#injective-function): $a/1=0$ implies $sa=0$ for some [non-zero-divisor](../../../mathematics.md#non-zero-divisor) $s$, hence $a=0$.

Finally let $Y$ be the reduced closed union of exactly those [irreducible components](../../../algebraic-geometry.md#irreducible-component) of $X$ which contain $P$. Removing all the other components gives an open neighbourhood of $P$ on which $X$ and $Y$ coincide, including their [structure sheaves](../../../ringed-space.md#structure-sheaf-of-a-scheme). Hence $\mathcal O_{X,P}\cong\mathcal O_{Y,P}$. Write $B=k[Y]$ and let $\mathfrak n_P$ be its maximal ideal at $P$. Every minimal prime of $B$ is contained in $\mathfrak n_P$, because every component of $Y$ contains $P$. If $b\notin\mathfrak n_P$, it avoids each such prime and is a [non-zero-divisor](../../../mathematics.md#non-zero-divisor). Therefore the map of [localizations](../../../commutative-algebra.md#localization-of-a-ring)

$$
B_{\mathfrak n_P}\longrightarrow Q(B)=\operatorname{Rat}(Y),
\qquad a/b\longmapsto a/b,
$$

is defined and [injective](../../../algebra.md#injective-function): if its value is zero, a [non-zero-divisor](../../../mathematics.md#non-zero-divisor) annihilates $a$, so $a=0$. We obtain the desired [local ring embeds in rational functions on incident components](../../../algebraic-geometry.md#local-ring-embeds-in-rational-functions-on-incident-components):

$$
\boxed{\mathcal O_{X,P}\hookrightarrow\operatorname{Rat}(Y),
\qquad Y=\bigcup_{P\in X_i}X_i\ \text{with reduced structure}.}
$$

At an intersection point one must retain all incident components. For example, the [local ring](../../../commutative-algebra.md#local-ring) of $V(xy)$ at the origin has two nonzero germs $x,y$ with $xy=0$; it cannot embed into the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) of just one of its axes.

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf) is a [sheaf of modules](../../../ringed-space.md#sheaf-of-modules) which locally has a presentation by [free module](../../../module-theory.md#free-module) [sheaves](../../../algebraic-geometry.md#sheaf-mathematics):

$$
\mathcal O_U^{(J)}\longrightarrow\mathcal O_U^{(I)}
\longrightarrow\mathcal F|_U\longrightarrow0,
$$

where the index sets may be infinite. Equivalently, on affine neighbourhoods it is an [affine module sheaf](../../../ringed-space.md#affine-module-sheaf). A [coherent sheaf](../../../ringed-space.md#coherent-sheaf) is locally finitely generated, with the additional requirement that the kernel of every map from a [finite free module](../../../module-theory.md#finite-free-module) [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) is locally finitely generated. On a [Noetherian scheme](../../../ringed-space.md#noetherian-scheme), these conditions are equivalent to being locally associated with a [finitely generated module](../../../module-theory.md#finitely-generated-module).

For an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) $X$ with [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $A$ and an $A$-[module](../../../module-theory.md#module-mathematics) $M$, set

$$
\widetilde M(D(a))=M_a,\qquad
\widetilde M_P=M_{\mathfrak m_P}.
$$

Restriction on [principal open subsets](../../../ringed-space.md#principal-open-subscheme) is the natural [module localization](../../../commutative-algebra.md#localization-of-a-module) map. On an arbitrary open subset, sections are families of these stalk values locally represented by a single fraction from a [localization](../../../commutative-algebra.md#localization-of-a-ring). This constructs the [affine module sheaf](../../../ringed-space.md#affine-module-sheaf); its [global sections](../../../ringed-space.md#global-section) are $M$. Choose a free-module presentation $A^{(J)}\to A^{(I)}\to M\to0$. [Exactness of localization](../../../commutative-algebra.md#exactness-of-localization) and its compatibility with direct sums yield

$$
\mathcal O_X^{(J)}\longrightarrow\mathcal O_X^{(I)}
\longrightarrow\widetilde M\longrightarrow0.
$$

Thus $\widetilde M$ is a [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf), without a finite-generation assumption.

We now prove [coherence of an affine module sheaf](../../../ringed-space.md#coherence-of-an-affine-module-sheaf). If $M$ is finitely generated, take a [surjection](../../../algebra.md#surjective-function) $A^r\to M$. Since $A$ is a [Noetherian ring](../../../algebra.md#noetherian-ring), its kernel is finitely generated, so $M$ has a [finite presentation of a module](../../../module-theory.md#finite-presentation-of-a-module). More generally, on every principal affine open, the kernel of a map $A_a^s\to M_a$ is a [submodule](../../../module-theory.md#submodule) of a [finite free module](../../../module-theory.md#finite-free-module) over the [Noetherian ring](../../../algebra.md#noetherian-ring) $A_a$, and is finitely generated. On sheafifying, this verifies both parts of the definition of a [coherent sheaf](../../../ringed-space.md#coherent-sheaf).

Conversely, if $\widetilde M$ is coherent, choose a finite principal-open cover $X=\bigcup_iD(a_i)$ on which it has finitely many generators. Write those local generators as $m_{ij}/a_i^{r_{ij}}$. Their numerators generate a finite [submodule](../../../module-theory.md#submodule) $N=\sum_{i,j}Am_{ij}$ of $M$, and $N_{a_i}=M_{a_i}$ for every $i$. To check that $M/N=0$, let $q\in M/N$. Each equality after [localization](../../../commutative-algebra.md#localization-of-a-ring) gives an exponent $r_i$ such that $a_i^{r_i}q=0$. The ideal generated by the $a_i^{r_i}$ is the [unit ideal](../../../commutative-algebra.md#unit-ideal): otherwise a maximal ideal containing all of them would give a point outside the principal-open cover. A linear combination of these powers equal to $1$ consequently annihilates $q$. Every $q$ is zero, proving

$$
\boxed{\widetilde M\text{ is coherent}\quad\Longleftrightarrow\quad
M\text{ is a finitely generated }A\text{-module}.}
$$

Next consider a morphism $\phi:\mathcal G_1\to\mathcal G_2$ between [quasi-coherent sheaves](../../../ringed-space.md#quasi-coherent-sheaf). On an affine open $V$ of the target [variety](../../../algebraic-geometry.md#algebraic-variety), use the assumed [affine module-sheaf equivalence](../../../ringed-space.md#affine-module-sheaf-equivalence) to write $\mathcal G_j|_V=\widetilde{M_j}$, with $M_j=\Gamma(V,\mathcal G_j)$. The [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) morphism is the sheafification of the [module](../../../module-theory.md#module-mathematics) map $\psi=\Gamma(V,\phi)$. Indeed, its action on a section $m/a^r$ of a principal open is forced by module-linearity and restriction to be $\psi(m)/a^r$. Therefore [exactness of localization](../../../commutative-algebra.md#exactness-of-localization) gives

$$
(\ker\phi)(D(a))=\ker\bigl((M_1)_a\to(M_2)_a\bigr)
=(\ker\psi)_a.
$$

These identities are compatible with restriction, so $(\ker\phi)|_V=\widetilde{\ker\psi}$. Since this holds on an affine cover, **the [kernel sheaf](../../../algebraic-geometry.md#kernel-sheaf) is quasi-coherent on every [variety](../../../algebraic-geometry.md#algebraic-variety)**. This proof of [kernels of quasi-coherent sheaf morphisms](../../../ringed-space.md#kernels-of-quasi-coherent-sheaf-morphisms) does not assert that taking [global sections](../../../ringed-space.md#global-section) is right exact.

For [direct image](../../../ringed-space.md#direct-image-sheaf) along a morphism of [affine varieties](../../../algebraic-geometry.md#affine-algebraic-set), write $Y$ with [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $A$, $X$ with [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $B$, and let $\alpha:A\to B$ be the induced ring homomorphism. If $\mathcal F=\widetilde M$ on $X$, regard $M$ as an $A$-module by [restriction of scalars](../../../module-theory.md#restriction-of-scalars). For $a\in A$,

$$
f^{-1}(D(a))=D(\alpha(a)),\qquad
(f_*\mathcal F)(D(a))=M_{\alpha(a)}=M_a.
$$

The last equality identifies [localization](../../../commutative-algebra.md#localization-of-a-ring) with the scalar action of $a$. It identifies the [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) with the [affine module sheaf](../../../ringed-space.md#affine-module-sheaf) of the restricted [module](../../../module-theory.md#module-mathematics), so $f_*\mathcal F$ is quasi-coherent.

Suppose $Y$ is affine and $X=\bigcup_{i=1}^rU_i$ is a finite affine cover. Since a [variety](../../../algebraic-geometry.md#algebraic-variety) is separated, every $U_i\cap U_j$ is affine: it is identified with the inverse image of the closed [diagonal morphism](../../../ringed-space.md#diagonal-morphism) inside the affine product $U_i\times_kU_j$. Write $g_i=f|_{U_i}$ and $g_{ij}=f|_{U_i\cap U_j}$. Form the morphism of [sheaves of modules](../../../ringed-space.md#sheaf-of-modules)

$$
d:\bigoplus_i(g_i)_*(\mathcal F|_{U_i})
\longrightarrow
\bigoplus_{i,j}(g_{ij})_*(\mathcal F|_{U_i\cap U_j}),
\qquad
(s_i)\longmapsto(s_i|_{U_i\cap U_j}-s_j|_{U_i\cap U_j}).
$$

Both sums are finite, and every summand is quasi-coherent by the affine calculation. For every open $V\subseteq Y$, the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) on $f^{-1}(V)$ identifies the kernel of this map on sections with $\mathcal F(f^{-1}(V))$. Hence

$$
f_*\mathcal F=\ker d.
$$

The kernel result proved above establishes quasi-coherence.

Finally, for arbitrary $Y$, take an affine neighbourhood $V\subseteq Y$ and apply the preceding argument to $f^{-1}(V)\to V$. The open subset $f^{-1}(V)$ is again a [variety](../../../algebraic-geometry.md#algebraic-variety) and has a finite affine cover, because [varieties](../../../algebraic-geometry.md#algebraic-variety) have [Noetherian Zariski topology](../../../algebraic-geometry.md#noetherian-zariski-topology). The restriction of $f_*\mathcal F$ to $V$ is exactly the direct image for this restricted morphism. Thus

$$
\boxed{f_*\mathcal F\text{ is quasi-coherent for every morphism of varieties}.}
$$

The finiteness and separation conditions are the relevant hypotheses, not affineness of the original source or target. More generally, [quasi-coherence of direct image under a quasi-compact quasi-separated morphism](../../../ringed-space.md#quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism) is valid. If one permits nonseparated finite-type prevarieties, each overlap in the argument has a finite affine cover; replacing its summand by the sum of direct images from these charts gives the same kernel, since agreement can be tested on a cover. This also proves the assertion in that convention. It does not extend by this argument to arbitrary spaces with an unrestricted infinite cover.

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $S=k[X_0,\ldots,X_n]$ with its usual grading, and put $S(m)_d=S_{m+d}$. Define the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) by

$$
\mathcal O_{\mathbb P^n}(m)=\widetilde{S(m)}.
$$

More explicitly, on $U_i=D_+(X_i)$ its sections are the homogeneous degree-$m$ part of $S_{X_i}$. They are a free rank-one [module](../../../module-theory.md#module-mathematics) over $(S_{X_i})_0=k[X_j/X_i:j\ne i]$, with generator $e_i=X_i^m$. These generators make sense for every integer $m$, since $X_i$ is invertible on this chart. Their transition rule is

$$
e_i=(X_i/X_j)^m e_j.
$$

The ratios are regular units on overlaps and satisfy the cocycle identity, so they glue to an [invertible sheaf](../../../ringed-space.md#line-bundle). In particular $\mathcal O(m)\otimes\mathcal O(r)\cong\mathcal O(m+r)$.

For $n\ge1$, a [global section](../../../ringed-space.md#global-section) is a compatible homogeneous degree-$m$ rational expression lying in every $S_{X_i}$. Inside the [fraction field](../../../commutative-algebra.md#field-of-fractions) of $S$,

$$
\bigcap_{i=0}^nS_{X_i}=S.
$$

To justify this, write a fraction in lowest terms in the [unique factorization domain](../../../algebra.md#unique-factorization-domain) $S$. Membership in $S_{X_i}$ forces every irreducible divisor of its denominator to be associated with $X_i$. Since there are at least two nonassociated variables, the denominator must be a unit. Therefore

$$
H^0(\mathbb P^n,\mathcal O(m))=
\begin{cases}
S_m,&m\ge0,\\
0,&m<0,
\end{cases}
\qquad(n\ge1).
$$

The degree-$m$ [monomials](../../../polynomial.md#monomial) are indexed by nonnegative integers $a_0,\ldots,a_n$ with sum $m$. The [stars and bars](../../../combinatorics.md#stars-and-bars-combinatorics) count gives

$$
\boxed{h^0(\mathcal O_{\mathbb P^n}(m))=
\begin{cases}
\binom{m+n}{n},&m\ge0,\\
0,&m<0,
\end{cases}\qquad(n\ge1).}
$$

Here and below, an all-integer binomial shorthand must use the counting convention $\binom{a}{n}=0$ when $a<n$, including negative $a$. The polynomial extension of binomial coefficients to negative upper arguments does not give the stated dimensions. In dimension zero, $\mathbb P^0$ is one point and every $\mathcal O_{\mathbb P^0}(m)$ is trivial, so its space of [global sections](../../../ringed-space.md#global-section) is $k$ for every $m$; this case is treated separately.

For a closed inclusion $i:H\hookrightarrow\mathbb P^n$, [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) formation is exact: its stalk is the original stalk at a point of $H$ and zero outside $H$. It preserves [flabby sheaves](../../../ringed-space.md#flasque-sheaf), since restrictions on the target are restrictions between the corresponding open subsets of $H$. Push forward a [flasque resolution](../../../ringed-space.md#flasque-resolution) of $\mathcal F$; exactness gives a [flasque resolution](../../../ringed-space.md#flasque-resolution) of $i_*\mathcal F$, and its complex of [global sections](../../../ringed-space.md#global-section) is the original one because

$$
\Gamma(\mathbb P^n,i_*\mathcal I^j)=\Gamma(H,\mathcal I^j).
$$

Taking cohomology of these identical complexes proves [sheaf cohomology under a closed inclusion](../../../ringed-space.md#sheaf-cohomology-under-a-closed-inclusion):

$$
\boxed{H^r(H,\mathcal F)\cong H^r(\mathbb P^n,i_*\mathcal F)\quad(r\ge0).}
$$

This argument applies even without quasi-coherence.

We derive the remaining [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) dimensions using the given eventual vanishing, the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology), and induction on dimension. Multiplication by the linear equation of a [hyperplane](../../../vector-space.md#hyperplane) $H\cong\mathbb P^{n-1}$ gives the [hyperplane exact sequence for twisting sheaves](../../../ringed-space.md#hyperplane-exact-sequence-for-twisting-sheaves)

$$
0\longrightarrow\mathcal O_{\mathbb P^n}(m-1)
\longrightarrow\mathcal O_{\mathbb P^n}(m)
\longrightarrow i_*\mathcal O_H(m)\longrightarrow0.
$$

Exactness can be checked in each chart by quotienting its [polynomial ring](../../../commutative-algebra.md#polynomial-ring) by the equation of $H$; multiplication is [injective](../../../algebra.md#injective-function) because that equation is a [non-zero-divisor](../../../mathematics.md#non-zero-divisor). We use the closed-inclusion cohomology identification to replace the cohomology of the final [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) by that on $H$.

The dimension-zero base is a point, whose global-section functor is exact. Thus all its higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) is zero. For $n=1$, the relevant [long exact sequence](../../../homology.md#long-exact-sequence) is

$$
0\to H^0(\mathcal O(m-1))\to H^0(\mathcal O(m))
\to k\to H^1(\mathcal O(m-1))\to H^1(\mathcal O(m))\to0.
$$

When $m\ge0$, restriction of [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) to the hyperplane point is [surjective](../../../algebra.md#surjective-function): after choosing that point as $[1:0]$, the section $X_0^m$ restricts to a generator. Therefore the consecutive $H^1$ groups are isomorphic for $m\ge0$. The given vanishing for large $m$ propagates down to $m=-1$. For $m<0$, both displayed $H^0$ groups are zero, and the sequence becomes

$$
0\to k\to H^1(\mathcal O(m-1))\to H^1(\mathcal O(m))\to0.
$$

Starting with $H^1(\mathcal O(-1))=0$, induction downward gives $h^1(\mathcal O(m))=-m-1$ for $m\le-2$. For degrees $i>1$, the point contributes no cohomology to the exact sequence, so consecutive $H^i$ groups are isomorphic for every $m$; the given eventual vanishing makes them all zero. Hence the complete positive-degree formula holds for $\mathbb P^1$.

Now let $n\ge2$ and assume the formulas for $H\cong\mathbb P^{n-1}$. For every $m$, the restriction

$$
H^0(\mathbb P^n,\mathcal O(m))\to H^0(H,\mathcal O_H(m))
$$

is [surjective](../../../algebra.md#surjective-function): for $m\ge0$ extend a polynomial in the hyperplane coordinates to the same polynomial on $\mathbb P^n$, and for $m<0$ both groups vanish because $H$ has positive dimension. Consequently the exact sequence gives an [injection](../../../algebra.md#injective-function)

$$
H^1(\mathbb P^n,\mathcal O(m-1))
\hookrightarrow H^1(\mathbb P^n,\mathcal O(m)).
$$

For $2\le i\le n-1$, the induction hypothesis says $H^{i-1}(H,\mathcal O_H(m))=0$, and gives the same [injection](../../../algebra.md#injective-function) in degree $i$. For each fixed $m$, composing finitely many [injections](../../../algebra.md#injective-function) reaches a sufficiently large twist, whose higher cohomology is zero by the given hypothesis. Therefore

$$
H^i(\mathbb P^n,\mathcal O(m))=0
\quad(0<i<n,\ \text{every }m).
$$

For $i>n$, the two neighbouring hyperplane groups $H^{i-1}(H,\mathcal O_H(m))$ and $H^i(H,\mathcal O_H(m))$ are zero by induction. Consecutive $H^i$ groups on $\mathbb P^n$ are then isomorphic, and eventual vanishing again makes them zero. This derives vanishing above the dimension too, without needing a special projective-space cohomology theorem.

For top cohomology the exact sequence now reduces to

$$
0\to H^{n-1}(H,\mathcal O_H(m))
\to H^n(\mathbb P^n,\mathcal O(m-1))
\to H^n(\mathbb P^n,\mathcal O(m))\to0.
$$

Write $b_n(m)=h^n(\mathcal O_{\mathbb P^n}(m))$. The induction hypothesis and eventual vanishing give the recurrence

$$
b_n(m-1)=b_n(m)+b_{n-1}(m),\qquad
b_{n-1}(m)=
\begin{cases}
\binom{-m-1}{n-1},&m\le-n,\\
0,&m\ge-n+1.
\end{cases}
$$

Consecutive top groups agree for $m\ge-n+1$, so descending from a large twist gives $b_n(m)=0$ for $m\ge-n$. Below this range, iterating the recurrence gives a finite sum:

$$
b_n(m)=\sum_{j=m+1}^{-n}\binom{-j-1}{n-1}
=\sum_{\ell=n-1}^{-m-2}\binom{\ell}{n-1}
=\binom{-m-1}{n}
\qquad(m\le-n-1).
$$

The last equality follows by summing [Pascal's identity](../../../combinatorics.md#pascal-s-rule). These short exact sequences also prove that every group whose dimension is being counted is finite-dimensional. Thus, for $n\ge1$,

$$
\boxed{
h^i(\mathcal O_{\mathbb P^n}(m))=0\quad(0<i\ne n),\qquad
h^n(\mathcal O_{\mathbb P^n}(m))=
\begin{cases}
\binom{-m-1}{n},&m\le-n-1,\\
0,&m\ge-n.
\end{cases}}
$$

With the stated counting convention, the latter is the requested single binomial formula. The base $\mathbb P^0$ has $h^0=1$ for all twists and no higher cohomology; it is not governed by the negative-twist $H^0$ rule for positive-dimensional projective space.

Finally calculate the [canonical line bundle of a smooth variety](../../../ringed-space.md#canonical-line-bundle-of-a-smooth-variety) from its transition functions. On $U_0$ write $t_j=X_j/X_0$ for $1\le j\le n$. On $U_i$, $i>0$, take the coordinates $u_j=X_j/X_i$ in increasing order of $j\ne i$. Thus

$$
u_0=t_i^{-1},\qquad u_j=t_j/t_i\quad(j\ne0,i).
$$

In their wedge product, $du_0=-t_i^{-2}\,dt_i$ and  
$du_j=t_i^{-1}dt_j-t_jt_i^{-2}dt_i$. Every term involving a second $dt_i$ vanishes, so reordering the remaining differentials gives

$$
\bigwedge_{j\ne i}du_j
=(-1)^i t_i^{-(n+1)}\,dt_1\wedge\cdots\wedge dt_n.
$$

This computation is valid in every characteristic. Multiply the ordered local generator on $U_i$ by $(-1)^i$. The resulting generators $\eta_i$ satisfy $\eta_i=(X_i/X_0)^{-n-1}\eta_0$ on $U_i\cap U_0$, and hence the corresponding transition rule on every overlap. They are exactly the transitions of $\mathcal O(-n-1)$. Therefore the [canonical bundle of projective space](../../../ringed-space.md#canonical-bundle-of-projective-space) is

$$
\boxed{\omega_{\mathbb P^n}\cong\mathcal O_{\mathbb P^n}(-n-1).}
$$

For a [line bundle](../../../ringed-space.md#line-bundle), [Serre duality](../../../ringed-space.md#serre-duality) states

$$
H^i(\mathbb P^n,\mathcal O(m))^*
\cong H^{n-i}(\mathbb P^n,\mathcal O(-m-n-1)).
$$

The intermediate groups on both sides vanish. In the two outer degrees, the top group at twist $m$ has the same dimension as the global-section group at twist $-m-n-1$:

$$
h^n(\mathcal O(m))=h^0(\mathcal O(-m-n-1)).
$$

The polynomial degree on the right is nonnegative precisely when $m\le-n-1$, and its dimension is $\binom{-m-1}{n}$. Interchanging $m$ and $-m-n-1$ checks the other outer degree. On $\mathbb P^0$ both sides are one-dimensional. Thus all the formulas are consistent with [Serre duality](../../../ringed-space.md#serre-duality), which was used only for this final consistency check, not to prove the cohomology formulas.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
