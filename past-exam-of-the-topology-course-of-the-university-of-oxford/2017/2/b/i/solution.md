<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [set](../../../../../set-split.md) $X/\mathcal R$ consists of the [equivalence classes](../../../../../equivalence-class.md) $[x]$ for $\mathcal R$. The canonical [surjection](../../../../../surjective-function.md) $q:X\to X/\mathcal R$, $q(x)=[x]$, defines its [quotient topology](../../../../../quotient-topology.md):

$$
O\subseteq X/\mathcal R\text{ is open}\quad\Longleftrightarrow\quad q^{-1}(O)\text{ is open in }X.
$$

The [quotient space](../../../../../quotient-topological-space.md) includes this [topology](../../../../../topology-split.md), not just the collection of [equivalence classes](../../../../../equivalence-class.md).

Regard the [circle](../../../../../circle.md) as $S^1=\{z\in\mathbb C:|z|=1\}$ and use the [continuous](../../../../../continuous-function.md) [surjection](../../../../../surjective-function.md)

$$
h:S^1\longrightarrow[0,1],\qquad h(z)=\frac{1+\operatorname{Re}z}{2}.
$$

Define $z\mathcal R w$ precisely when $h(z)=h(w)$. This is an [equivalence relation](../../../../../equivalence-relation.md), being equality of [function](../../../../../function-split.md) values. Equivalently $w=z$ or $w=\overline z$, so the construction is the [circle modulo reflection](../../../../../circle-modulo-reflection.md).

Since $h$ is constant on each [equivalence class](../../../../../equivalence-class.md), it induces a [bijection](../../../../../bijection.md)

$$
\overline h:S^1/\mathcal R\longrightarrow[0,1],\qquad [z]\longmapsto h(z).
$$

It is [continuous](../../../../../continuous-function.md) by the [universal property of the quotient topology](../../../../../universal-property-of-the-quotient-topology.md), because $\overline h\circ q=h$ is [continuous](../../../../../continuous-function.md). The [circle](../../../../../circle.md) is [compact](../../../../../compact-space.md) by the [Heine-Borel theorem](../../../../../heine-borel-theorem.md), and its [quotient space](../../../../../quotient-topological-space.md) is a [continuous image of a compact space](../../../../../continuous-image-of-a-compact-space.md), hence [compact](../../../../../compact-space.md). The [closed interval](../../../../../closed-real-interval.md) is [Hausdorff](../../../../../hausdorff-space.md). Part (a)(ii) therefore proves

$$
\boxed{S^1/\mathcal R\cong[0,1].}
$$

Geometrically, the [equivalence relation](../../../../../equivalence-relation.md) folds the upper and lower semicircles together, retaining the two real endpoints separately.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
