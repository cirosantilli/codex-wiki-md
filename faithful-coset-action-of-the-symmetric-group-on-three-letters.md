# Faithful coset action of the symmetric group on three letters

↑ **Parent:** [Coset action](coset-action.md)

Take the [symmetric group](symmetric-group.md) $G=S_3$ and the [subgroup](subgroup.md) $H=\langle(12)\rangle=\{e,(12)\}$ of [group order](order-of-a-finite-group.md) two. With the rightmost [permutation](permutation.md) applied first, its three left [cosets](coset.md) are

$$
C_3=H=\{e,(12)\},\qquad C_2=(23)H=\{(23),(132)\},\qquad C_1=(13)H=\{(13),(123)\}.
$$

The subscripts record the image of $3$: every member of $C_i$ sends $3$ to $i$. Because $H$ is the [stabilizer subgroup](stabilizer-subgroup.md) of $3$ in the usual [group action](group-action-split.md), $aH\mapsto a(3)$ is a [bijection](bijection.md) onto $\{1,2,3\}$. It is an [equivariant map](equivariant-map.md), since $(ga)(3)=g(a(3))$. The [coset action](coset-action.md) therefore becomes the familiar [group action](group-action-split.md) on three letters. In particular,

$$
(12):C_1\leftrightarrow C_2,\ C_3\mapsto C_3,\qquad
(123):C_1\mapsto C_2\mapsto C_3\mapsto C_1.
$$

<a id="s3-three-coset-action"></a>
![](s3-three-coset-action.png)

**[Figure 11](#s3-three-coset-action). Three left cosets turn left multiplication in $S_3$ into its faithful group action on three labels**. An original computed [coset](coset.md) partition matches each two-element [coset](coset.md) to the common image of $3$. The two rows show left multiplication by $(12)$ and $(123)$. The three [stabilizer subgroups](stabilizer-subgroup.md) intersect only in the [identity element](identity-element.md).

The three [stabilizer subgroups](stabilizer-subgroup.md) are

$$
G_{C_1}=\{e,(23)\},\qquad G_{C_2}=\{e,(13)\},\qquad G_{C_3}=\{e,(12)\}.
$$

Their [intersection](set-intersection.md) is $\{e\}$, so the [subgroup core](core-group-theory.md) and the [group kernel](kernel-of-a-group-homomorphism.md) are trivial. This proves that the [coset action](coset-action.md) is a [faithful group action](faithful-group-action.md) even though every point has a nontrivial [stabilizer subgroup](stabilizer-subgroup.md). The [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) reads $6=3\cdot2$, while the induced [group homomorphism](group-homomorphism.md) gives six distinct [permutations](permutation.md) of the three [cosets](coset.md). For example, $(12)$ and $e$ agree at $C_3$, but disagree at $C_1$; inspecting one label would miss their difference.

The [subgroup](subgroup.md) need not be a [normal subgroup](normal-subgroup.md) for the [coset action](coset-action.md) to exist: $(123)H(123)^{-1}=\{e,(23)\}\ne H$. Here the [group action](group-action-split.md) is informative because the three conjugate [stabilizer subgroups](stabilizer-subgroup.md) have no common nonidentity element. For the [normal subgroup](normal-subgroup.md) $A_3$ instead, [nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md) shows that only the [sign of a permutation](sign-of-a-permutation.md) survives.

## ↑ Ancestors (7)

1. [Coset action](coset-action.md)
2. [Group action](group-action-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Faithful group action](faithful-group-action.md)
- [Faithful quotient of a group action](faithful-quotient-of-a-group-action.md)
- [Nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md)
