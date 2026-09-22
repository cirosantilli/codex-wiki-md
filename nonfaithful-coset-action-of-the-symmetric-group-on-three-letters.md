# Nonfaithful coset action of the symmetric group on three letters

↑ **Parent:** [Faithful group action](faithful-group-action.md)

Let $G=S_3$, the [symmetric group](symmetric-group.md) on three letters, and take the [normal subgroup](normal-subgroup.md) $N=A_3=\{e,(123),(132)\}$, the [alternating group](alternating-group.md) of [even permutations](even-permutation.md). Its two left [cosets](coset.md) are

$$
E=N=\{e,(123),(132)\},\qquad O=(12)N=\{(12),(13),(23)\}.
$$

Products of [permutations](permutation.md) apply the rightmost factor first. Left multiplication by an [even permutation](even-permutation.md) preserves both [cosets](coset.md), while left multiplication by an [odd permutation](odd-permutation.md) exchanges them. For example,

$$
(123)\cdot E=E,\quad (123)\cdot O=O,\qquad
(12)\cdot E=O,\quad (12)\cdot O=E.
$$

Consequently all six [group](group-split.md) elements give only two distinct [permutations](permutation.md) of $\{E,O\}$. Both [stabilizer subgroups](stabilizer-subgroup.md) equal $A_3$, so their intersection, the [group kernel](kernel-of-a-group-homomorphism.md), is $A_3$. This is a [transitive group action](transitive-group-action.md) because $(12)$ reaches the other [coset](coset.md), but it is not a [faithful group action](faithful-group-action.md) because $(123)$ fixes both.

<a id="s3-two-coset-action-kernel"></a>
![](s3-two-coset-action-kernel.png)

**[Figure 10](#s3-two-coset-action-kernel). A transitive group action of $S_3$ on two cosets detects only the sign of a permutation**. This computed example groups the six [permutations](permutation.md) by their induced [permutations](permutation.md) of the two [cosets](coset.md). All three [even permutations](even-permutation.md) fix both labels; all three [odd permutations](odd-permutation.md) exchange them. The [group kernel](kernel-of-a-group-homomorphism.md) has three elements.

The [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) still works perfectly: $6=2\cdot3$. It counts reachable labels, without asserting that the induced [group homomorphism](group-homomorphism.md) is [injective](injective-function.md). The [quotient group](quotient-group.md) $S_3/A_3\cong C_2$ captures exactly the two visible operations, identity and exchange. This is the same [group homomorphism](group-homomorphism.md) as the [sign of a permutation](sign-of-a-permutation.md), with $+1$ represented by fixing both labels and $-1$ by exchanging them. Contrast the three-label example in [faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md).

## ↑ Ancestors (7)

1. [Faithful group action](faithful-group-action.md)
2. [Group action](group-action-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Coset action](coset-action.md)
- [Faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Faithful group action](faithful-group-action.md)
- [Faithful quotient of a group action](faithful-quotient-of-a-group-action.md)
