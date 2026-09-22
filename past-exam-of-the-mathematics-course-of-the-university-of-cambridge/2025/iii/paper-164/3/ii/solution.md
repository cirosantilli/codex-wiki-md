<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mathcal Q$ be the set of valid quintuples and choose $(A_1,\ldots,A_5)$ uniformly from $\mathcal Q$. Then

$$
H(A_1,\ldots,A_5)=\log|\mathcal Q|.
$$

Apply [Shearer's inequality](../../../../../../shearer-s-inequality.md) to the ten pairs $\{i,j\}\subseteq[5]$. Every index occurs in four pairs, so

$$
4H(A_1,\ldots,A_5)\leq\sum_{1\leq i<j\leq5}H(A_i,A_j).
$$

Put $U_{ij}=A_i\cup A_j$. Since $U_{ij}\in\mathcal A$, it has cardinality $k$. For each element of $U_{ij}$, its membership bits in $(A_i,A_j)$ are one of $(1,0),(0,1),(1,1)$; outside $U_{ij}$ they are forced to be $(0,0)$. Thus at most $3^k$ ordered pairs have any prescribed union. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md), [conditional entropy](../../../../../../conditional-entropy.md), and the support bound for [information entropy](../../../../../../information-entropy.md) give

$$
H(A_i,A_j)
\leq H(U_{ij})+H(A_i,A_j\mid U_{ij})
\leq\log|\mathcal A|+k\log3,
$$

because every $U_{ij}$ belongs to $\mathcal A$. There are ten pairs, hence

$$
\log|\mathcal Q|
\leq\frac{10}{4}\bigl(\log|\mathcal A|+k\log3\bigr).
$$

Exponentiating proves

$$
|\mathcal Q|\leq3^{5k/2}|\mathcal A|^{5/2},
$$

which is the five-variable case of the [entropy bound for pairwise-union tuples](../../../../../../entropy-bound-for-pairwise-union-tuples.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
