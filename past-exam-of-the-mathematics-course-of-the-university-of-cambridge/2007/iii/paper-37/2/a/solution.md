<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Count each unordered $k$-vertex set once. For each such set $A$, let $I_A$ be its [clique](../../../../../../clique-graph-theory.md) indicator in the [binomial random graph](../../../../../../binomial-random-graph.md). All $\binom k2$ required edges are independent, so

$$
X=\sum_{|A|=k}I_A,\qquad
\mu_n=\mathbb EX=\binom nkp^{\binom k2}.
$$

The [Markov inequality](../../../../../../markov-inequality.md), or [first moment method](../../../../../../first-moment-method.md), gives

$$
\mathbb P(X\ge1)\le\mathbb EX=\mu_n.
$$

Consequently

$$
\boxed{\mu_n\to0\quad\Longrightarrow\quad\mathbb P(X=0)\to1.}
$$

This argument works even if $k=k(n)$ varies. The [binomial coefficient](../../../../../../binomial-coefficient.md) shows that [cliques](../../../../../../clique-graph-theory.md) are counted as vertex sets, not as their different ordered listings.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
