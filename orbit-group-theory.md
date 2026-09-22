# Orbit (group theory)

↑ **Parent:** [Group action](group-action.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbit_(group_theory))

For a [group action](group-action.md) of a [group](group-split.md) $G$ on a [set](set-split.md) $X$, the [orbit of a group action](orbit-group-theory.md) of $x\in X$ is the [subset](subset.md) of all positions reachable from $x$:

$$
Gx=G\cdot x=\{g\cdot x:g\in G\}\subseteq X.
$$

Two points belong to the same [group orbit](orbit-group-theory.md) exactly when one can be moved to the other by a [group](group-split.md) element. This is an [equivalence relation](equivalence-relation.md): the [identity element](identity-element.md) gives $x\sim x$, the [inverse element](inverse-element.md) of a transformation reverses a move, and a product combines two moves. Hence the [group orbits](orbit-group-theory.md) form a [partition of a set](partition-of-a-set.md) of $X$ into [equivalence classes](equivalence-class.md). A [transitive group action](transitive-group-action.md) on a nonempty [set](set-split.md) has just one [group orbit](orbit-group-theory.md). See [Ackerman's algebra notes, lemma 0.5.1.3, for the orbit partition](https://people.math.harvard.edu/~nate/teaching/UPenn/2007/fall/math_371/lectures/week_1/lecture_1/lecture_1.pdf).

For the [square](square.md) and the eight-element [dihedral group](dihedral-group.md) $D_4$ defined under [group action](group-action.md), direct enumeration gives the following separate [group orbits](orbit-group-theory.md):

- On [vertices of a polygon](vertex-of-a-polygon.md), $D_4\cdot A=\{A,B,C,D\}$ has size four.
- On unoriented [sides of a polygon](side-of-a-polygon.md), $D_4\cdot AB=\{AB,BC,CD,DA\}$ has size four; $AB$ and $BA$ denote the same [side of a polygon](side-of-a-polygon.md).
- On unoriented [diagonals of a polygon](diagonal-of-a-polygon.md), $D_4\cdot AC=\{AC,BD\}$ has size two.
- On the [singleton set](singleton-mathematics.md) containing the [centroid](centroid.md) $O=(0,0)$, $D_4\cdot O=\{O\}$ has size one, so $O$ is a [fixed point of a group action](fixed-point-of-a-group-action.md).

These counts depend on the chosen [group action](group-action.md), not just the [group](group-split.md). An [orbit of a group action](orbit-group-theory.md) describes all configurations equivalent under the permitted transformations. For [ordered pairs](ordered-pair.md) under the [symmetric group](symmetric-group.md), equality of the two entries is preserved, separating the two [group orbits](orbit-group-theory.md) in [equality-pattern orbits of ordered pairs](equality-pattern-orbits-of-ordered-pairs.md); the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) computes their sizes when the [symmetric group](symmetric-group.md) is $S_3$.

**Table of contents**

- [Equality-pattern orbits of ordered pairs](equality-pattern-orbits-of-ordered-pairs.md)
- [Real rotation orbits on a complex unit quadric](real-rotation-orbits-on-a-complex-unit-quadric.md)
- [Equality-pattern orbits of projective triples](equality-pattern-orbits-of-projective-triples.md)

## ↑ Ancestors (6)

1. [Group action](group-action.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
