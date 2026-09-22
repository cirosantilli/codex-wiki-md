<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The set $S(\mathbb N)$ consists of all [bijections](../../../../../bijection.md) $\mathbb N\to\mathbb N$. The composition of two bijections is a bijection, composition is associative, the identity map is an identity, and every bijection has an inverse, so $S(\mathbb N)$ is a [group](../../../../../group-split.md).

An element of $S_{\mathrm{fin}}(\mathbb N)$ has finite [support](../../../../../support-of-a-permutation.md). The support of a composition is contained in the union of the two supports, and a permutation and its inverse have the same support. The identity has empty support. Hence $S_{\mathrm{fin}}(\mathbb N)$ is a [subgroup](../../../../../subgroup.md).

Let $\sigma$ be a cycle and choose $n$ that it moves. Because $\sigma$ has finite support, the sequence

$$
n,\sigma(n),\sigma^2(n),\ldots
$$

must repeat. Since $\sigma$ is invertible, its first repetition returns to $n$; let the least positive return time be $l$. The cycle condition says that every moved point occurs in this orbit, so $\sigma^l$ fixes every point. No smaller positive power fixes $n$. Therefore

$$
\boxed{\operatorname{ord}(\sigma)=l},
$$

which is finite.

For $\tau\in S_{\mathrm{fin}}(\mathbb N)$, partition its finite support into the orbits of the [cyclic group](../../../../../cyclic-group.md) $\langle\tau\rangle$. On each orbit, let $\sigma_i$ agree with $\tau$ and fix every point outside that orbit. Then each $\sigma_i$ is a [permutation cycle](../../../../../permutation-cycle.md), their supports are pairwise disjoint, and

$$
\tau=\sigma_1\cdots\sigma_k.
$$

Disjoint cycles commute because at every point at most one of them acts nontrivially.

Writing $l_i=\operatorname{ord}(\sigma_i)$, a power $\tau^m$ is the identity exactly when every $\sigma_i^m$ is the identity, equivalently when every $l_i$ divides $m$. Thus

$$
\boxed{\operatorname{ord}(\tau)
=\operatorname{lcm}(l_1,\ldots,l_k)}.
$$

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
