# Paper 151

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_151.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_151.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
    - [iv](#2/c/iv)
      - [Solution](#2/c/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
    - [iv](#4/a/iv)
      - [Solution](#4/a/iv/solution)
    - [v](#4/a/v)
      - [Solution](#4/a/v/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)

## 1

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

For an [inverse system](../../../module-theory.md#inverse-system) of sets $(X_j,f_{ij})$ indexed by a [directed set](../../../set.md#directed-set) $J$, the [inverse limit](../../../module-theory.md#inverse-limit) is the set of compatible tuples

$$
\varprojlim_{j\in J}X_j
=\left\{(x_j)\in\prod_{j\in J}X_j:f_{ij}(x_j)=x_i\text{ whenever }i\leq j\right\}.
$$

Its projection to $X_j$ sends $(x_i)_i$ to $x_j$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Give each nonempty [finite set](../../../set.md#finite-set) $X_j$ the [discrete topology](../../../topology.md#discrete-space). The [product space](../../../geometry-and-topology.md#product-space) $X=\prod_jX_j$ is [compact](../../../topology.md#compact-space) by the [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem). For each $i\leq j$, the compatibility condition $f_{ij}(x_j)=x_i$ defines a [closed subset](../../../topology.md#closed-set) $C_{ij}\subseteq X$.

These sets have the [finite intersection property](../../../topology.md#finite-intersection-property). Indeed, for finitely many conditions choose an index $k$ above every index occurring in them, choose any $x_k\in X_k$, and use the transition maps from $k$ to define all required coordinates; choose the remaining coordinates arbitrarily. Compactness therefore gives

$$
\varprojlim_jX_j=\bigcap_{i\leq j}C_{ij}\ne\varnothing.
$$

This is the [nonemptiness theorem for inverse limits of finite sets](../../../module-theory.md#nonemptiness-theorem-for-inverse-limits-of-finite-sets).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The product $\prod_jG_j$ of the [finite groups](../../../group.md#finite-group) with their [discrete topology](../../../topology.md#discrete-space) is a [topological group](../../../topological-group.md) under coordinatewise multiplication and inversion. The compatibility equations defining $G=\varprojlim_jG_j$ are preserved by both operations, so $G$ is a subgroup. Their restrictions to the [subspace topology](../../../topology.md#subspace-topology) on $G$ are continuous. Hence $G$ with its standard [inverse-limit topology](../../../topological-group.md#inverse-limit-topology) is a topological group.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For fixed $h\in G$, the [conjugation](../../../group-theory.md#conjugation) map is the composite

$$
G\longrightarrow G\times G\times G,
\qquad g\longmapsto(g,h,g^{-1}),
$$

followed by multiplication. Inversion, constant maps, diagonal maps, and multiplication are continuous in a [topological group](../../../topological-group.md), so $c_h(g)=ghg^{-1}$ is continuous.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The [profinite group](../../../topological-group.md#profinite-group) $G$ is [compact](../../../topology.md#compact-space), and the preceding part shows that

$$
\operatorname{Cl}_G(h)=c_h(G)
$$

is its image. By the [continuous image of a compact space](../../../topology.md#continuous-image-of-a-compact-space) theorem, the [conjugacy class](../../../group-theory.md#conjugacy-class) is compact. Since a profinite group is [Hausdorff](../../../topology.md#hausdorff-space), every compact subset is closed, so $\operatorname{Cl}_G(h)$ is closed.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

If $g=xhx^{-1}$ in $G$, applying each [projection map](../../../function.md#projection-map) gives $p_j(g)=p_j(x)p_j(h)p_j(x)^{-1}$ in $G_j$.

Conversely, suppose $p_j(g)$ and $p_j(h)$ are conjugate for every $j$. Define the nonempty finite set

$$
X_j=\{x_j\in G_j:x_jp_j(h)x_j^{-1}=p_j(g)\}.
$$

Every transition map $G_j\to G_i$ carries $X_j$ into $X_i$, so the $X_j$ form an [inverse system](../../../module-theory.md#inverse-system). By the [nonemptiness theorem for inverse limits of finite sets](../../../module-theory.md#nonemptiness-theorem-for-inverse-limits-of-finite-sets), there is a compatible tuple $(x_j)\in\varprojlim_jX_j\subseteq G$. Coordinatewise equality then gives $xhx^{-1}=g$. This proves the [finite-quotient criterion for conjugacy in a profinite group](../../../topological-group.md#finite-quotient-criterion-for-conjugacy-in-a-profinite-group).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The canonical image of $\Gamma$ is [dense](../../../topology.md#dense-set) in its [profinite completion](../../../topological-group.md#profinite-completion) $\widehat\Gamma$. Therefore every $x\in\widehat\Gamma$ is a limit of a net $(\delta_\lambda)$ in $\Gamma$. Continuity of conjugation gives

$$
\delta_\lambda\gamma\delta_\lambda^{-1}
\longrightarrow x\gamma x^{-1},
$$

so every element of $\operatorname{Cl}_{\widehat\Gamma}(\gamma)$ lies in the [closure](../../../topology.md#closure-topology) of $\operatorname{Cl}_\Gamma(\gamma)$. The reverse inclusion follows because the larger conjugacy class contains the smaller one and is closed by part b(iii). Hence

$$
\boxed{\overline{\operatorname{Cl}_\Gamma(\gamma)}
=\operatorname{Cl}_{\widehat\Gamma}(\gamma)}.
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Suppose first that $\Gamma$ is [conjugacy separable](../../../group-theory.md#conjugacy-separable-group). If $h\in\Gamma$ is not conjugate to $\gamma$ in $\Gamma$, some homomorphism to a [finite group](../../../group.md#finite-group) sends them to nonconjugate elements. This homomorphism factors through a finite quotient of $\widehat\Gamma$, so $h$ cannot be conjugate to $\gamma$ in $\widehat\Gamma$. Thus

$$
\operatorname{Cl}_{\widehat\Gamma}(\gamma)\cap\Gamma
=\operatorname{Cl}_\Gamma(\gamma).
$$

Conversely, suppose this equality holds and $h$ is not conjugate to $\gamma$ in $\Gamma$. Then they are not conjugate in $\widehat\Gamma$. By the [finite-quotient criterion for conjugacy in a profinite group](../../../topological-group.md#finite-quotient-criterion-for-conjugacy-in-a-profinite-group), their images fail to be conjugate in some finite quotient. This is precisely conjugacy separability.

## 2

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A subset $S\subseteq G$ [topologically generates](../../../topological-group.md#topological-generating-set) $G$ exactly when

$$
\langle p_j(S)\rangle=p_j(G)
$$

for every $j$. In the usual presentation by surjective finite quotients this reads $\langle p_j(S)\rangle=G_j$. Indeed, a subgroup is dense exactly when its image in every finite discrete quotient is the whole quotient. This is the [finite-quotient criterion for topological generation](../../../topological-group.md#finite-quotient-criterion-for-topological-generation).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Apply part i to

$$
\mathbb Z_p=\varprojlim_n\mathbb Z/p^n\mathbb Z.
$$

The element $\alpha$ generates the additive cyclic group $\mathbb Z/p^n\mathbb Z$ exactly when it is coprime to $p$, which is equivalent to its reduction modulo $p$ being nonzero. Hence $\{\alpha\}$ is a [topological generating set](../../../topological-group.md#topological-generating-set) of the additive group $\mathbb Z_p$ if and only if $\alpha\not\equiv0\pmod p$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

An element of the [p-adic integers](../../../number-theory.md#p-adic-integer) is a [unit in a ring](../../../algebra.md#unit-in-a-ring) exactly when its reduction modulo $p$ is nonzero. More explicitly, if $\alpha\not\equiv0\pmod p$, its inverses modulo $p^n$ are unique and compatible, so they define $\beta\in\mathbb Z_p$ with $\alpha\beta=1$. The converse follows by reducing $\alpha\beta=1$ modulo $p$. Part ii therefore proves that $\alpha$ topologically generates the additive group if and only if $\alpha$ is a [p-adic unit](../../../arithmetic.md#p-adic-unit).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

By the [Fundamental theorem of finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups), write

$$
A\cong\mathbb Z^r\oplus F
$$

with $F$ finite. Taking [profinite completions](../../../topological-group.md#profinite-completion) gives

$$
\widehat A\cong\widehat{\mathbb Z}^{,r}\oplus F.
$$

If $A\cong\mathbb Z$, this is plainly $\widehat{\mathbb Z}$.

Conversely, suppose $\widehat A\cong\widehat{\mathbb Z}$. Reduction modulo a prime $p$ gives

$$
A/pA\cong(\mathbb Z/p\mathbb Z)^r\oplus F/pF,
$$

whereas $\widehat{\mathbb Z}/p\widehat{\mathbb Z}\cong\mathbb Z/p\mathbb Z$. Choosing $p\nmid|F|$ first shows $r=1$. If $F\ne0$, choosing a prime divisor $p$ of $|F|$ makes $F/pF\ne0$, a contradiction. Thus $F=0$ and $A\cong\mathbb Z$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Suppose $\widehat\Gamma\cong\mathbb Z_p$. This completion is an [abelian group](../../../group.md#abelian-group), so every finite quotient of $\Gamma$ is abelian. Consequently the quotient map to the [abelianization](../../../group-theory.md#abelianization) $A=\Gamma^{\mathrm{ab}}$ induces

$$
\widehat\Gamma\cong\widehat A.
$$

The group $A$ is a finitely generated [abelian group](../../../group.md#abelian-group). If its free rank is zero, $\widehat A=A$ is finite. If its free rank is positive, $A$ and hence $\widehat A$ have a nontrivial quotient $\mathbb Z/q\mathbb Z$ for every sufficiently chosen prime $q$. But $\mathbb Z_p$ has no nontrivial finite quotient of order coprime to $p$. Both cases are impossible, so $\widehat\Gamma\not\cong\mathbb Z_p$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Every element of $A_{\neg p}$ can be written $m/n$ with $p\nmid n$. Since $n$ is a [p-adic unit](../../../arithmetic.md#p-adic-unit), define

$$
\iota_p:A_{\neg p}\longrightarrow\mathbb Z_p,
\qquad \frac mn\longmapsto m n^{-1}.
$$

This is the restriction of the standard embedding $\mathbb Q\hookrightarrow\mathbb Q_p$, so it is an injective [group homomorphism](../../../group-theory.md#group-homomorphism). Equivalently, if $mn^{-1}=0$ in $\mathbb Z_p$, then $m=0$ because the [characteristic](../../../algebra.md#characteristic-of-a-field) is zero.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

If $\pi$ omits a prime $p$, then $A_\pi\subseteq A_{\neg p}\subseteq\mathbb Z_p$ by part i. The reductions

$$
\mathbb Z_p\longrightarrow\mathbb Z/p^n\mathbb Z
$$

separate its nonzero elements, so their restrictions separate the elements of $A_\pi$. Thus $A_\pi$ is [residually finite](../../../group-theory.md#residually-finite-group). If $\pi$ contains every prime, then $A_\pi=\mathbb Q$, which has no nontrivial finite quotient because it is a [divisible group](../../../group.md#divisible-group).

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

Let $q\ne p$ and let $f:A_{\neg p}\to\mathbb Z/q\mathbb Z$ be a homomorphism. Since $q$ is inverted in $A_{\neg p}$, every $x$ has the form $x=qy$. Therefore

$$
f(x)=qf(y)=0.
$$

**Hence the only such homomorphism is trivial.**

<h4 id="2/c/iv">iv</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/c/iv)

Every finite quotient of the abelian group $A_{\neg p}$ is abelian. Part iii excludes elements of prime order $q\ne p$ by the [Cauchy theorem for groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), so any finite quotient is a finite abelian $p$-group. If its exponent divides $p^n$, the quotient map kills $p^nA_{\neg p}$ and therefore factors through

$$
A_{\neg p}/p^nA_{\neg p}\cong\mathbb Z/p^n\mathbb Z.
$$

Every quotient of a [cyclic group](../../../group.md#cyclic-group) is cyclic, so the finite quotient is isomorphic to $\mathbb Z/p^k\mathbb Z$ for some $k\leq n$. Conversely, reduction modulo $p^k$ gives a surjection $A_{\neg p}\to\mathbb Z/p^k\mathbb Z$. Thus these are exactly the nontrivial finite quotients, together with the trivial case $k=0$.

## 3

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The quotient maps define a continuous homomorphism

$$
\Phi:G\longrightarrow\varprojlim_{U\in\mathcal U}G/U.
$$

Its kernel is $\bigcap_{U\in\mathcal U}U=\{1\}$, because $\mathcal U$ is a [neighborhood basis](../../../topology.md#neighbourhood-basis) and $G$ is [Hausdorff](../../../topology.md#hausdorff-space). Thus $\Phi$ is injective. The standard compactness argument for [inverse limits](../../../module-theory.md#inverse-limit) makes it surjective: a compatible family of cosets has the [finite intersection property](../../../topology.md#finite-intersection-property), and the corresponding closed cosets in compact $G$ have nonempty intersection. Finally, a continuous bijection from compact $G$ to the Hausdorff inverse limit is a [homeomorphism](../../../topology.md#homeomorphism). Hence

$$
G\cong\varprojlim_{U\in\mathcal U}G/U
$$

as [topological groups](../../../topological-group.md).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Suppose $G$ is topologically generated by $d$ elements. An open subgroup $H$ of index $n$ gives a continuous transitive [coset action](../../../group-theory.md#coset-action)

$$
G\longrightarrow S_n.
$$

A continuous homomorphism $G\to S_n$ is determined by the images of the $d$ topological generators, so there are at most $|S_n|^d$ such homomorphisms. Each has only finitely many point stabilizers. Therefore $G$ has only finitely many open subgroups of index $n$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

By part ii, $G_n$ is the intersection of finitely many open subgroups, so it is open. Conjugation permutes the subgroups of each index, hence $G_n$ is also a [normal subgroup](../../../group-theory.md#normal-subgroup). The groups $G_n$ form a descending family. If $U$ is any open normal subgroup and $[G:U]=m$, then $G_m\subseteq U$. Thus $(G_n)$ is cofinal among the open normal neighborhoods of the identity. Part i now gives

$$
\boxed{G\cong\varprojlim_nG/G_n}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

A [topological group](../../../topological-group.md) has the [topological Hopf property](../../../topological-group.md#topological-hopf-property) when every continuous surjective endomorphism is a topological automorphism.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Let $\phi:G\to G$ be a continuous surjective endomorphism. For each $n$, inverse image under $\phi$ permutes the finite set of open subgroups of index at most $n$: surjectivity preserves the index, and injectivity of the inverse-image operation follows from surjectivity. Hence

$$
\phi^{-1}(G_n)=G_n.
$$

If $x\in\ker\phi$, then $x\in G_n$ for every $n$. Part 3(a)(iii) implies $\bigcap_nG_n=\{1\}$, so $x=1$. Thus $\phi$ is bijective. A continuous bijection from compact $G$ to Hausdorff $G$ is a homeomorphism, proving the [Hopf property of a topologically finitely generated profinite group](../../../topological-group.md#hopf-property-of-a-topologically-finitely-generated-profinite-group).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

If $\gcd(m,|H|)=1$, choose $r$ with $mr\equiv1\pmod{|H|}$ by the [Bezout identity](../../../algebra.md#bezout-identity). The [Lagrange theorem](../../../group-theory.md#lagrange-s-theorem) gives $x^{|H|}=1$ for every $x\in H$, so $(x^m)^r=x$ and $(x^r)^m=x$. Thus $x\mapsto x^m$ is bijective, even though it need not be a homomorphism.

Conversely, if a prime $p$ divides both $m$ and $|H|$, the [Cauchy theorem for groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) gives $x\ne1$ with $x^p=1$. Then $x^m=1$, so the power map sends both $x$ and the identity to the identity and is not injective. This proves the [power-map criterion for a finite group](../../../finite-group-theory.md#power-map-criterion-for-a-finite-group).

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Necessity follows by applying $p_j$ to an equality $x^m=g$. Conversely, suppose every finite quotient contains an $m$th root of $p_j(g)$ and define

$$
X_j=\{x_j\in G_j:x_j^m=p_j(g)\}.
$$

These are nonempty finite sets, and the transition maps preserve them. The [nonemptiness theorem for inverse limits of finite sets](../../../module-theory.md#nonemptiness-theorem-for-inverse-limits-of-finite-sets) supplies a compatible tuple $x\in\varprojlim_jX_j=G$, for which $x^m=g$. This is the [finite-quotient criterion for roots in a profinite group](../../../topological-group.md#finite-quotient-criterion-for-roots-in-a-profinite-group).

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

If $m$ is coprime to every $|G_j|$, the [power-map criterion for a finite group](../../../finite-group-theory.md#power-map-criterion-for-a-finite-group) says that every finite-quotient power map is bijective. Part ii gives surjectivity of $f_m:G\to G$. If $x^m=y^m$, then $p_j(x)=p_j(y)$ for every $j$ by injectivity in $G_j$, and hence $x=y$. Thus the continuous power map is bijective.

## 4

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The inhomogeneous [group cochain](../../../group-theory.md#group-cochain) group is

$$
C^r(G,M)=\{f:G^r\to M\},
$$

with $C^0(G,M)=M$. Its [group coboundary](../../../group-theory.md#group-coboundary) $d:C^r(G,M)\to C^{r+1}(G,M)$ is

$$
(df)(g_1,\ldots,g_{r+1})
=g_1f(g_2,\ldots,g_{r+1})
+\sum_{i=1}^{r}(-1)^if(g_1,\ldots,g_ig_{i+1},\ldots,g_{r+1})
+(-1)^{r+1}f(g_1,\ldots,g_r).
$$

One checks that $d^2=0$, and [group cohomology](../../../group-theory.md#group-cohomology) is $H^r(G,M)=\ker d/\operatorname{im}d$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

A [crossed homomorphism](../../../group-theory.md#crossed-homomorphism) is a map $\phi:G\to M$ satisfying

$$
\phi(gh)=\phi(g)+g\phi(h).
$$

For a one-cochain, the formula in part i gives

$$
(d\phi)(g,h)=g\phi(h)-\phi(gh)+\phi(g),
$$

so the crossed homomorphisms are exactly the [one-cocycles](../../../group-theory.md#one-cocycle). A zero-cochain $m\in M$ has coboundary $g\mapsto gm-m$, the [principal crossed homomorphism](../../../group-theory.md#principal-crossed-homomorphism) associated with $m$. Therefore

$$
\boxed{H^1(G,M)=\frac{\{\text{crossed homomorphisms }G\to M\}}
{\{g\mapsto gm-m:m\in M\}}}.
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

For $g,h\in G$, substitute the definition of $\psi$ and in the first sum replace $\gamma$ by $\delta g$:

$$
\begin{aligned}
(d\psi)(g,h)
&=g\psi(h)-\psi(gh)+\psi(g)\\
&=\sum_{\delta\in G}\delta^{-1}
\bigl(\phi(\delta,g)+\phi(\delta g,h)-\phi(\delta,gh)\bigr).
\end{aligned}
$$

The [two-cocycle](../../../group-theory.md#two-cocycle) identity at $(\delta,g,h)$ says that the expression in parentheses is $\delta\phi(g,h)$. Every summand is therefore $\phi(g,h)$, and

$$
\boxed{d\psi=|G|\phi}.
$$

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

Let $\phi\in Z^2(G,\mathbb Q)$. Part iii gives $d\psi=|G|\phi$. Since division by $|G|$ is possible in the [rational numbers](../../../number-theory.md#rational-number),

$$
\phi=d\left(\frac{\psi}{|G|}\right)
$$

is a [two-coboundary](../../../group-theory.md#group-coboundary). Hence

$$
\boxed{H^2(G,\mathbb Q)=0}.
$$

This is a degree-two instance of the vanishing of finite-group cohomology when the group order is invertible on the coefficient module.

<h4 id="4/a/v">v</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/v/solution">Solution</h5>

↑ **Parent:** [V](#4/a/v)

For the trivial action, crossed homomorphisms $G\to\mathbb Q$ are ordinary [group homomorphisms](../../../group-theory.md#group-homomorphism), while principal crossed homomorphisms vanish. The image of a finite group in the torsion-free additive group $\mathbb Q$ must be trivial, so

$$
\boxed{H^1(G,\mathbb Q)=0}.
$$

Degree-zero cohomology is the [invariant submodule](../../../module-theory.md#invariant-submodule); the action is trivial, so

$$
\boxed{H^0(G,\mathbb Q)=\mathbb Q}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

The [short exact sequence](../../../module-theory.md#short-exact-sequence) of $G$-modules induces the [long exact sequence in group cohomology](../../../group-theory.md#long-exact-sequence-in-group-cohomology)

$$
0\to H^0(G,M_1)\to H^0(G,M_2)\to H^0(G,M_3)
\xrightarrow{\delta}H^1(G,M_1)\to H^1(G,M_2)\to\cdots.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Apply part i to the short exact sequence of trivial $G$-modules

$$
0\longrightarrow\mathbb Z\longrightarrow\mathbb Q
\longrightarrow\mathbb Q/\mathbb Z\longrightarrow0.
$$

The relevant segment is

$$
H^1(G,\mathbb Q)\longrightarrow H^1(G,\mathbb Q/\mathbb Z)
\xrightarrow{\delta}H^2(G,\mathbb Z)
\longrightarrow H^2(G,\mathbb Q).
$$

Both outer groups vanish by parts a(iv) and a(v), so the [connecting homomorphism](../../../homology.md#connecting-homomorphism) is an isomorphism:

$$
\boxed{H^2(G,\mathbb Z)\cong H^1(G,\mathbb Q/\mathbb Z)}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

The trivial action gives

$$
H^1(D_n,\mathbb Z)=\operatorname{Hom}(D_n,\mathbb Z)=0
$$

because $D_n$ is finite. By part b(ii),

$$
H^2(D_n,\mathbb Z)
\cong\operatorname{Hom}(D_n,\mathbb Q/\mathbb Z)
\cong\operatorname{Hom}(D_n^{\mathrm{ab}},\mathbb Q/\mathbb Z).
$$

In the [abelianization](../../../group-theory.md#abelianization) the relation $aba=b^{-1}$ becomes $b=b^{-1}$. Hence

$$
D_n^{\mathrm{ab}}\cong
\begin{cases}
C_2,&n\text{ odd},\\
C_2\times C_2,&n\text{ even}.
\end{cases}
$$

Each finite cyclic group is naturally isomorphic to its character group in $\mathbb Q/\mathbb Z$, so

$$
\boxed{H^2(D_n,\mathbb Z)\cong
\begin{cases}
\mathbb Z/2\mathbb Z,&n\text{ odd},\\
(\mathbb Z/2\mathbb Z)^2,&n\text{ even}.
\end{cases}}
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Write every element as $a^kb^l$ with $k\in\{0,1\}$. The action of this element on $M=\mathbb Z$ is multiplication by $(-1)^k$. A direct check of the four possibilities for the two exponents of $a$ shows

$$
\phi(xy)=\phi(x)+x\phi(y),
$$

so $\phi$ is a [crossed homomorphism](../../../group-theory.md#crossed-homomorphism) and hence a [one-cocycle](../../../group-theory.md#one-cocycle).

It cannot be principal: if $\phi(g)=gm-m$ for some $m\in\mathbb Z$, then at $g=a$ one would have

$$
1=\phi(a)=a m-m=-2m,
$$

which is impossible in the [integers](../../../number-theory.md#integer). Thus $[\phi]\ne0$ and

$$
\boxed{H^1(D_n,M)\ne0}.
$$

## 5

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Choose a normalized set-theoretic section $s:H\to E$ of $\pi$, so $s(1)=1$. Define the [extension cocycle](../../../group-theory.md#extension-cocycle)

$$
\phi(h,k)=s(h)s(k)s(hk)^{-1}\in M.
$$

Associativity of $s(h)s(k)s(l)$ gives, in multiplicative notation for $M$,

$$
\phi(h,k)\phi(hk,l)
=(h\cdot\phi(k,l))\phi(h,kl),
$$

which is exactly the [two-cocycle](../../../group-theory.md#two-cocycle) identity. Thus $\phi$ represents the class of the [group extension](../../../group-theory.md#group-extension) in $H^2(H,M)$.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

The [fiber product of groups](../../../group-theory.md#fiber-product-of-groups)

$$
E'=E\times_HG=\{(e,g)\in E\times G:\pi(e)=f(g)\}
$$

is a group under componentwise multiplication. The maps $m\mapsto(m,1)$ and $(e,g)\mapsto g$ give an exact sequence

$$
1\longrightarrow M\longrightarrow E'\longrightarrow G\longrightarrow1.
$$

The section $g\mapsto(s(f(g)),g)$ has extension cocycle

$$
(g,h)\longmapsto\phi(f(g),f(h))=(f^*\phi)(g,h).
$$

**Therefore this pullback extension represents $f^*([\phi])\in H^2(G,M)$.**

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Assume $f$ is injective. If two elements $(e,g),(e',g')\in E'$ have the same image under the first projection $E'\to E$, then $e=e'$. Applying $\pi$ gives $f(g)=f(g')$, so injectivity of $f$ gives $g=g'$. Hence the natural map $E'\to E$ is injective.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For every open normal subgroup $U\triangleleft G$, the composite

$$
\Gamma\xrightarrow{f}G\longrightarrow G/U
$$

has finite image and therefore factors uniquely through the [profinite completion](../../../topological-group.md#profinite-completion) $\widehat\Gamma$. These factor maps are compatible as $U$ varies. The [universal property of an inverse limit](../../../module-theory.md#universal-property-of-an-inverse-limit) consequently produces a continuous homomorphism

$$
\widehat f:\widehat\Gamma\longrightarrow
\varprojlim_U G/U\cong G
$$

with $\widehat f\iota=f$. It is unique because $\iota(\Gamma)$ is dense in $\widehat\Gamma$ and two continuous maps into the Hausdorff group $G$ that agree on a dense subset agree everywhere. This is the [universal property of profinite completion](../../../topological-group.md#universal-property-of-profinite-completion).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Choose $\widehat\zeta\in H^2(\widehat\Gamma,M)$ with $\iota^*(\widehat\zeta)=\zeta$, and let

$$
1\longrightarrow M\longrightarrow E\longrightarrow\widehat\Gamma\longrightarrow1
$$

be its extension. By the given fact, $E$ is a [profinite group](../../../topological-group.md#profinite-group), hence is [residually finite](../../../group-theory.md#residually-finite-group). The extension $E'_\zeta$ over $\Gamma$ is the pullback of $E$ along the injective map $\iota$. Part 5(a)(iii) embeds $E'_\zeta$ into $E$. Since every [subgroup of a residually finite group](../../../group-theory.md#subgroup-of-a-residually-finite-group) is residually finite, so is $E'_\zeta$.

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

Let $\widehat\zeta\in H^2(\widehat\Gamma,M)$ lie in the kernel of $\iota^*$, and represent it by a profinite extension

$$
1\longrightarrow M\longrightarrow E\xrightarrow{\pi}\widehat\Gamma\longrightarrow1.
$$

Its pullback to $\Gamma$ is split, so there is a homomorphism $s:\Gamma\to E$ satisfying $\pi s=\iota$. By part b, $s$ extends uniquely to a continuous homomorphism $\widehat s:\widehat\Gamma\to E$. The continuous maps $\pi\widehat s$ and the identity of $\widehat\Gamma$ agree on the dense image of $\Gamma$, hence agree everywhere. Thus $\widehat s$ is a section of $\pi$, the extension splits, and $\widehat\zeta=0$. Therefore

$$
\boxed{\iota^*:H^2(\widehat\Gamma,M)\longrightarrow H^2(\Gamma,M)\text{ is injective}}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
