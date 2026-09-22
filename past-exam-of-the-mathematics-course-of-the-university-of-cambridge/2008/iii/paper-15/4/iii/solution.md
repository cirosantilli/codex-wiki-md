<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the same random variables for the edge cover of $G$. For a fixed color vector, any two compatible candidate vertices cannot be adjacent: an edge in a covering graph would force different colors at that coordinate. Thus the compatible candidates form an [independent set](../../../../../../independent-set-graph-theory.md) and there are at most $\alpha$ of them. By the [maximum entropy on a finite alphabet](../../../../../../maximum-entropy-on-a-finite-alphabet.md), $H(X\mid Y_1,\ldots,Y_\ell)\leq\log_2\alpha$.

Consequently the [mutual information](../../../../../../mutual-information.md) is at least $\log_2n-\log_2\alpha$, while the marginal and conditional-entropy bounds from part (i) make it at most $n^{-1}\sum_iw(G_i)$. The [entropy weight of a graph cover](../../../../../../entropy-weight-of-a-graph-cover.md) bound follows:

$$
\boxed{\sum_iw(G_i)\geq n\log_2(n/\alpha).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
