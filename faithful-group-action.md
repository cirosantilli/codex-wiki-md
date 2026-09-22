# Faithful group action

↑ **Parent:** [Group action](group-action-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faithful_group_action)

A group action is faithful when only the identity acts as the identity on every point.

For a [group action](group-action-split.md) of $G$ on a [set](set-split.md) $X$, form the [group homomorphism](group-homomorphism.md)

$$
\rho:G\longrightarrow\operatorname{Sym}(X),\qquad \rho(g)(x)=g\cdot x.
$$

A [faithful group action](faithful-group-action.md) means that $\rho$ is [injective](injective-function.md): different [group](group-split.md) elements induce different [permutations](permutation.md) of $X$. Equivalently, its [group kernel](kernel-of-a-group-homomorphism.md) is trivial:

$$
K=\ker\rho=\{g\in G:g\cdot x=x\text{ for every }x\in X\}=\bigcap_{x\in X}G_x=\{e\}.
$$

Here $G_x$ is the [stabilizer subgroup](stabilizer-subgroup.md) of $x$, and $e$ is the [identity element](identity-element.md).[Theorem 1.7, printed page 3, and Definition 2.17, printed page 9: actions as homomorphisms and faithfulness](group-actions-by-keith-conrad.md)

The test is global. A [faithful group action](faithful-group-action.md) requires each nonidentity [group](group-split.md) element to move at least one point; a [free group action](free-group-action.md) requires it to move every point. In the [faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md), $(12)$ fixes one [coset](coset.md) and exchanges the other two. Thus a nontrivial [stabilizer subgroup](stabilizer-subgroup.md) does not rule out faithfulness. The distinction follows directly from the order of the quantifiers:

$$
\text{faithful: }\forall g\ne e\ \exists x:\ g\cdot x\ne x,\qquad
\text{free: }\forall g\ne e\ \forall x:\ g\cdot x\ne x.
$$

On a nonempty [set](set-split.md), a [free group action](free-group-action.md) is therefore a [faithful group action](faithful-group-action.md). A [transitive group action](transitive-group-action.md) instead asks whether every point can reach every other; it allows several [group](group-split.md) elements to perform exactly the same rearrangement. The [nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md) is a counterexample to the claim that every [transitive group action](transitive-group-action.md) is a [faithful group action](faithful-group-action.md).

For a short proof of the [group kernel](kernel-of-a-group-homomorphism.md) criterion, $\rho(g)=\rho(h)$ exactly when $\rho(h^{-1}g)$ is the identity [permutation](permutation.md), or $h^{-1}g\in K$. If $K=\{e\}$, this forces $g=h$; if $K$ contains a nonidentity element, that element and $e$ act identically. Thus a [faithful group action](faithful-group-action.md) turns $G$ into an actual [subgroup](subgroup.md) of a [symmetric group](symmetric-group.md), retaining its [group operation](group-operation.md) as [function composition](function-composition.md). Choosing a suitable [coset action](coset-action.md) can give a much smaller [set](set-split.md) of labels than the [regular group action](regular-group-action.md) used in [Cayley's theorem](cayley-s-theorem.md).

**Table of contents**

- [Nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Faithful quotient of a group action](faithful-quotient-of-a-group-action.md)
- [Normal subgroup orbits in a faithful prime-degree action](normal-subgroup-orbits-in-a-faithful-prime-degree-action.md)

## ↑ Ancestors (6)

1. [Group action](group-action-split.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Cayley's theorem](cayley-s-theorem.md)
- [Coset action](coset-action.md)
- [Faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Faithful group action](faithful-group-action.md)
- [Faithful quotient of a group action](faithful-quotient-of-a-group-action.md)
- [Group action](group-action-split.md)
- [Minimal faithful permutation degree of the quaternion group](minimal-faithful-permutation-degree-of-the-quaternion-group.md)
- [Nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Normalizer](normalizer.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/5e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/5e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/5d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/2/f/iii/solution.md)
- [Stabilizer subgroup](stabilizer-subgroup.md)
