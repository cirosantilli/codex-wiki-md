<h1 id="17h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Construct a [bipartite graph](../../../../../../bipartite-graph.md) with left vertices $A_1,\ldots,A_k$, right vertices $B_1,\ldots,B_k$, and an edge $A_iB_j$ exactly when $A_i\cap B_j\ne\varnothing$. For $S\subseteq[k]$, every point of $\bigcup_{i\in S}A_i$ lies in some $B_j$ adjacent to one of those $A_i$. Thus

$$
\bigcup_{i\in S}A_i
\subseteq
\bigcup_{j\in N(S)}B_j.
$$

Using finite additivity of [Lebesgue measure](../../../../../../lebesgue-measure.md) and the equal-volume hypotheses,

$$
\frac{|S|}{k}
=\operatorname{vol}\left(\bigcup_{i\in S}A_i\right)
\leq
\operatorname{vol}\left(\bigcup_{j\in N(S)}B_j\right)
=\frac{|N(S)|}{k}.
$$

Hence $|N(S)|\geq|S|$ for every $S$. The [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) supplies a [perfect matching](../../../../../../perfect-matching.md), which has the form $A_iB_{\sigma(i)}$ for a permutation $\sigma$ of $[k]$. Every matched edge means precisely that $A_i\cap B_{\sigma(i)}\ne\varnothing$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
