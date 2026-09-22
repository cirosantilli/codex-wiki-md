<h1 id="7d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Because $n$ is not a prime power, distinct primes $p<q$ divide $n$. By Cauchy's theorem, $G$ has [subgroups](../../../../../../subgroup.md) $H,K$ of orders $p,q$. Combine the two [coset action](../../../../../../coset-action.md)s to obtain

$$
G\longrightarrow S_{n/p}\times S_{n/q}
\longrightarrow S_{n/p+n/q}.
$$

The kernel of the first action is contained in $H$, and that of the second is contained in $K$. Their intersection is trivial because $H\cap K=\{1\}$, so the combined action is faithful.

Since $p\geq2$, $q\geq3$, and $n\geq6$,

$$
\frac np+\frac nq
\leq\frac{5n}{6}
\leq n-1.
$$

Adding fixed points embeds this symmetric [group](../../../../../../group-split.md) into $S_{n-1}$. Thus every [group](../../../../../../group-split.md) of non-prime-power order $n$ is a [subgroup](../../../../../../subgroup.md) of $S_{n-1}$, as summarized by [symmetric-group embedding at one less than the group order](../../../../../../symmetric-group-embedding-at-one-less-than-the-group-order.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
