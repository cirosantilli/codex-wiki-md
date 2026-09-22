<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite set $S=\{s_1,\ldots,s_k\}$ of [vectors](../../../../../../vector.md) in a real [vector space](../../../../../../vector-space-split.md), its [span](../../../../../../linear-span.md) is the set of all [linear combinations](../../../../../../linear-combination.md):

$$
\boxed{\operatorname{Sp}(S)=\left\{\sum_{i=1}^ka_is_i:a_i\in\mathbb R\right\}.}
$$

The [span](../../../../../../linear-span.md) of the empty set is $\{0\}$. The set $S$ is [linearly independent](../../../../../../linear-independence.md) if $\sum_i a_is_i=0$ implies $a_i=0$ for every $i$. It is a [spanning set](../../../../../../spanning-set.md) for $V$ if $\operatorname{Sp}(S)=V$. A [basis](../../../../../../basis.md) is both a [linearly independent](../../../../../../linear-independence.md) set and a [spanning set](../../../../../../spanning-set.md).

For [basis extension](../../../../../../basis-extension.md), start with the given [linearly independent](../../../../../../linear-independence.md) set. If it does not span $V$, choose $v\notin\operatorname{Sp}(S)$ and adjoin it. The enlarged set remains [linearly independent](../../../../../../linear-independence.md): a relation $av+\sum_i a_is_i=0$ with $a\ne0$ would express $v$ as a [linear combination](../../../../../../linear-combination.md) of $S$, a contradiction; if $a=0$, independence of $S$ forces all other coefficients to be zero.

Repeat whenever the current [span](../../../../../../linear-span.md) is proper. Each step increases the set's size by one, while the allowed bound says its size cannot exceed $\dim V$. Thus the process terminates with a [linearly independent](../../../../../../linear-independence.md) set spanning $V$, hence a [basis](../../../../../../basis.md) containing the original set. This also covers an initially empty set and the zero-dimensional [vector space](../../../../../../vector-space-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
