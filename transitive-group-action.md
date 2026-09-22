# Transitive group action

↑ **Parent:** [Group action](group-action-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transitive_group_action)

A [group action](group-action-split.md) on a nonempty [set](set-split.md) $X$ is transitive when every two points lie in the same [orbit of a group action](orbit-group-theory.md), equivalently when for all $x,y\in X$ there is a [group](group-split.md) element $g$ with $g\cdot x=y$. There is exactly one [group orbit](orbit-group-theory.md): every position is reachable from every other. Requiring $X\ne\varnothing$ avoids calling the [group action](group-action-split.md) on the [empty set](empty-set.md) transitive merely because the quantified statement has no points to test.[Definition 1.1, printed page 1: transitivity requires a nonempty set and exactly one orbit](transitive-group-actions-by-keith-conrad.md)

Here a left [group action](group-action-split.md) of a [group](group-split.md) $G$ means a [function](function-split.md) $G\times X\to X$, written $(g,x)\mapsto g\cdot x$, satisfying

$$
e\cdot x=x,\qquad (gh)\cdot x=g\cdot(h\cdot x),
$$

where $e$ is the [identity element](identity-element.md). Products move the point by $h$ first, then by $g$. Transitivity says that an [orbit map](orbit-map.md) $G\to X$, $g\mapsto g\cdot x$, is [surjective](surjective-function.md) for every $x\in X$; it suffices to check one chosen point.[Definition 1.3, printed page 2: the two action axioms](group-actions-by-keith-conrad.md)[Theorem 3.1, printed page 2: equivalent tests for transitivity](transitive-group-actions-by-keith-conrad.md)

For example, the [symmetric group](symmetric-group.md) $S_3$ acts on $X=\{1,2,3\}$ by $\sigma\cdot i=\sigma(i)$. This is a [transitive group action](transitive-group-action.md), but it is not a [free group action](free-group-action.md): the [stabilizer subgroup](stabilizer-subgroup.md) of $1$ is $\{e,(23)\}$. Both the [transposition](transposition-permutation.md) $(12)$ and the [cyclic permutation](cyclic-permutation.md) $(123)$ send $1$ to $2$. In contrast, the [cyclic group](cyclic-group.md) $C_3=\mathbb Z/3\mathbb Z$ acts on itself by $k\cdot x=k+x\pmod3$, using [modular arithmetic](modular-arithmetic-split.md). The [group](group-split.md) element sending $x$ to $y$ is uniquely $k=y-x\pmod3$. These two [group actions](group-action-split.md) reach the same number of points, but only the second has unique transport between them.

<a id="transitive-actions-symmetric-and-cyclic"></a>
![](transitive-actions-symmetric-and-cyclic.png)

**[Figure 5](#transitive-actions-symmetric-and-cyclic). Transitive group actions with and without unique transport**. The [symmetric group](symmetric-group.md) $S_3$ on three labels has a [stabilizer subgroup](stabilizer-subgroup.md) of [group order](order-of-a-finite-group.md) two at each point, hence two [group](group-split.md) elements sending any chosen point to any other. The [cyclic group](cyclic-group.md) $C_3$ acting on itself has trivial [stabilizer subgroups](stabilizer-subgroup.md) and one transport per pair. Red arrows show a generating [cyclic permutation](cyclic-permutation.md); blue arrows show the extra [transposition](transposition-permutation.md) in $S_3$. Gray loops show the [identity element](identity-element.md) in both [group actions](group-action-split.md).

The [stabilizer subgroup](stabilizer-subgroup.md) $G_x=\{h\in G:h\cdot x=x\}$ measures the ambiguity of transport. If $g_0\cdot x=y$, then

$$
\{g\in G:g\cdot x=y\}=g_0G_x,\qquad G_y=g_0G_xg_0^{-1}.
$$

The first [set](set-split.md) is a left [coset](coset.md), and the second identity says that [stabilizer subgroups](stabilizer-subgroup.md) in one [group orbit](orbit-group-theory.md) are [conjugate subgroups](conjugate-subgroup.md). Briefly, $g\cdot x=g_0\cdot x$ exactly when $g_0^{-1}g\in G_x$. Thus, for a [finite group](finite-group.md) in a [transitive group action](transitive-group-action.md), the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) gives $|G|=|X|\,|G_x|$, and there are exactly $|G_x|$ transports for each pair of points. The example counts are $6=3\cdot2$ for $S_3$ and $3=3\cdot1$ for $C_3$. This separates the number of reachable positions from the number of ways to reach each one.[Theorem 3.16(b)-(c), printed pages 12-13: conjugate stabilizers, transport cosets and the orbit-stabilizer formula](group-actions-by-keith-conrad.md)

**Table of contents**

- [Simply transitive group action](simply-transitive-group-action.md)
- [Regular group action](regular-group-action.md)
- [Derangement in a transitive group action](derangement-in-a-transitive-group-action.md)
  - [Derangement counting formula](derangement-counting-formula.md)
- [Rank of a transitive permutation group](rank-of-a-transitive-permutation-group.md)
- [Regular permutation subgroup](regular-permutation-subgroup.md)
  - [Centralizer of a regular permutation subgroup](centralizer-of-a-regular-permutation-subgroup.md)
- [Sharp t-transitivity](sharp-t-transitivity.md)
  - [Sharp three-transitivity](sharp-three-transitivity.md)
  - [Sharp two-transitivity](sharp-two-transitivity.md)
  - [Regular kernel of a finite sharply two-transitive group](regular-kernel-of-a-finite-sharply-two-transitive-group.md)
- [One-point extension of a permutation group](one-point-extension-of-a-permutation-group.md)
  - [Double-coset criterion for a one-point extension](double-coset-criterion-for-a-one-point-extension.md)
- [Prime-degree transposition criterion](prime-degree-transposition-criterion.md)

## ↑ Ancestors (6)

1. [Group action](group-action-split.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Cayley's theorem](cayley-s-theorem.md)
- [Coset action](coset-action.md)
- [Faithful group action](faithful-group-action.md)
- [Free group action](free-group-action.md)
- [Nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Orbit (group theory)](orbit-group-theory.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-2/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/11g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-143/1/d/solution.md)
- [Rotational symmetry group of a regular icosahedron](rotational-symmetry-group-of-a-regular-icosahedron.md)
- [Simply transitive group action](simply-transitive-group-action.md)
- [Transitive group action](transitive-group-action.md)
