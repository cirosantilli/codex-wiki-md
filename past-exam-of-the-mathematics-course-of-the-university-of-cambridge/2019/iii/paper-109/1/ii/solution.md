<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mathcal A\subseteq[n]^{(r)}$ be an [intersecting family](../../../../../../intersecting-family.md), with $n\geq2r$. By the [Iterated local LYM inequality](../../../../../../iterated-local-lym-inequality.md), its upper shadow in level $n-r$ satisfies

$$
|\nabla^{,n-2r}\mathcal A|
\geq
\frac{\binom n{n-r}}{\binom nr}|\mathcal A|
=|\mathcal A|.
$$

The family of complements $\mathcal A^c=\{[n]\setminus A:A\in\mathcal A\}$ also lies in level $n-r$ and has cardinality $|\mathcal A|$. It is disjoint from the upper shadow: if $A\subseteq[n]\setminus B$ for $A,B\in\mathcal A$, then $A\cap B=\varnothing$, contradicting intersection. Both families fit inside the $(n-r)$th level, so

$$
2|\mathcal A|\leq\binom n{n-r}=\binom nr.
$$

Thus replacing the [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md) by Local LYM gives only

$$
\boxed{|\mathcal A|\leq\frac12\binom nr.}
$$

This agrees with the [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) when $n=2r$ but is weaker when $n>2r$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
