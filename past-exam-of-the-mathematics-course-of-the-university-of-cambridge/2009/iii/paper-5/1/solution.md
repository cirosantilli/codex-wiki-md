<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [topological group](../../../../../topological-group-split.md) is a [group](../../../../../group-split.md) equipped with a [topology](../../../../../topology-split.md) for which multiplication $G\times G\to G$ and inversion $G\to G$ are [continuous maps](../../../../../continuous-map.md). The product uses the [product topology](../../../../../product-topology.md). Translation and inversion are therefore [homeomorphisms](../../../../../homeomorphism.md). Hausdorffness is sometimes included in the definition; the two open-subgroup arguments below do not require it.

For the [inverse system](../../../../../inverse-system.md), take a [directed set](../../../../../directed-set.md) $I$, [topological spaces](../../../../../topological-space.md) $X_i$, and [continuous maps](../../../../../continuous-map.md) $f_{ij}:X_j\to X_i$ for $i\leq j$, with $f_{ii}=\mathrm{id}$ and $f_{ik}=f_{ij}f_{jk}$. An [inverse limit](../../../../../inverse-limit.md) is a space $X$ with compatible [continuous maps](../../../../../continuous-map.md) $\pi_i:X\to X_i$ such that every compatible family $q_i:Y\to X_i$ factors uniquely as $q_i=\pi_iq$ through a [continuous map](../../../../../continuous-map.md) $q:Y\to X$. Existence follows from the concrete construction

$$
X=\left\{(x_i)\in\prod_{i\in I}X_i:f_{ij}(x_j)=x_i\text{ whenever }i\leq j\right\},
$$

with the subspace [topology](../../../../../topology-split.md) of the [product topology](../../../../../product-topology.md). The only possible map $q$ is $q(y)=(q_i(y))_i$. Compatibility puts its image in $X$, and coordinatewise continuity makes it continuous. This proves the [universal property of an inverse limit](../../../../../universal-property-of-an-inverse-limit.md), even when $X$ is empty. Given two [inverse limits](../../../../../inverse-limit.md), their universal properties supply maps each way; the composites have the same coordinates as the identity, so uniqueness makes them identities. **The inverse limit exists and is unique up to the unique homeomorphism respecting its projections.**

A [profinite group](../../../../../profinite-group.md) can be defined as an [inverse limit](../../../../../inverse-limit.md) of finite discrete [groups](../../../../../group-split.md), or as a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) that is a [totally disconnected space](../../../../../totally-disconnected-space.md), equipped with continuous [group](../../../../../group-split.md) operations. For the first implication, use the [Tychonoff theorem](../../../../../tychonoff-s-theorem.md). The compatibility equalities define a closed [subgroup](../../../../../subgroup.md) of the compact Hausdorff product. Two distinct points are distinguished by a finite discrete coordinate, so no connected subset contains both. Consequently the [inverse limit](../../../../../inverse-limit.md) is a compact Hausdorff totally disconnected [topological group](../../../../../topological-group-split.md).

For the converse, use the topological result that a compact Hausdorff totally disconnected space has a basis of [clopen sets](../../../../../clopen-set.md). Choose a [clopen set](../../../../../clopen-set.md) $U$ containing $1$ inside any specified identity neighbourhood. For each $u\in U$, continuity gives an identity neighbourhood $V_u$ and an open neighbourhood $W_u$ of $u$ with $V_uW_u\subseteq U$. Finitely many $W_u$ cover the [compact set](../../../../../compact-space.md) $U$. Intersect their $V_u$ and its inverse to obtain a symmetric identity neighbourhood $V$ with $VU\subseteq U$. Symmetry also gives $V^{-1}U\subseteq U$, and hence $vU=U$ for every $v\in V$. The set

$$
H=\{g\in G:gU=U\}
$$

is a [subgroup](../../../../../subgroup.md) containing $V$, so it is open. It is contained in $U$, since $1\in U$ and $h=h\cdot1\in hU=U$. By part (ii), $H$ has finite index. Its [normal core of a subgroup](../../../../../core-group-theory.md) is a finite intersection of conjugates of $H$, hence an open [normal subgroup](../../../../../normal-subgroup.md) $N$ contained in $U$. This proves the [open normal subgroup basis of a profinite group](../../../../../open-normal-subgroup-basis-of-a-profinite-group.md).

The natural [group homomorphism](../../../../../group-homomorphism.md)

$$
G\longrightarrow\varprojlim_{N\trianglelefteq_oG}G/N
$$

is injective because the intersection of these $N$ is $\{1\}$. For a compatible family of cosets, any finitely many have nonempty intersection: their intersection subgroup is another indexing subgroup, and its prescribed coset lies in each. The [finite intersection property](../../../../../finite-intersection-property.md) and compactness give a point belonging to all the cosets, proving surjectivity. Finally a continuous bijection from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md). **The two definitions of profinite group are equivalent.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
