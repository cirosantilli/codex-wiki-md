# Paper 5

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper5.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper5.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [topological group](../../../topological-group.md) is a [group](../../../group.md) equipped with a [topology](../../../topology.md) for which multiplication $G\times G\to G$ and inversion $G\to G$ are [continuous maps](../../../topology.md#continuous-map). The product uses the [product topology](../../../geometry-and-topology.md#product-topology). Translation and inversion are therefore [homeomorphisms](../../../topology.md#homeomorphism). Hausdorffness is sometimes included in the definition; the two open-subgroup arguments below do not require it.

For the [inverse system](../../../module-theory.md#inverse-system), take a [directed set](../../../set.md#directed-set) $I$, [topological spaces](../../../topology.md#topological-space) $X_i$, and [continuous maps](../../../topology.md#continuous-map) $f_{ij}:X_j\to X_i$ for $i\leq j$, with $f_{ii}=\mathrm{id}$ and $f_{ik}=f_{ij}f_{jk}$. An [inverse limit](../../../module-theory.md#inverse-limit) is a space $X$ with compatible [continuous maps](../../../topology.md#continuous-map) $\pi_i:X\to X_i$ such that every compatible family $q_i:Y\to X_i$ factors uniquely as $q_i=\pi_iq$ through a [continuous map](../../../topology.md#continuous-map) $q:Y\to X$. Existence follows from the concrete construction

$$
X=\left\{(x_i)\in\prod_{i\in I}X_i:f_{ij}(x_j)=x_i\text{ whenever }i\leq j\right\},
$$

with the subspace [topology](../../../topology.md) of the [product topology](../../../geometry-and-topology.md#product-topology). The only possible map $q$ is $q(y)=(q_i(y))_i$. Compatibility puts its image in $X$, and coordinatewise continuity makes it continuous. This proves the [universal property of an inverse limit](../../../module-theory.md#universal-property-of-an-inverse-limit), even when $X$ is empty. Given two [inverse limits](../../../module-theory.md#inverse-limit), their universal properties supply maps each way; the composites have the same coordinates as the identity, so uniqueness makes them identities. **The inverse limit exists and is unique up to the unique homeomorphism respecting its projections.**

A [profinite group](../../../topological-group.md#profinite-group) can be defined as an [inverse limit](../../../module-theory.md#inverse-limit) of finite discrete [groups](../../../group.md), or as a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) that is a [totally disconnected space](../../../arithmetic.md#totally-disconnected-space), equipped with continuous [group](../../../group.md) operations. For the first implication, use the [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem). The compatibility equalities define a closed [subgroup](../../../group.md#subgroup) of the compact Hausdorff product. Two distinct points are distinguished by a finite discrete coordinate, so no connected subset contains both. Consequently the [inverse limit](../../../module-theory.md#inverse-limit) is a compact Hausdorff totally disconnected [topological group](../../../topological-group.md).

For the converse, use the topological result that a compact Hausdorff totally disconnected space has a basis of [clopen sets](../../../topology.md#clopen-set). Choose a [clopen set](../../../topology.md#clopen-set) $U$ containing $1$ inside any specified identity neighbourhood. For each $u\in U$, continuity gives an identity neighbourhood $V_u$ and an open neighbourhood $W_u$ of $u$ with $V_uW_u\subseteq U$. Finitely many $W_u$ cover the [compact set](../../../topology.md#compact-space) $U$. Intersect their $V_u$ and its inverse to obtain a symmetric identity neighbourhood $V$ with $VU\subseteq U$. Symmetry also gives $V^{-1}U\subseteq U$, and hence $vU=U$ for every $v\in V$. The set

$$
H=\{g\in G:gU=U\}
$$

is a [subgroup](../../../group.md#subgroup) containing $V$, so it is open. It is contained in $U$, since $1\in U$ and $h=h\cdot1\in hU=U$. By part (ii), $H$ has finite index. Its [normal core of a subgroup](../../../group-theory.md#core-group-theory) is a finite intersection of conjugates of $H$, hence an open [normal subgroup](../../../group-theory.md#normal-subgroup) $N$ contained in $U$. This proves the [open normal subgroup basis of a profinite group](../../../topological-group.md#open-normal-subgroup-basis-of-a-profinite-group).

The natural [group homomorphism](../../../group-theory.md#group-homomorphism)

$$
G\longrightarrow\varprojlim_{N\trianglelefteq_oG}G/N
$$

is injective because the intersection of these $N$ is $\{1\}$. For a compatible family of cosets, any finitely many have nonempty intersection: their intersection subgroup is another indexing subgroup, and its prescribed coset lies in each. The [finite intersection property](../../../topology.md#finite-intersection-property) and compactness give a point belonging to all the cosets, proving surjectivity. Finally a continuous bijection from a [compact space](../../../topology.md#compact-space) to a [Hausdorff space](../../../topology.md#hausdorff-space) is a [homeomorphism](../../../topology.md#homeomorphism). **The two definitions of profinite group are equivalent.**

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

If $H$ is an open [subgroup](../../../group.md#subgroup) of a [topological group](../../../topological-group.md), each [coset](../../../group-theory.md#coset) $gH$ is open because translation is a [homeomorphism](../../../topology.md#homeomorphism). Distinct [cosets](../../../group-theory.md#coset) partition the [group](../../../group.md), so

$$
G\setminus H=\bigcup_{gH\ne H}gH
$$

is open. **Every open subgroup is closed.**

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [cosets](../../../group-theory.md#coset) of an open [subgroup](../../../group.md#subgroup) $H$ form an open cover of the [compact space](../../../topology.md#compact-space) $G$. A finite subcover exists. Since distinct [cosets](../../../group-theory.md#coset) are disjoint, that subcover must contain every [coset](../../../group-theory.md#coset). Thus **$[G:H]$ is finite**. Neither normality nor Hausdorffness is needed for this argument.

## 2

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [profinite group](../../../topological-group.md#profinite-group), its [profinite Frattini subgroup](../../../topological-group.md#profinite-frattini-subgroup) is

$$
\Phi(G)=\bigcap\{M:M\text{ is a maximal proper open subgroup of }G\}.
$$

Use $G$ for an empty intersection. This is a closed [normal subgroup](../../../group-theory.md#normal-subgroup), invariant under continuous [group automorphisms](../../../algebra.md#group-automorphism), since these automorphisms permute the maximal open [subgroups](../../../group.md#subgroup). Let $H=\overline{\langle X\rangle}$. If $H=G$, its image certainly topologically generates $G/\Phi(G)$. Conversely, suppose $H\ne G$. For $g\notin H$, the [open normal subgroup basis of a profinite group](../../../topological-group.md#open-normal-subgroup-basis-of-a-profinite-group) gives $N\trianglelefteq_oG$ with $g\notin HN$: choose a sufficiently small neighbourhood $gN$ disjoint from the closed [subgroup](../../../group.md#subgroup) $H$. The proper [subgroup](../../../group.md#subgroup) $HN/N$ of the [finite group](../../../group.md#finite-group) $G/N$ lies in a maximal proper [subgroup](../../../group.md#subgroup). Its preimage $M$ is a maximal proper open [subgroup](../../../group.md#subgroup) of $G$, contains $H$, and contains $\Phi(G)$. Since $H\Phi(G)$ is compact and therefore closed, density of the image of $X$ in $G/\Phi(G)$ would force $H\Phi(G)=G$, contradicting $H\Phi(G)\leq M<G$. **Generation can therefore be tested modulo the profinite Frattini subgroup.**

For a [finite p-group](../../../finite-group-theory.md#finite-p-group), every maximal proper [subgroup](../../../group.md#subgroup) is normal and has index $p$. One proof uses the [normalizer condition for finite p-groups](../../../finite-group-theory.md#normalizer-condition-for-finite-p-groups): maximality forces its normalizer to be the whole [group](../../../group.md), and its simple $p$-group quotient has order $p$. Therefore every such maximal [subgroup](../../../group.md#subgroup) contains powers and [group commutators](../../../group.md#group-commutator). Conversely, the quotient by the algebraic $G^p[G,G]$ is an [elementary abelian p-group](../../../group.md#elementary-abelian-group); its nonzero elements are separated by linear maps to $\mathbb F_p$. Their kernels give maximal [subgroups](../../../group.md#subgroup). This proves the finite [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) formula.

Now take a [pro-p group](../../../topological-group.md#pro-p-group) and put $D=\overline{G^p[G,G]}$, retaining the [closure](../../../topology.md#closure-topology) of the algebraically generated [subgroups](../../../group.md#subgroup). A maximal open [subgroup](../../../group.md#subgroup) is the preimage of a maximal [subgroup](../../../group.md#subgroup) of a finite $p$-group quotient, so it contains $D$. If $g\notin D$, some finite quotient of the [profinite group](../../../topological-group.md#profinite-group) $G/D$ detects $gD$. That quotient is [elementary abelian](../../../group.md#elementary-abelian-group), and a linear functional nonzero at $gD$ gives a continuous [group homomorphism](../../../group-theory.md#group-homomorphism) $G\to\mathbb F_p$ whose kernel is a maximal open [subgroup](../../../group.md#subgroup) missing $g$. Hence

$$
\boxed{\Phi(G)=\overline{G^p[G,G]}.}
$$

The [closure](../../../topology.md#closure-topology) bar is present in the original PDF; the converted TeX fraction is an extraction error.

For the finite-index assertion, first pass from the arbitrary abstract [subgroup](../../../group.md#subgroup) $K$ to its [normal core of a subgroup](../../../group-theory.md#core-group-theory) $C$. The action on the finitely many [cosets](../../../group-theory.md#coset) of $K$ shows $[G:C]<\infty$, without assuming that $K$ or $C$ is closed. Write $m=[G:C]=p^rq$ with $(p,q)=1$, and let $X_m=\{h^m:h\in G\}$. By [Lagrange theorem](../../../group-theory.md#lagrange-s-theorem), $X_m\subseteq C$. For $N\trianglelefteq_oG$, the quotient $G/N$ is a [finite p-group](../../../finite-group-theory.md#finite-p-group) of order, say, $p^s$. Choose an integer $a$ with $aq\equiv1\pmod {p^s}$. Then

$$
(g^a)^mN=g^{p^r}N,
$$

so $g^{p^r}\in X_mN$ for every such $N$. The set $X_m$ is the continuous image of the [compact space](../../../topology.md#compact-space) $G$, hence is closed. Consequently $g^{p^r}\in\bigcap_NX_mN=X_m\subseteq C$. Every element of the abstract finite quotient $G/C$ thus has order dividing $p^r$. By [Cauchy theorem for groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), no prime other than $p$ divides its order. Therefore $[G:C]$, and its divisor $[G:K]$, are powers of $p$. **This proof does not assume continuity of the finite quotient map.**

To prove openness under finite generation, first establish [commutator collection with fixed generators in nilpotent groups](../../../group-theory.md#commutator-collection-with-fixed-generators-in-nilpotent-groups). If a [nilpotent group](../../../group-theory.md#nilpotent-group) $P$ is generated by $a_1,\ldots,a_d$, every element of $P\prime$ is

$$
[x_1,a_1]\cdots[x_d,a_d].
$$

Induct on the nilpotency class $c$. The assertion is trivial for $c=1$. Apply the induction hypothesis in $P/\gamma_c(P)$; the remaining error lies in the central [subgroup](../../../group.md#subgroup) $\gamma_c(P)=[\gamma_{c-1}(P),P]$. Since commutators in this last layer are central, collecting against words in the $a_i$ expresses the error as $\prod_i[y_i,a_i]$ with $y_i\in\gamma_{c-1}(P)$. Also $[P\prime,\gamma_{c-1}(P)]\leq\gamma_{c+1}(P)=1$. Thus replacing each $x_i$ by $x_iy_i$ multiplies the desired product by precisely that central error, proving the formula.

Let $a_1,\ldots,a_d$ now topologically generate $G$. Every finite continuous quotient is a [nilpotent group](../../../group-theory.md#nilpotent-group), so the formula holds there with these fixed generators. For $z\in\overline{[G,G]}$, the sets of tuples $(x_1,\ldots,x_d)\in G^d$ solving $z\equiv\prod_i[x_i,a_i]\pmod N$ are nonempty closed subsets of a [compact space](../../../topology.md#compact-space). They have the [finite intersection property](../../../topology.md#finite-intersection-property), by replacing finitely many $N$ by their intersection. A common tuple solves the equality in $G$. It follows that the algebraic [commutator subgroup](../../../group-theory.md#commutator-subgroup) is the compact image of $G^d$ under this product map, and is closed.

Its quotient $A=G/[G,G]$ is a topologically finitely generated abelian [pro-p group](../../../topological-group.md#pro-p-group). The continuous map $\mathbb Z_p^d\to A$ taking $(\lambda_i)$ to $\prod_i\bar a_i^{\lambda_i}$ is onto, because its compact image contains a dense generating [subgroup](../../../group.md#subgroup). Therefore $A/pA$ is generated as an [elementary abelian group](../../../group.md#elementary-abelian-group) by at most $d$ elements, and $pA$ is compact. The preimage $G^p[G,G]$ of $pA$ is closed of finite index, hence open: its complement is a finite union of closed [cosets](../../../group-theory.md#coset). The finite-index result and the maximal-subgroup property of [finite p-groups](../../../finite-group-theory.md#finite-p-group) show that any abstract index-$p$ [subgroup](../../../group.md#subgroup) of $G$ is normal. It contains this open [subgroup](../../../group.md#subgroup), so is itself open.

Finally, a finite-index normal [subgroup](../../../group.md#subgroup) $C$ has finite $p$-group quotient. If $[G:C]>1$, choose a normal index-$p$ [subgroup](../../../group.md#subgroup) in that quotient and call its preimage $H$. The preceding argument makes $H$ open. An open [subgroup](../../../group.md#subgroup) of a finitely generated [pro-p group](../../../topological-group.md#pro-p-group) is finitely generated: intersect a finitely generated dense abstract [subgroup](../../../group.md#subgroup) with $H$, use the [Schreier lemma](../../../geometric-group-theory.md#reidemeister-schreier-theorem), and observe that the intersection is dense in the open [subgroup](../../../group.md#subgroup) $H$. Induction on $[G:C]$ now makes $C$ open in $H$, hence in $G$. Returning to the [normal core of a subgroup](../../../group-theory.md#core-group-theory), $K$ is a union of open [cosets](../../../group-theory.md#coset) of $C$. **Every finite-index subgroup of a finitely generated pro-p group is open.**

## 3

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Here $p$ is odd. For a [finite p-group](../../../finite-group-theory.md#finite-p-group), write $N^p=\langle n^p:n\in N\rangle$. A [powerfully embedded subgroup](../../../finite-group-theory.md#powerfully-embedded-subgroup) satisfies $[N,G]\leq N^p$; this also makes $N$ normal, since every conjugate of an element of $N$ differs from it by an element of $N$. A [powerful p-group](../../../finite-group-theory.md#powerful-p-group) is one with $[G,G]\leq G^p$, namely one powerfully embedded in itself. Use $[a,b]=a^{-1}b^{-1}ab$ and $a^b=b^{-1}ab$ throughout.

The [lower p-series](../../../finite-group-theory.md#lower-p-series) is defined by

$$
G_1=G,\qquad G_{i+1}=G_i^p[G_i,G].
$$

Each quotient $G_i/G_{i+1}$ is an [elementary abelian p-group](../../../group.md#elementary-abelian-group), and $[G_i,G]\leq G_{i+1}$. These are generated [subgroups](../../../group.md#subgroup), without closure bars, because the [group](../../../group.md) is finite.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Since $N$ is normal in $G$, it is normal in $H=\langle x,N\rangle$, and $H/N$ is a [cyclic group](../../../group.md#cyclic-group). More specifically, quotienting $H$ by $[N,H]$ makes the image of $N$ central. The quotient is generated by this central image and the single element $x$, and is therefore abelian. Hence

$$
[H,H]\leq[N,H]\leq[N,G]\leq N^p\leq H^p.
$$

**Thus $H$ is a powerful p-group.** Merely saying that $H/N$ is cyclic would give only $[H,H]\leq N$; centralizing $N$ is the extra step needed here.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [powerfully embedded subgroup](../../../finite-group-theory.md#powerfully-embedded-subgroup) $N$ is itself a [powerful p-group](../../../finite-group-theory.md#powerful-p-group), so the finite [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) formula gives $\Phi(N)=N^p$. [Conjugation](../../../group-theory.md#conjugation) by $G$ acts trivially on $N/N^p$, because $[N,G]\leq N^p$. Since $N$ is the [normal closure](../../../group-theory.md#normal-closure) of $X$, the image of $X$ therefore generates $N/N^p$: all conjugates have the same images as the original elements. The [Burnside basis theorem](../../../finite-group-theory.md#burnside-basis-theorem) now gives **$N=\langle X\rangle$**. Equivalently, a proper generated [subgroup](../../../group.md#subgroup) would lie in a maximal [subgroup](../../../group.md#subgroup) of $N$, which contains $N^p$ and contradicts generation of that quotient.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the allowed reduction $[N,G,G,G]=1$. Set $C=[N,G]$ and $D=[C,G]$. Then $[D,G]=1$, so $D$ is central. For $n\in N$ and $g\in G$, put $c=[n,g]$. The identity $[ab,g]=[a,g]^b[b,g]$ and centrality of $[c,n]\in D$ give, by induction on $k$,

$$
[n^k,g]=c^k[c,n]^{\binom{k}{2}}.
$$

At $k=p$, both factors belong to $C^p$: the first is a $p$th power in $C$, and the second is a $p$th power because $p\mid\binom p2$ and $[c,n]\in D\leq C$. The [subgroup](../../../group.md#subgroup) $C^p$ is normal in $G$. Commuting products of the generators $n^p$ with $g$ and using the same identity consequently yields

$$
[N^p,G]\leq C^p.
$$

Since $C=[N,G]\leq N^p$, it follows that $[C,G]\leq C^p$. **Thus $[N,G]$ is powerfully embedded.** This proves the reduced case, and the reduction permitted in the question gives the general assertion.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For a [powerful p-group](../../../finite-group-theory.md#powerful-p-group), $G_2=G^p$, and $G_3=(G^p)^p[G^p,G]$. In $G/G_3$, the image of $G_2$ is central and has exponent dividing $p$, while the [commutator subgroup](../../../group-theory.md#commutator-subgroup) is contained in that image. The quotient thus has nilpotency class at most two. Direct collection in such a [group](../../../group.md) gives

$$
(xy)^p=x^py^p[y,x]^{\binom p2}\equiv x^py^p\pmod {G_3},
$$

because $p$ is odd. If $z\in G_2$, the same calculation gives $(xz)^p\equiv x^p$ modulo $G_3$, since $z^p\in G_3$. Consequently the power map is well defined on $G/G_2$ and is a [group homomorphism](../../../group-theory.md#group-homomorphism) to $G_2/G_3$. Its image contains all the power generators of that quotient. **It is therefore surjective.**

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Set $P_0=G$ and $P_{i+1}=P_i^p$. The permitted power-embedding result, applied repeatedly, gives $[P_i,G]\leq P_{i+1}$, and each $P_i$ is a [powerful p-group](../../../finite-group-theory.md#powerful-p-group). These [subgroups](../../../group.md#subgroup) eventually reach $1$: if $P_i\ne1$, its [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) $P_i^p$ is proper. In fact these are the [lower p-series](../../../finite-group-theory.md#lower-p-series) layers, with their indices shifted by one.

For $x\in G$ and $y\in P_i$, the [commutator](../../../lie-algebra.md#commutator) $[y,x]$ lies in $P_{i+1}$, is central modulo $P_{i+2}$, and has exponent dividing $p$ there. The class-two collection calculation from part (iv) therefore gives

$$
(xy)^p\equiv x^py^p\pmod {P_{i+2}}.
$$

Applying part (iv) inside $P_i$, whose third lower-series term is contained in $P_{i+2}$, shows that the map $y\mapsto y^p$ is onto $P_{i+1}/P_{i+2}$.

Given $a\in P_1$, first choose $x$ with $x^p\equiv a\pmod {P_2}$. Suppose $x^p\equiv a\pmod {P_{i+1}}$. Choose $y\in P_i$ with $y^p\equiv x^{-p}a\pmod {P_{i+2}}$. The displayed collection congruence then gives $(xy)^p\equiv a\pmod {P_{i+2}}$. Replacing $x$ by $xy$ improves the approximation by one layer. Since the [filtration on a group](../../../associative-algebra.md#filtration-on-a-group) terminates, a finite sequence of corrections gives $x^p=a$ exactly. The reverse inclusion is the definition of $G^p$. Hence

$$
\boxed{G^p=G^{\{p\}}=\{x^p:x\in G\}.}
$$

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

Write $G=\langle a,b\rangle$ and $c=[a,b]$. The [commutator subgroup](../../../group-theory.md#commutator-subgroup) $G\prime$ is the [normal closure](../../../group-theory.md#normal-closure) of $c$: imposing $c=1$ makes the two generators commute, so the quotient is abelian. Part (iii), with $N=G$, makes $G\prime$ a [powerfully embedded subgroup](../../../finite-group-theory.md#powerfully-embedded-subgroup). Part (ii) therefore gives

$$
G\prime=\langle c\rangle.
$$

This proves the hint, but cyclicity of the [commutator subgroup](../../../group-theory.md#commutator-subgroup) alone is not yet the required cyclic normal subgroup with cyclic quotient.

If $c=1$, the [group](../../../group.md) is abelian and any one of the two generator subgroups is normal with cyclic quotient. Otherwise $c\in G^p$. Part (v) permits taking a $p$th root of $c$. Whenever the chosen root is still in $G^p$, take another $p$th root. The order increases by a factor $p$ at every step, since the power being rooted is nonidentity. Finiteness forces this process to stop. Thus

$$
c=d^{p^r},\qquad d\notin G^p=\Phi(G)
$$

for some $d$. The [cyclic subgroup](../../../group.md#cyclic-subgroup) $A=\langle d\rangle$ contains $G\prime$, and hence is normal: every conjugate of $d$ differs from $d$ by an element of $G\prime\leq A$. The nonzero image of $d$ in the [Frattini quotient](../../../finite-group-theory.md#frattini-quotient) can be completed to a basis of dimension at most two. By the [Burnside basis theorem](../../../finite-group-theory.md#burnside-basis-theorem), $G=\langle d,e\rangle$ for a suitable $e$; if the quotient has dimension one, $d$ already generates $G$. Therefore $G/A$ is cyclic. **The powerful two-generator finite p-group is metacyclic.**

## 4

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The correspondence concerns [uniform pro-p groups](../../../topological-group.md#uniform-pro-p-group) and [powerful Lie lattices](../../../lie-algebra.md#powerful-lie-algebra-over-p-adic-integers), with their natural morphisms. Put $\epsilon=1$ for odd $p$ and $\epsilon=2$ for $p=2$. A [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group) is a [pro-p group](../../../topological-group.md#pro-p-group) whose closed [commutator subgroup](../../../group-theory.md#commutator-subgroup) lies in its closed $p^\epsilon$-power [subgroup](../../../group.md#subgroup). It is uniform when it is topologically finitely generated and all successive indices in its [lower p-series](../../../finite-group-theory.md#lower-p-series) are equal. Equivalently, a finitely generated [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group) is uniform precisely when it is a [torsion-free group](../../../group.md#torsion-free-group). A [powerful Lie algebra over p-adic integers](../../../lie-algebra.md#powerful-lie-algebra-over-p-adic-integers) means a [Lie algebra](../../../lie-algebra.md) over $\mathbb Z_p$ that is free of finite rank as a [module](../../../module-theory.md#module-mathematics) and satisfies

$$
[L,L]\subseteq p^\epsilon L.
$$

Here a [Lie algebra](../../../lie-algebra.md) over a ring is a [module](../../../module-theory.md#module-mathematics) with an alternating bilinear [Lie bracket](../../../lie-algebra.md#lie-bracket) satisfying the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Finite freeness is an essential part of the lattice convention. The zero-bracket [module](../../../module-theory.md#module-mathematics) $\mathbb F_p$ satisfies the bracket inclusion but has torsion, and its additive [group](../../../group.md) is not uniform. Thus allowing arbitrary torsion modules would make the categorical assertion false.

The basic structural facts behind the construction can be seen from the power layers. Write $P_n=G^{p^n}$ with $P_0=G$. Collection for a [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group) gives

$$
[P_r,P_s]\subseteq P_{r+s+\epsilon},\qquad P_n=\{g^{p^n}:g\in G\}.
$$

For odd $p$, the power lifting is exactly the successive-correction argument of Question 3, followed by compactness; at $p=2$ the stronger fourth-power commutator condition makes the corresponding collection corrections work. The maps between successive layers are surjective linear maps. Uniformity makes their finite dimensions equal, so these maps are isomorphisms. Comparing the first layer in which two elements differ now shows that the power map $P_n\to P_{n+1}$ is injective, while the power-set formula makes it surjective. Thus all the roots used below exist uniquely in the indicated layer. If $g_1,\ldots,g_d$ lift a basis of $G/P_1$, the images of $g_i^{p^n}$ form a basis of $P_n/P_{n+1}$. Successively choosing their coefficients modulo $p$ gives the unique ordered expression

$$
g=g_1^{\lambda_1}\cdots g_d^{\lambda_d},\qquad \lambda_i\in\mathbb Z_p.
$$

Existence follows by lifting one layer at a time and taking a limit; uniqueness follows by comparing the first nonzero coefficient layer. In particular $[G:P_n]=p^{nd}$ and these layers form a neighbourhood basis. These are the power-layer and coordinate facts needed in the proof, rather than an assumption that an arbitrary [pro-p group](../../../topological-group.md#pro-p-group) has unique roots.

On the underlying set of $G$, set the additive zero to $1$, the additive negative of $x$ to $x^{-1}$, and define

$$
\lambda\cdot_Lx=x^\lambda,\qquad
x+_Ly=\lim_{n\to\infty}(x^{p^n}y^{p^n})^{p^{-n}},\qquad
[x,y]_L=\lim_{n\to\infty}[x^{p^n},y^{p^n}]^{p^{-2n}}.
$$

The [p-adic integers](../../../number-theory.md#p-adic-integer) act through limits of integer powers in the closed [cyclic subgroup](../../../group.md#cyclic-subgroup) generated by $x$. In the second formula the product belongs to $P_n$; in the third the [group commutator](../../../group.md#group-commutator) belongs to $P_{2n+\epsilon}$. The symbols $p^{-n}$ and $p^{-2n}$ denote the unique group roots, not unrestricted division in a [group](../../../group.md). We next justify convergence and the [Lie algebra](../../../lie-algebra.md) laws together.

A useful concrete tool is a complete normed [group algebra](../../../associative-algebra.md#group-algebra) containing $G$. In its [completed group algebra](../../../associative-algebra.md#completed-group-algebra), put $b_i=g_i-1$. Ordered-coordinate uniqueness gives unique expansions $\sum_{\alpha\in\mathbb N^d}c_\alpha b_1^{\alpha_1}\cdots b_d^{\alpha_d}$ with $c_\alpha\in\mathbb Z_p$. To see why, first work modulo $p$ and $P_n$: the ordered products of the $g_i$ with exponents below $p^n$ form the regular basis, and the change to the corresponding products of $g_i-1$ is triangular with diagonal entries one. Take inverse limits and then lift the coefficient digits successively in powers of $p$. Define the weight

$$
v\left(\sum_\alpha c_\alpha b^\alpha\right)=\inf_\alpha\{v_p(c_\alpha)+\epsilon|\alpha|\}.
$$

It is a genuine separated, submultiplicative weight. Indeed reordering $b_jb_i$ produces a group-commutator correction in $P_\epsilon$; the binomial expansion of a $p^\epsilon$th power gives that correction weight at least $2\epsilon$, so collection never decreases total weight. Also $v(pc)=1+v(c)$. Inverting $p$ and completing therefore gives a [Banach algebra](../../../banach-algebra.md) $B$ over $\mathbb Q_p$. For $g\in G$, ordered coordinates show

$$
v(g-1)=\epsilon+\max\{n:g\in P_n\},
$$

with value infinity at $g=1$. Thus the induced [topology](../../../topology.md) on $G$ is exactly its original [topology](../../../topology.md). This construction supplies the ambient algebra without presupposing the [uniform pro-p group and powerful Lie lattice correspondence](../../../topological-group.md#uniform-pro-p-group-and-powerful-lie-lattice-correspondence). The weighted construction, including the case $p=2$, is described in [Equivariant D-modules on rigid analytic spaces, Section 6.5](https://smf.emath.fr/system/files/filepdf/smf_ast_423.pdf).

Since $\epsilon>1/(p-1)$, the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) and [p-adic exponential](../../../arithmetic.md#p-adic-exponential-function) converge on the relevant balls in $B$:

$$
\log(1+b)=\sum_{k\geq1}\frac{(-1)^{k+1}b^k}{k},\qquad
\exp(a)=\sum_{k\geq0}\frac{a^k}{k!}.
$$

The estimates $v_p(k!)\leq k/(p-1)$ and $v_p(k)\leq\log_p k$ show that term weights tend to infinity. Formal substitution is legitimate there and proves that the two maps are inverse. They preserve the leading weight. In particular $\log$ embeds the compact set $G$ homeomorphically into $B$, and $\log(g^{p^n})=p^n\log g$.

Put $a=\log x$ and $b=\log y$. Expanding the convergent [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) in $B$ gives

$$
p^{-n}\log(x^{p^n}y^{p^n})\longrightarrow a+b,\qquad
p^{-2n}\log([x^{p^n},y^{p^n}])\longrightarrow ab-ba.
$$

The first expansion has linear part $p^n(a+b)$ and all other terms have degree at least two in $p^na,p^nb$. The second has leading term $p^{2n}(ab-ba)$ and all remaining terms have degree at least three. After division by the displayed powers of $p$, the extra factor of $p^n$ forces those errors to zero. The normalized expressions are logarithms of the unique roots already specified. Since $\log G$ is compact and closed in $B$, both limits belong to $\log G$. Scalar multiplication also remains in $\log G$ by continuity of powers. Consequently $\log G$ is a [module](../../../module-theory.md#module-mathematics) over $\mathbb Z_p$, closed under the associative-algebra [Lie bracket](../../../lie-algebra.md#lie-bracket) $ab-ba$. Bilinearity, alternation and the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) follow by expanding products in the [associative algebra](../../../associative-algebra.md) $B$. Transporting these operations back gives exactly $L_G$ above.

The commutator-layer inclusion places every normalized bracket root in $P_\epsilon$. Since $\log P_\epsilon=p^\epsilon\log G$ and this set is compact, passage to the limit proves $[L_G,L_G]\subseteq p^\epsilon L_G$. Addition modulo $pL_G$ is the original multiplication modulo $P_1$: collection shows $(x^{p^n}y^{p^n})^{p^{-n}}\equiv xy\pmod {P_1}$, as the nonlinear errors lie at least one layer deeper. Thus $L_G/pL_G$ has dimension $d$, with basis $e_i=\log g_i$. Given $a\in\log G$, write its residue as $\sum_i\lambda_{0i}e_i$ and repeat on $(a-\sum_i\lambda_{0i}e_i)/p$. This iterative digit lifting converges because the remainders stay in the bounded compact set $\log G$. It gives $a=\sum_i\lambda_i e_i$ with $\lambda_i\in\mathbb Z_p$. A nontrivial relation among the $e_i$ could be divided by the smallest power of $p$ among its coefficients, contradicting their independence modulo $p$. Hence $L_G$ is free of rank $d$, proving that it is a [powerful Lie lattice](../../../lie-algebra.md#powerful-lie-algebra-over-p-adic-integers).

Conversely, let $L$ be a [powerful Lie lattice](../../../lie-algebra.md#powerful-lie-algebra-over-p-adic-integers). In $L\otimes_{\mathbb Z_p}\mathbb Q_p$, define

$$
x*y=\operatorname{BCH}(x,y)
=x+y+\frac12[x,y]+\frac1{12}\bigl([x,[x,y]]+[y,[y,x]]\bigr)+\cdots.
$$

The formal [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) and its coefficient estimate are the algebraic ingredients used here. More precisely, the degree-$m$ component can be expressed as an integral Lie polynomial divided by a number of $p$-adic valuation at most $\lfloor(m-1)/(p-1)\rfloor$. One way to obtain this estimate is to bound the associative coefficients of $\log(\exp X\exp Y)$ and use an integral ordered basis of the free [Lie algebra](../../../lie-algebra.md). The denominator bound $v_p(m!)+\lfloor\log_p s_p(m)\rfloor$, where $s_p(m)$ is the base-$p$ digit sum, is at most $\lfloor(m-1)/(p-1)\rfloor$. A precise primary reference for that denominator estimate is [Smallest common denominators for the homogeneous components of the Baker-Campbell-Hausdorff series](https://arxiv.org/abs/2012.03818). A length-$m$ [Lie bracket](../../../lie-algebra.md#lie-bracket) in $L$ lies in $p^{\epsilon(m-1)}L$. Thus the degree-$m$ term belongs to

$$
p^{\epsilon(m-1)-\lfloor(m-1)/(p-1)\rfloor}L.
$$

These exponents are nonnegative and tend to infinity; for $m\geq2$ they are at least one. This proves integral convergence, continuity and $x*y\equiv x+y\pmod {pL}$. Associativity follows from the formal identity $\exp(\operatorname{BCH}(X,Y))=\exp X\exp Y$ in the completed [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra). Substitution of three elements is justified by the same valuation estimates, so the two associative expressions agree. The identity is $0$, the inverse is $-x$, and $x^{*k}=kx$ because every nonlinear term involving only $x$ vanishes.

For powerfulness, formal conjugation gives

$$
\exp(-x)\exp(-y)\exp(x)=\exp(-e^{-\operatorname{ad}x}y).
$$

The difference $\delta=y-e^{-\operatorname{ad}x}y$ lies in $p^\epsilon L$: its $k$th term has valuation at least $k\epsilon-v_p(k!)\geq\epsilon$ for $k\geq1$. The group [commutator](../../../lie-algebra.md#commutator) is therefore $(-y+\delta)*y$. Its linear term is $\delta$. Every nonlinear Lie term contains $\delta$, since it vanishes when $\delta=0$, and the extra divisibility makes all those terms lie in $p^\epsilon L$ too. Hence $[(L,*),(L,*)]\subseteq p^\epsilon L$. The ideals $p^nL$ are open normal [subgroups](../../../group.md#subgroup) for $*$, and their finite quotients have order $p^{nd}$. The [group](../../../group.md) is consequently a [pro-p group](../../../topological-group.md#pro-p-group). Its power sets are exactly $p^nL$, its lower-series indices are constantly $p^d$, and a basis of $L$ topologically generates it by the same successive digit lifting. **The BCH group $(L,*)$ is uniform.**

To check the inverse constructions, powers in the [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) group are ordinary multiples in $L$. Therefore

$$
p^{-n}\operatorname{BCH}(p^nx,p^ny)\longrightarrow x+y,
$$

and the similarly normalized [group commutator](../../../group.md#group-commutator) tends to $[x,y]$. The limit constructions recover the original [Lie algebra](../../../lie-algebra.md) exactly. In the other direction, the ambient [Banach algebra](../../../banach-algebra.md) construction gives $\log(xy)=\operatorname{BCH}(\log x,\log y)$, so the recovered operation is the original multiplication of $G$.

Finally a continuous [group homomorphism](../../../group-theory.md#group-homomorphism) between [uniform pro-p groups](../../../topological-group.md#uniform-pro-p-group) preserves integer powers and powers with exponents in the [p-adic integers](../../../number-theory.md#p-adic-integer), preserves the unique roots in the power layers, and commutes with their limits. It therefore becomes a linear [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism). Conversely a linear [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism) between finite free [modules](../../../module-theory.md#module-mathematics) is continuous and preserves every term of the convergent [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula), hence is a continuous [group homomorphism](../../../group-theory.md#group-homomorphism) for $*$. The constructions preserve identity maps and composition, and the inverse identifications are natural. **They are mutually inverse functors, giving the stated category correspondence with the finite-free lattice convention.**

## 5

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [topological group module](../../../module-theory.md#topological-group-module) $A$ is a topological [abelian group](../../../group.md#abelian-group) with a jointly continuous action of $G$ by [group automorphisms](../../../algebra.md#group-automorphism). Its [continuous cochains with topological coefficients](../../../group-theory.md#continuous-cochains-with-topological-coefficients) are

$$
C^0(G,A)=A,\qquad C^n(G,A)=\operatorname{Cont}(G^n,A)\quad(n\geq1),
$$

with pointwise addition. The inhomogeneous differential is

$$
\begin{aligned}
(dc)(g_1,\ldots,g_{n+1})={}&g_1c(g_2,\ldots,g_{n+1})\\
&+\sum_{i=1}^n(-1)^ic(g_1,\ldots,g_ig_{i+1},\ldots,g_{n+1})\\
&+(-1)^{n+1}c(g_1,\ldots,g_n).
\end{aligned}
$$

For $n=0$, this means $(da)(g)=ga-a$. Continuity of multiplication and of the action ensures that $d$ preserves continuous cochains. Expanding $d(dc)$ gives cancellation in pairs: the two orders of multiplying neighbouring arguments agree by associativity, and the two ways of applying the action agree by its action law. Thus $d^2=0$. The [cocycles](../../../algebra.md#cocycle) are $Z^n=\ker(d:C^n\to C^{n+1})$ and the [coboundaries](../../../algebra.md#coboundary) are $B^n=\operatorname{im}(d:C^{n-1}\to C^n)$, with $B^0=0$. Define

$$
\boxed{H^n(G,A)=Z^n(G,A)/B^n(G,A).}
$$

For general topological coefficients this is an algebraic quotient of the continuous cochains; its optional quotient [topology](../../../topology.md) need not be Hausdorff. For discrete coefficients it is the usual [continuous cohomology of a profinite group](../../../group-theory.md#continuous-cohomology-of-a-profinite-group). In degree zero it is the subgroup of invariant elements.

Give the discrete [prime field](../../../algebra.md#prime-field) $\mathbb F_p$ its trivial $G$-action. The one-cocycle condition becomes $c(gh)=c(g)+c(h)$ and every one-coboundary is zero. Hence

$$
H^1(G,\mathbb F_p)=\operatorname{Hom}_{\mathrm{cont}}(G,\mathbb F_p)
=\operatorname{Hom}_{\mathrm{cont}}(G/\Phi(G),\mathbb F_p).
$$

Every such [group homomorphism](../../../group-theory.md#group-homomorphism) kills powers and [group commutators](../../../group.md#group-commutator), hence their [closure](../../../topology.md#closure-topology) $\Phi(G)$, and every continuous functional on the quotient pulls back. If $G$ is topologically finitely generated, $V=G/\Phi(G)$ is a finite [elementary abelian group](../../../group.md#elementary-abelian-group). To verify finiteness without assuming it, the [closure](../../../topology.md#closure-topology) of a subgroup generated by $r$ elements of this abelian exponent-$p$ quotient has at most $p^r$ elements; a finite subgroup is already closed. Thus $V$ is a finite-dimensional [vector space](../../../vector-space.md). Question 2 says that a generating family of $G$ is minimal precisely when its images give a basis of $V$. The [dual space](../../../linear-algebra.md#dual-space) has the same finite dimension. This proves

$$
\boxed{d(G)=\dim_{\mathbb F_p}H^1(G,\mathbb F_p)\quad\text{for finitely generated }G.}
$$

There is a genuine missing hypothesis if the printed assertion is read for arbitrary [pro-p groups](../../../topological-group.md#pro-p-group) and $d(G)$ means the least cardinality of any dense generating family. Here is an explicit [infinite-rank failure of the first-cohomology generator formula](../../../topological-group.md#infinite-rank-failure-of-the-first-cohomology-generator-formula). Let $I=\{0,1\}^{\mathbb N}$ and $G=\prod_{r\in I}\mathbb F_p$. Enumerate the finite binary strings as $s_1,s_2,\ldots$ and define $g_n(r)=1$ if $s_n$ is a prefix of $r$, and $0$ otherwise. For finitely many distinct sequences $r_1,\ldots,r_k$, choose long enough prefixes to distinguish each individually. The corresponding $g_n$ project onto the coordinate unit vectors of $\mathbb F_p^k$, so $\langle g_n:n\geq1\rangle$ surjects onto every finite coordinate projection and is dense in the [product topology](../../../geometry-and-topology.md#product-topology). No finite family can generate densely, since a finitely generated abelian exponent-$p$ subgroup is finite and closed. Thus $d(G)=\aleph_0$. On the other hand, continuity of a linear functional to $\mathbb F_p$ means its kernel contains a basic neighbourhood, so it depends on finitely many coordinates. The coordinate projections are consequently a basis of the continuous [dual space](../../../linear-algebra.md#dual-space), giving

$$
\dim_{\mathbb F_p}H^1(G,\mathbb F_p)=|I|=2^{\aleph_0}>\aleph_0.
$$

**The unrestricted infinite-rank formula is false.** A convention requiring a generating basis tending to the identity is different from the printed unrestricted topological generator count; the finite-rank identity proved above has no such ambiguity.

For finite $X$, a [free pro-p group](../../../topological-group.md#free-pro-p-group) $F_p(X)$ is characterized by the [universal property](../../../category-theory.md#universal-property) that every map $X\to P$ to a [pro-p group](../../../topological-group.md#pro-p-group) extends uniquely to a continuous [group homomorphism](../../../group-theory.md#group-homomorphism) $F_p(X)\to P$. It is the [pro-p completion](../../../topological-group.md#pro-p-completion) of the abstract [free group](../../../geometric-group-theory.md#free-group) on $X$: each map to a finite $p$-group factors through one of the defining finite quotients, and passing to the [inverse limit](../../../module-theory.md#inverse-limit) gives the extension to any [pro-p group](../../../topological-group.md#pro-p-group); uniqueness follows from density. This unrestricted universal property can also define the completion on an arbitrary set $X$. When using an infinite basis required to tend to the identity, one instead imposes the universal property only for maps tending to the identity. Only the finite-rank version is needed for the following argument.

A [finite pro-p presentation](../../../topological-group.md#finite-pro-p-presentation) is an isomorphism

$$
G\cong F_p(x_1,\ldots,x_a)/\overline{\langle R_1,\ldots,R_t\rangle^{F_p}}.
$$

There are finitely many generators and finitely many relators, and the denominator is their closed [normal closure](../../../group-theory.md#normal-closure). The relators are elements of the [free pro-p group](../../../topological-group.md#free-pro-p-group); they may be limits of ordinary words. That distinction is important when writing conjugation relations below.

Now suppose $K\trianglelefteq_oG$ has a [finite pro-p presentation](../../../topological-group.md#finite-pro-p-presentation) with generators $k_1,\ldots,k_a$ and relators $R_1,\ldots,R_t$. The quotient $Q=G/K$ is a [finite p-group](../../../finite-group-theory.md#finite-p-group). Choose a finite [finite pro-p presentation](../../../topological-group.md#finite-pro-p-presentation) $Q=\langle\bar y_1,\ldots,\bar y_b\mid S_1,\ldots,S_c\rangle$. Such a presentation exists, for example by using its entire finite multiplication table. Lift the quotient generators to $y_j\in G$. For every $i,j$, choose elements $W_{ij},V_{ij}$ of the [free pro-p group](../../../topological-group.md#free-pro-p-group) on the $x_i$ that map respectively to $y_j^{-1}k_iy_j$ and $y_jk_iy_j^{-1}$ in $K$. Choose $U_\ell(x)$ mapping to $S_\ell(y)$, which lies in $K$. Form the finite [finite pro-p presentation](../../../topological-group.md#finite-pro-p-presentation)

$$
\begin{aligned}
P=\langle x_1,\ldots,x_a,y_1,\ldots,y_b\mid{}&R_h(x)=1,\\
&y_j^{-1}x_iy_j=W_{ij}(x),\quad y_jx_iy_j^{-1}=V_{ij}(x),\\
&S_\ell(y)=U_\ell(x)\rangle_{\mathrm{pro}\text{-}p}.
\end{aligned}
$$

All listed relations hold in $G$, giving a continuous surjective [group homomorphism](../../../group-theory.md#group-homomorphism) $P\to G$: its compact image contains $K$ and maps onto $Q$.

Let $X$ be the closed [subgroup](../../../group.md#subgroup) of $P$ topologically generated by the $x_i$. Both conjugation directions were included, so each $y_j$ normalizes $X$. The $x_i$ also normalize it, and its closed normalizer contains the generators of $P$. Thus $X\trianglelefteq P$. The relations $R_h$ give a continuous surjection $K\to X$. Its composite with $X\to K$ induced by $P\to G$ fixes every $k_i$, and hence is the identity. Therefore the surjection $K\to X$ is injective as well, so $X\cong K$. On quotienting by $X$, the conjugation and kernel relations disappear, and the remaining presentation is exactly $\langle y_1,\ldots,y_b\mid S_1,\ldots,S_c\rangle_{\mathrm{pro}\text{-}p}=Q$. Thus $P/X\to G/K$ is an isomorphism. The kernel of $P\to G$ lies in $X$ and meets $X$ trivially, so is trivial. Consequently $P\cong G$, proving

$$
\boxed{K\trianglelefteq_oG\text{ finitely presented}\quad\Longrightarrow\quad G\text{ finitely presented}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
