# Commutator subgroup of the symmetric group on three letters

↑ **Parent:** [Commutator subgroup](commutator-subgroup.md)

For the [symmetric group](symmetric-group.md) $S_3$, take the [transpositions](transposition-permutation.md) $x=(12)$ and $y=(23)$. Products of [permutations](permutation.md) apply the rightmost factor first. Then

$$
xy=(123),\qquad yx=(132),\qquad [x,y]=(12)(23)(12)(23)=(132).
$$

The last [permutation](permutation.md) sends $1\mapsto3$, $3\mapsto2$, and $2\mapsto1$: two swaps fail to commute by an entire three-cycle.

<a id="image-group-commutators-and-the-information-surviving-abelianization-in-the-symmetric-group-s-3"></a>
![](s3-commutator-and-abelianization.png)

**[Figure 3](#image-group-commutators-and-the-information-surviving-abelianization-in-the-symmetric-group-s-3). Group commutators and the information surviving abelianization in the symmetric group $S_3$**. The upper rows group the six [permutations](permutation.md) by [sign of a permutation](sign-of-a-permutation.md). Each triangle labels the original vertices in their new positions. The lower row applies $y,x,y^{-1},x^{-1}$ successively, giving $[x,y]=(132)$ under the rightmost-first convention. The [commutator subgroup](commutator-subgroup.md) consists of the three [even permutations](even-permutation.md); the [center of a group](center-of-a-group.md) here contains only $e$.

Every [group commutator](group-commutator.md) has [sign of a permutation](sign-of-a-permutation.md) $+1$, so $S_3'\subseteq A_3$, the [alternating group](alternating-group.md) of [even permutations](even-permutation.md). Conversely, the displayed [group commutator](group-commutator.md) generates $A_3=\{e,(123),(132)\}$. Therefore $S_3'=A_3$. The two [cosets](coset.md) are the [even permutations](even-permutation.md) and the [odd permutations](odd-permutation.md), and their multiplication is just multiplication of signs:

$$
S_3^{\mathrm{ab}}=S_3/A_3\cong\{+1,-1\}\cong C_2.
$$

This is the [first isomorphism theorem](first-isomorphism-theorem.md) applied to the [sign of a permutation](sign-of-a-permutation.md). Once [commutativity](commutativity.md) is forced, all three [transpositions](transposition-permutation.md) become indistinguishable, and both three-cycles become the [identity element](identity-element.md). The surviving information is exactly whether the [permutation](permutation.md) is even or odd. Compare the very different [center of a group](center-of-a-group.md) $Z(S_3)=\{e\}$.

## ↑ Ancestors (6)

1. [Commutator subgroup](commutator-subgroup.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Abelianization](abelianization.md)
- [Center of a group](center-of-a-group.md)
