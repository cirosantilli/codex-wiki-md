<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [inverse system](../../../../../inverse-system.md) of [topological spaces](../../../../../topological-space.md) over a [directed set](../../../../../directed-set.md) $I$ consists of spaces $X_i$ and continuous maps $f_{ij}:X_j\to X_i$ for $i\leq j$, with $f_{ii}=1$ and $f_{ik}=f_{ij}f_{jk}$. Its [inverse limit](../../../../../inverse-limit.md) is a space $X$ with compatible continuous projections $\pi_i$ such that every compatible family of continuous maps $u_i:Y\to X_i$ factors uniquely through a continuous map $u:Y\to X$. To construct it, take

$$
X=\{(x_i)\in\prod_{i\in I}X_i:f_{ij}(x_j)=x_i\text{ whenever }i\leq j\}
$$

with the [subspace topology](../../../../../subspace-topology.md) inherited from the [product topology](../../../../../product-topology.md). The map $u(y)=(u_i(y))$ has values in $X$ and is continuous by the definition of the [product topology](../../../../../product-topology.md); its coordinates force uniqueness. If $X'$ is another [inverse limit](../../../../../inverse-limit.md), the two universal properties give continuous maps $X\to X'$ and $X'\to X$ whose composites have all the same projections as the identity. Uniqueness makes these composites the identity. **The inverse limit exists and is unique up to a unique projection-preserving homeomorphism.** An arbitrary [inverse limit](../../../../../inverse-limit.md) may be empty; nonemptiness requires additional hypotheses.

Use the usual Hausdorff convention for a [topological group](../../../../../topological-group-split.md). An [inverse limit](../../../../../inverse-limit.md) of finite discrete [groups](../../../../../group-split.md) is a closed subgroup of their product: each compatibility condition is closed because the finite factors are [Hausdorff spaces](../../../../../hausdorff-space.md). The [Tychonoff theorem](../../../../../tychonoff-s-theorem.md) gives [compactness](../../../../../compact-space.md), and distinct tuples are separated by a clopen coordinate cylinder, so the limit is [totally disconnected](../../../../../totally-disconnected-space.md). Coordinatewise multiplication and inversion are continuous, giving a [profinite group](../../../../../profinite-group.md).

Conversely, let $G$ be a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) and a [totally disconnected](../../../../../totally-disconnected-space.md) [topological group](../../../../../topological-group-split.md). We use the standard topological fact that a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) that is [totally disconnected](../../../../../totally-disconnected-space.md) has a basis of [clopen sets](../../../../../clopen-set.md). Given an identity neighbourhood, choose a clopen identity neighbourhood $U$ inside it. [Compactness](../../../../../compact-space.md) of $U$ and continuity of multiplication give a symmetric identity neighbourhood $V$ with $VU\subseteq U$: cover $U$ by finitely many neighbourhoods on which multiplication by a sufficiently small identity neighbourhood stays inside $U$, then intersect those identity neighbourhoods. Symmetry gives $vU=U$ for $v\in V$. Consequently $H=\{g:gU=U\}$ is a subgroup containing $V$, hence an [open subgroup](../../../../../open-subgroup.md), and $H\subseteq U$ since $1\in U$. Its open [cosets](../../../../../coset.md) cover the compact group, so there are finitely many. The [normal core](../../../../../core-group-theory.md) $N=\bigcap_{g\in G}gHg^{-1}$ is a finite intersection of open subgroups, hence an [open normal subgroup](../../../../../open-normal-subgroup.md) contained in $U$. Thus the open normal subgroups form an identity-neighbourhood basis and have trivial intersection.

The canonical [group homomorphism](../../../../../group-homomorphism.md) $G\to\varprojlim_NG/N$ is continuous and injective. For a compatible tuple of quotient elements, its inverse-image cosets in $G$ are closed and have the [finite intersection property](../../../../../finite-intersection-property.md): a finite family is refined by the quotient for the intersection of its normal subgroups. [Compactness](../../../../../compact-space.md) gives an element in all those cosets, proving surjectivity. A continuous bijection from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md). **The compact totally disconnected and inverse-limit definitions of a profinite group agree.**

Index the finite nonempty sets $\mathcal P(N)$ by open normal subgroups, with the transition from $M$ to $N$ when $M\subseteq N$ given by image under $G/M\to G/N$. Images of [Sylow subgroups](../../../../../sylow-subgroup.md) under surjections of finite [groups](../../../../../group-split.md) are [Sylow subgroups](../../../../../sylow-subgroup.md). These transitions are surjective: if $S\leq G/N$ is a [Sylow subgroup](../../../../../sylow-subgroup.md), choose a [Sylow subgroup](../../../../../sylow-subgroup.md) in its full inverse image in $G/M$. It maps onto $S$, and its order has the full $p$-part of $|G/M|$, so it is a [Sylow subgroup](../../../../../sylow-subgroup.md) of $G/M$ too. The transitions respect composition, giving an [inverse system](../../../../../inverse-system.md) of finite sets.

Its [inverse limit](../../../../../inverse-limit.md) is nonempty. Indeed, finitely many compatibility conditions can be satisfied by choosing one [Sylow subgroup](../../../../../sylow-subgroup.md) in a quotient refining all the involved quotients and taking its images; [compactness](../../../../../compact-space.md) of the product of the finite sets then gives a compatible family $(P_N)_N$. Define

$$
P=\bigcap_N\pi_N^{-1}(P_N).
$$

This is a closed subgroup of $G$. Its image in $G/N$ is exactly $P_N$: for a prescribed $s\in P_N$, each finite collection of conditions defining $P$ together with $\pi_N(g)=s$ is satisfiable in a common refining quotient, because the transitions on the chosen [Sylow subgroups](../../../../../sylow-subgroup.md) are surjective. The [finite intersection property](../../../../../finite-intersection-property.md) again supplies $g\in P$. Hence $P\cong\varprojlim_NP_N$ is a [pro-p group](../../../../../pro-p-group.md) and $PN/N=P_N$ for every $N$.

Finally, if a [pro-p subgroup](../../../../../pro-p-subgroup.md) $Q$ contains $P$, its image in every finite quotient is a [p-group](../../../../../p-group.md) containing the [Sylow subgroup](../../../../../sylow-subgroup.md) $P_N$, so that image equals $P_N$. Thus every $q\in Q$ belongs to every $\pi_N^{-1}(P_N)$, whence $Q\subseteq P$. **The constructed $P$ is a maximal pro-p subgroup.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
