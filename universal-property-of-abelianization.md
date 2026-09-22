# Universal property of abelianization

↑ **Parent:** [Abelianization](abelianization.md)

For every [abelian group](abelian-group.md) $A$ and [group homomorphism](group-homomorphism.md) $f:G\to A$, there is a unique [group homomorphism](group-homomorphism.md) $\bar f:G^{\mathrm{ab}}\to A$ such that

$$
f=\bar f\circ q,\qquad \bar f(gG')=f(g).
$$

This is a [universal property](universal-property.md). To see why it holds, compute $f([x,y])=[f(x),f(y)]=e_A$, using [commutativity](commutativity.md) in $A$. Hence $G'\subseteq\ker f$, and $f$ is constant on each [coset](coset.md) of $G'$. The displayed formula is therefore well-defined and preserves multiplication. It is unique because $q$ is [surjective](surjective-function.md). This is an instance of factoring a [group homomorphism](group-homomorphism.md) through a [quotient group](quotient-group.md); see [Conrad, Universal mapping properties, theorem 3.4](https://kconrad.math.uconn.edu/blurbs/linmultialg/universalmapping.pdf).

In particular, every [abelian quotient](abelian-quotient.md) $G/N$ comes from a [surjective group homomorphism](surjective-group-homomorphism.md) $G^{\mathrm{ab}}\to G/N$, $gG'\mapsto gN$. For $S_3$, any [group homomorphism](group-homomorphism.md) to an [abelian group](abelian-group.md) is determined by the common image $a$ of its three [transpositions](transposition-permutation.md), with $a^2=e_A$. Every [even permutation](even-permutation.md) must map to $e_A$. Thus [sign of a permutation](sign-of-a-permutation.md) captures all possible information of this kind, including maps with infinite [abelian groups](abelian-group.md) as their targets.

## ↑ Ancestors (7)

1. [Abelianization](abelianization.md)
2. [Commutator subgroup](commutator-subgroup.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Abelianization](abelianization.md)
