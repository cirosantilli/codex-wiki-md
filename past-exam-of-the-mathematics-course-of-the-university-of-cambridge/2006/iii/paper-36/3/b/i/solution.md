<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Count each unordered triple once. For a three-element [vertex set](../../../../../../../vertex-set.md) $S$, let $I_S$ indicate that its three [edges](../../../../../../../edge-of-a-graph.md) are present. Then $X=\sum_{|S|=3}I_S$ and

$$
\mathbb E X^2=\sum_{S,T}\mathbb E[I_SI_T].
$$

If $|S\cap T|=\ell$, their edge sets have $\binom\ell2$ edges in common, so their union contains $6-\binom\ell2$ distinct [edges](../../../../../../../edge-of-a-graph.md). Independence gives $\mathbb E[I_SI_T]=p^{6-\binom\ell2}$. There are $\binom n3\binom3\ell\binom{n-3}{3-\ell}$ such ordered pairs: choose $S$, its shared vertices, and the remaining vertices of $T$. Thus

$$
\boxed{\mathbb E X^2=
\binom n3\sum_{\ell=0}^3
\binom3\ell\binom{n-3}{3-\ell}
p^{6-\binom\ell2}}.
$$

This overlap count is the basis of [triangle variance in a binomial random graph](../../../../../../../triangle-variance-in-a-binomial-random-graph.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 36](../../../../paper-36-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
