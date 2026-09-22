<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $p=Cn^{-3/4}$. For any fixed $U\subseteq[n]$ with $|U|\geq3n/5$, let $X_U$ count copies of the [cycle graph](../../../../../../cycle-graph.md) $C_4$ in $G[U]$. Then

$$
\mu_U=3\binom{|U|}{4}p^4=\Theta(C^4n).
$$

Pairs of distinct $4$-cycles are dependent only when they share an edge. Classifying them by their common paths gives

$$
\Delta_U
=O(n^6p^7+n^5p^6+n^4p^5)
=O_C(n^{3/4}+n^{1/2}+n^{1/4})
=o(n).
$$

The first [Janson inequality](../../../../../../janson-inequality.md) therefore gives

$$
\mathbb P(X_U=0)\leq e^{-cC^4n}
$$

for an absolute $c>0$ and all sufficiently large $n$. Choose $C$ so that $cC^4>\log2+1$. A [union bound](../../../../../../boole-s-inequality.md) over the at most $2^n$ choices of $U$ shows that, [with high probability](../../../../../../with-high-probability.md), every set of at least $3n/5$ vertices contains a $C_4$.

Now greedily choose vertex-disjoint $4$-cycles until none remains. If fewer than $n/10$ were chosen, they would cover fewer than $2n/5$ vertices, leaving more than $3n/5$ vertices and hence another $C_4$. This contradiction proves that the greedy packing contains at least $n/10$ vertex-disjoint copies.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
