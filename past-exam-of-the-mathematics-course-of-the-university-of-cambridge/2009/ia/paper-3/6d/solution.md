<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

For a [permutation](../../../../../permutation.md) $\sigma$ of a finite set, start with a point $x$. Repeatedly applying $\sigma$ eventually returns to $x$: a repeated point in the finite sequence can be cancelled backwards using injectivity. The distinct successive points before that return form a cycle. If any point has not yet been used, repeat the construction there. The resulting orbits are disjoint and cover the set, so their cycles, including one-cycles for fixed points, give a [cycle decomposition of a permutation](../../../../../cycle-decomposition-of-a-permutation.md). Disjoint cycles commute because they act on different points.

Conjugation relabels a cycle:

$$
\gamma(x_1\ x_2\ \cdots\ x_n)\gamma^{-1}
=(\gamma x_1\ \gamma x_2\ \cdots\ \gamma x_n).
$$

Thus conjugate [permutations](../../../../../permutation.md) have the same [cycle type](../../../../../cycle-type.md). Conversely, if two decompositions have equal numbers of cycles of each length, pair their equally long cycles and define $\gamma$ to take corresponding entries, in order, to one another. Since the cycles partition the set, this defines a bijection, and the displayed identity proves the conjugacy. Hence **cycle type characterizes conjugacy in the symmetric [group](../../../../../group-split.md)**.

For $\tau=(a\ b)$, use the convention that the rightmost [permutation](../../../../../permutation.md) acts first. If $a,b$ are in different cycles, write those cycles as

$$
(a\ x_1\ldots x_p)(b\ y_1\ldots y_q).
$$

Left multiplication by $\tau$ changes the arrow into $a$ to an arrow into $b$, and the arrow into $b$ to an arrow into $a$. Following these arrows gives the single cycle

$$
(a\ x_1\ldots x_p\ b\ y_1\ldots y_q).
$$

No other cycles change, so $\ell(\tau\sigma)=\ell(\sigma)-1$. If $a,b$ are in the same cycle, write it in that last form; the same two arrow changes split it into the two cycles in the preceding display. Thus $\ell(\tau\sigma)=\ell(\sigma)+1$. Empty lists are allowed and produce one-cycles. This proves [transposition changes the cycle count by one](../../../../../transposition-changes-the-cycle-count-by-one.md) in all cases:

$$
\boxed{\ell(\tau\sigma)=\ell(\sigma)\pm1.}
$$

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
