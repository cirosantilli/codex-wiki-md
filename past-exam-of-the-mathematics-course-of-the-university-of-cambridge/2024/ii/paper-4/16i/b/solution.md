<h1 id="16i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $\aleph_0=|\omega|$, let $\aleph_{\alpha+1}$ be the least cardinal greater than $\aleph_\alpha$, and at a [limit](../../../../../../limit-of-a-function.md) take the least cardinal above all earlier $\aleph_\gamma$. In ZFC every set is well-orderable, so every infinite cardinal is an initial ordinal and equals a unique $\aleph_\alpha$.

By transfinite induction on infinite well-ordered cardinals $\kappa$, order $\kappa\times\kappa$ first by $\max(\xi,\eta)$ and then lexicographically. Every proper initial segment has cardinal below $\kappa$, using the inductive hypothesis for smaller infinite cardinals. Hence this well-order has cardinal at most $\kappa$, while the diagonal gives the reverse inequality, so $\kappa^2=\kappa$. Therefore, for $\aleph_\alpha\leq\aleph_\beta$,

$$
\aleph_\alpha+\aleph_\beta
=\aleph_\alpha\aleph_\beta=\aleph_\beta.
$$

Finally suppose nonempty $x$ had a set $y$ containing every set equinumerous with $x$. For every ordinal $\gamma$, replacing each $z\in x$ by a tagged ordered pair $(\gamma,z)$ gives a set $t_\gamma$ equinumerous with $x$ whose rank is at least $\gamma$. Then every $t_\gamma$ would belong to $y$, so the ranks of members of $y$ would be unbounded in the ordinals, contradicting the ordinal rank of $y$. This proves the displayed sentence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16I](../../16i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
