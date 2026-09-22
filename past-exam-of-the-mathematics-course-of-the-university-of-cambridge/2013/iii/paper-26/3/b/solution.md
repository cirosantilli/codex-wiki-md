<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A connection to a box boundary can be witnessed by a finite self-avoiding open path stopped at its first boundary hit. On the event of reaching radius $m+n$, split such a path at its first [graph vertex](../../../../../../vertex-graph-theory.md) $z\in\partial\Lambda_n$. Its prefix witnesses connection from zero to $z$ within $\Lambda_n$. Its remaining segment reaches a point $y$ with $\|y\|_\infty=m+n$, so $\|y-z\|_\infty\geq m$; truncate it at its first hit of $z+\partial\Lambda_m$. The two witnessing [edge](../../../../../../edge-of-a-graph.md) sets are disjoint, giving [disjoint occurrence of increasing events](../../../../../../disjoint-occurrence-of-increasing-events.md).

Use the [BK inequality](../../../../../../van-den-berg-kesten-inequality.md): for increasing finite-coordinate events in a Bernoulli [product measure](../../../../../../product-measure.md), $P(A\mathbin\square B)\leq P(A)P(B)$, where the square means disjoint open-edge witnesses. For each fixed $z$, the first event has probability at most $\beta_n$, and the second has probability exactly $\beta_m$ by [translation invariance](../../../../../../translation-invariance.md). A [union bound](../../../../../../boole-s-inequality.md) over $z$ gives

$$
\boxed{\beta_{m+n}\leq|\partial\Lambda_n|\beta_n\beta_m}.
$$

The two boxes can overlap, so replacing BK by an independence claim would be incorrect. Restricting each event to paths stopped at its local boundary makes all the relevant coordinate sets finite, as required by the stated inequality.

Put $x_n=\log\beta_n$ and $\alpha_n=\log|\partial\Lambda_n|$. Here $|\partial\Lambda_n|=(2n+1)^d-(2n-1)^d$, so $\alpha_n=O(\log n)=o(n)$. A fixed straight open path of length $n$ gives $p^n\leq\beta_n\leq1$. Part (a) therefore gives the [almost-subadditive percolation decay rate](../../../../../../almost-subadditive-percolation-decay-rate.md)

$$
\boxed{\lambda=-\lim_{n\to\infty}\frac1n\log\beta_n\in[0,-\log p]}.
$$

In particular the limit is finite for the prescribed $0<p<1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
