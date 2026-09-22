# Free finite actions with equal cardinality are isomorphic

↑ **Parent:** [Free group action](free-group-action.md)

Let a [finite group](finite-group.md) $G$ have [free group actions](free-group-action.md) on finite [sets](set-split.md) $S,T$ of equal [cardinality](cardinality.md). There is a [bijection](bijection.md) $f:S\to T$ satisfying $f(g\cdot s)=g*f(s)$ for every $g\in G$, $s\in S$.

By the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md), every [orbit of a group action](orbit-group-theory.md) in either [set](set-split.md) has [cardinality](cardinality.md) $|G|$. Thus both have $r=|S|/|G|$ [orbits of a group action](orbit-group-theory.md). Choose representatives $s_1,\ldots,s_r$ and $t_1,\ldots,t_r$, and define

$$
f(g\cdot s_i)=g*t_i.
$$

Every point has a unique displayed representation: its [orbit of a group action](orbit-group-theory.md) determines $i$, and the [free group action](free-group-action.md) property makes $g$ unique. Thus $f$ is well defined, and $g*t_i\mapsto g\cdot s_i$ defines its inverse. Finally

$$
f(h\cdot(g\cdot s_i))=(hg)*t_i=h*(g*t_i)=h*f(g\cdot s_i),
$$

proving the required compatibility. Empty [sets](set-split.md) are covered by the unique empty [bijection](bijection.md). This shows that a finite free [group action](group-action-split.md) is determined up to such an isomorphism by its number of [orbits of a group action](orbit-group-theory.md).

## ↑ Ancestors (7)

1. [Free group action](free-group-action.md)
2. [Group action](group-action-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/7/b/ii/solution.md)
