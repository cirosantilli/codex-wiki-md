<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [standard notation for forcing](../../../../../../standard-notation-for-forcing.md), so $q\leq p$ means that $q$ is stronger. Let $\check p$ be the [canonical forcing name](../../../../../../canonical-forcing-name.md) for the ground-model condition $p$. Define

$$
\boxed{\tau=\{(\check p,q):p,q\in\mathbb P,\ q\perp p\}.}
$$

Here $q\perp p$ means that they are [incompatible forcing conditions](../../../../../../incompatible-forcing-conditions.md). The checks and their collection are formed by recursion and [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) in $M$, and the displayed set is selected by [axiom schema of separation](../../../../../../axiom-schema-of-specification.md), so this is a [forcing name](../../../../../../forcing-name.md) in $M$.

By [evaluation of a forcing name](../../../../../../evaluation-of-a-forcing-name.md),

$$
\operatorname{val}(\tau,G)=\{p\in\mathbb P:\exists q\in G\ (q\perp p)\}.
$$

If $p\in G$, directedness of the [generic filter](../../../../../../generic-filter.md) gives a common stronger condition for $p$ and each $q\in G$, so $p$ is absent from this value.

Conversely, for fixed $p\in\mathbb P$ the set

$$
D_p=\{q\in\mathbb P:q\leq p\text{ or }q\perp p\}
$$

is a [dense subset of a forcing order](../../../../../../dense-subset-of-a-forcing-order.md) belonging to $M$. A condition incompatible with $p$ is already in it, and one compatible with $p$ has a common extension below $p$. Genericity supplies $q\in G\cap D_p$. If $p\notin G$, upward closure of $G$ rules out $q\leq p$, hence $q\perp p$. Therefore

$$
\boxed{\operatorname{val}(\tau,G)=\mathbb P\setminus G.}
$$

This [forcing name for the complement of a generic filter](../../../../../../forcing-name-for-the-complement-of-a-generic-filter.md) works without a separativity assumption on the order.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
