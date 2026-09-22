<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $a_n=|\mathcal P_n|$ for the number of labelled $r$-[uniform hypergraphs](../../../../../../uniform-hypergraph.md) with the [hereditary hypergraph property](../../../../../../hereditary-hypergraph-property.md), so $d_n=a_n^{1/\binom nr}$ for $n\geq r$. The assertion is nonincrease; strict decrease need not hold, since allowing all [uniform hypergraphs](../../../../../../uniform-hypergraph.md) gives $d_n=2$.

If $a_n=0$, heredity forces $a_{n+1}=0$. If $a_{n+1}=0$, the desired inequality is immediate. Otherwise choose $H$ uniformly from $\mathcal P_{n+1}$ and record its edge indicators as a [random vector](../../../../../../random-vector.md) $X=(X_e)_{e\in[n+1]^{(r)}}$. Its [information entropy](../../../../../../information-entropy.md), with any fixed logarithm base, is $H(X)=\log a_{n+1}$. Deleting a vertex $v$ gives the restriction $X^{(v)}$ to the edges avoiding $v$. By heredity and relabelling, this restriction has at most $a_n$ possible values, so $H(X^{(v)})\leq\log a_n$.

Each edge coordinate occurs in exactly $n+1-r$ of these restrictions. For completeness, order all the edge coordinates. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) expands a restriction entropy as a sum of conditional coordinate entropies. The predecessors retained in a restriction form a subset of all predecessors, and [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md); hence each restriction term is at least the corresponding full-vector term. Summing over the restrictions counts each full-vector term $n+1-r$ times. This proves the needed [Shearer inequality](../../../../../../shearer-s-inequality.md):

$$
(n+1-r)\log a_{n+1}\leq\sum_{v=1}^{n+1}H(X^{(v)})\leq(n+1)\log a_n.
$$

Since $\binom{n+1}r=\frac{n+1}{n+1-r}\binom nr$, division gives $\log d_{n+1}\leq\log d_n$. Therefore the [normalized speed of a hereditary hypergraph property](../../../../../../normalized-speed-of-a-hereditary-hypergraph-property.md) satisfies

$$
\boxed{d_{n+1}\leq d_n\qquad(n\geq r).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
