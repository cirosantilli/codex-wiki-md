# Simply transitive group action

↑ **Parent:** [Transitive group action](transitive-group-action.md)

A [group action](group-action.md) on a nonempty [set](set-split.md) $X$ is simply transitive when exactly one [group](group-split.md) element sends any chosen point to any other:

$$
\forall x,y\in X\quad\exists!g\in G:\quad g\cdot x=y.
$$

Equivalently it is both a [transitive group action](transitive-group-action.md) and a [free group action](free-group-action.md); this is also a [regular group action](regular-group-action.md). Transitivity supplies a transport, and freeness makes it unique. Conversely, putting $y=x$ in the uniqueness condition shows that every [stabilizer subgroup](stabilizer-subgroup.md) is $\{e\}$, since the [identity element](identity-element.md) already fixes $x$. In a [transitive group action](transitive-group-action.md), checking that just one [stabilizer subgroup](stabilizer-subgroup.md) is trivial suffices: all the others are [conjugate subgroups](conjugate-subgroup.md).

The [cyclic group](cyclic-group.md) $C_3$ in the diagram under [transitive group action](transitive-group-action.md) is simply transitive. More generally, the [left regular action](left-regular-action.md) of any [group](group-split.md) $G$ on itself is simply transitive: the equation $gx=y$ has the unique solution $g=yx^{-1}$, using the [inverse element](inverse-element.md) of $x$. This shows why the property is useful: every position has a unique label relative to a chosen starting position.

Choose a point $x_0\in X$. Its [orbit map](orbit-map.md)

$$
\phi_{x_0}:G\longrightarrow X,\qquad g\longmapsto g\cdot x_0
$$

is a [bijection](bijection.md) and an [equivariant map](equivariant-map.md) from the [left regular action](left-regular-action.md): $\phi_{x_0}(hg)=h\cdot\phi_{x_0}(g)$. This identifies $X$ with a copy of $G$, but $X$ does not come with a preferred [identity element](identity-element.md). If $x_1=a\cdot x_0$, then $\phi_{x_1}(g)=\phi_{x_0}(ga)$: changing the chosen point composes this identification with right multiplication by $a$. An old label $g$ therefore becomes the new label $ga^{-1}$, which also specifies the side of multiplication for a noncommutative [group](group-split.md).

The transport from $x$ to $y$ remains independent of the chosen point. Writing $x=b\cdot x_0$ and $y=c\cdot x_0$, it is $cb^{-1}$. With $x_1=a\cdot x_0$, the new labels are $ba^{-1}$ and $ca^{-1}$, and

$$
(ca^{-1})(ba^{-1})^{-1}=cb^{-1}.
$$

For a [finite group](finite-group.md), simple transitivity implies $|X|=|G|$. Conversely, a [transitive group action](transitive-group-action.md) with $|X|=|G|<\infty$ is simply transitive by the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md). Equality of [cardinalities](cardinality.md) alone is insufficient without transitivity: the [cyclic group](cyclic-group.md) $C_2$ can fix both points of a two-point [set](set-split.md), giving two [group orbits](orbit-group-theory.md) and two possible self-transports at each point.

## ↑ Ancestors (7)

1. [Transitive group action](transitive-group-action.md)
2. [Group action](group-action.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Free group action](free-group-action.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58/2/solution.md)
