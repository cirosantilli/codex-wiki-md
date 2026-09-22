<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

An [equivalence relation](../../../../../equivalence-relation.md) is a [binary relation](../../../../../binary-relation.md) that is simultaneously a [reflexive relation](../../../../../reflexive-relation.md), a [symmetric relation](../../../../../symmetric-relation.md) and a [transitive relation](../../../../../transitive-relation.md): $x\sim x$; $x\sim y$ implies $y\sim x$; and $x\sim y$, $y\sim z$ imply $x\sim z$. The [equivalence class](../../../../../equivalence-class.md) of $x$ is

$$
[x]=\{y\in X:y\sim x\}.
$$

Each [equivalence class](../../../../../equivalence-class.md) is nonempty by [reflexivity](../../../../../reflexive-relation.md), and every $x$ belongs to $[x]$, so the classes cover $X$. If $z\in[x]\cap[y]$, then the [symmetric relation](../../../../../symmetric-relation.md) and [transitive relation](../../../../../transitive-relation.md) properties give $x\sim z\sim y$. Every $w\in[x]$ therefore satisfies $w\sim x\sim y$, so $[x]\subseteq[y]$; the reverse inclusion follows similarly. Thus two classes are either identical or disjoint. The distinct [equivalence classes](../../../../../equivalence-class.md) consequently form a [set partition](../../../../../set-partition.md) of $X$.

The divisibility-comparability relation is a [reflexive relation](../../../../../reflexive-relation.md) and a [symmetric relation](../../../../../symmetric-relation.md), but **is not an equivalence relation**. Indeed, $2\sim6$ and $6\sim3$, whereas neither $2\mid3$ nor $3\mid2$, so [transitivity](../../../../../transitive-relation.md) fails.

For the requested four-class construction, partition the positive integers into

$$
C_1=\{1\},\quad C_2=\{2\},\quad
C_3=\{3,5,7,\ldots\},\quad C_4=\{4,6,8,\ldots\}.
$$

Define $x\approx y$ exactly when they lie in the same $C_j$. Equality of the class label is an [equivalence relation](../../../../../equivalence-relation.md). **Its four classes are the two finite singletons and the two infinite parity classes displayed above.**

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
