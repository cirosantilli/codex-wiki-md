# Free group action

↑ **Parent:** [Group action](group-action.md)

A [group action](group-action.md) is free if the only element of the [group](group-split.md) fixing any point is the [identity element](identity-element.md). Thus every [stabilizer subgroup](stabilizer-subgroup.md) is trivial. This is a property of an action of any [group](group-split.md), not an assertion that the acting group is a [free group](free-group.md).

Explicitly, for a left [group action](group-action.md) of a [group](group-split.md) $G$ on a [set](set-split.md) $X$ with [identity element](identity-element.md) $e$, freeness means

$$
g\cdot x=x\Longrightarrow g=e\qquad(g\in G,\ x\in X),\qquad G_x=\{e\}\quad(x\in X).
$$

Equivalently, for any $x,y\in X$ there is at most one $g\in G$ with $g\cdot x=y$. Indeed, if $g\cdot x=h\cdot x$, the [group action](group-action.md) rules give $(h^{-1}g)\cdot x=x$, so freeness forces $g=h$; conversely, take $y=x$, since the [identity element](identity-element.md) already sends $x$ to itself. Thus every [orbit map](orbit-map.md) $g\mapsto g\cdot x$ is [injective](injective-function.md), even when its [image of a function](image-of-a-function.md) is only part of $X$.

For a [permutation](permutation.md) example, let the [cyclic group](cyclic-group.md) $C_2=\{e,a\}$ act on the [set](set-split.md) $X=\{1,2,3,4\}$ by $a=(12)(34)$. The nonidentity element exchanges both pairs and fixes no point, so every [stabilizer subgroup](stabilizer-subgroup.md) is $\{e\}$. Its two [group orbits](orbit-group-theory.md) are $\{1,2\}$ and $\{3,4\}$. This is a [free group action](free-group-action.md) but not a [transitive group action](transitive-group-action.md): there is no [group](group-split.md) element sending $1$ to $3$. Each restriction to one [group orbit](orbit-group-theory.md) is a [simply transitive group action](simply-transitive-group-action.md).

<a id="free-actions-two-orbits-and-fixed-points"></a>
![](free-actions-two-orbits-and-fixed-points.png)

**[Figure 7](#free-actions-two-orbits-and-fixed-points). A free group action can have several group orbits**. Two [group actions](group-action.md) of the same [cyclic group](cyclic-group.md) $C_2=\{e,a\}$ on four points. On the left, $a=(12)(34)$ exchanges two pairs. On the right, both [group](group-split.md) elements fix every point. Green outlines show [group orbits](orbit-group-theory.md); gray loops show the [identity element](identity-element.md), and blue arrows show $a$.

The [identity element](identity-element.md) fixes every point in every [group action](group-action.md); freeness excludes fixed points only for nonidentity elements. This also differs from a [fixed point of a group action](fixed-point-of-a-group-action.md), which must be fixed by every [group](group-split.md) element. In the left diagram there are no such [fixed points of a group action](fixed-point-of-a-group-action.md). In the right diagram, the same abstract [cyclic group](cyclic-group.md) $C_2$ acts by $e\cdot x=a\cdot x=x$: all four points are [fixed points of a group action](fixed-point-of-a-group-action.md), every [stabilizer subgroup](stabilizer-subgroup.md) is $C_2$, and each [group orbit](orbit-group-theory.md) is a [singleton set](singleton-mathematics.md). Consequently this second [group action](group-action.md) is neither free nor transitive. A [group action](group-action.md) with no [fixed points of a group action](fixed-point-of-a-group-action.md) can still fail freeness: the natural [group action](group-action.md) of the [symmetric group](symmetric-group.md) $S_3$ has no point fixed by all of $S_3$, but $(23)$ fixes $1$.

For a [finite group](finite-group.md), the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) makes each [group orbit](orbit-group-theory.md) of a [free group action](free-group-action.md) have [cardinality](cardinality.md) $|G|$. If $X$ is also finite, $|X|$ is therefore a multiple of the [group order](order-of-a-finite-group.md), with one copy of $|G|$ for each [group orbit](orbit-group-theory.md). The [trivial group](trivial-group.md) acts freely on every [set](set-split.md), and acts transitively exactly on a [singleton set](singleton-mathematics.md). On the [empty set](empty-set.md) freeness is vacuous; our convention under [transitive group action](transitive-group-action.md) requires a nonempty [set](set-split.md) for transitivity.

**Table of contents**

- [Finite groups cannot act freely on Euclidean space](finite-groups-cannot-act-freely-on-euclidean-space.md)
- [Free actions on even-dimensional spheres have order at most two](free-actions-on-even-dimensional-spheres-have-order-at-most-two.md)
- [Free sphere actions exclude elementary abelian subgroups of rank two](free-sphere-actions-exclude-elementary-abelian-subgroups-of-rank-two.md)

## ↑ Ancestors (6)

1. [Group action](group-action.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Free actions on even-dimensional spheres have order at most two](free-actions-on-even-dimensional-spheres-have-order-at-most-two.md)
- [Free group action](free-group-action.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16/4/2/solution.md)
- [Simply transitive group action](simply-transitive-group-action.md)
- [Transitive group action](transitive-group-action.md)
