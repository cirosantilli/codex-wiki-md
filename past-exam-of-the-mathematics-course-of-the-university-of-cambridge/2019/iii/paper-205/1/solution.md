<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A procedure controls the [familywise error rate](../../../../../familywise-error-rate.md) at level $\alpha$ when, for every configuration of true nulls $I$,

$$
\mathbb P(\text{at least one }H_i, i\in I,
\text{ is rejected})\leq\alpha.
$$

Let $i_*=\min I$. The step-down procedure can reject any true null only if it reaches and rejects $H_{i_*}$, which requires $p_{i_*}\leq\alpha$. Since a valid [p-value](../../../../../p-value.md) under its null satisfies $\mathbb P(p_{i_*}\leq\alpha)\leq\alpha$, the procedure controls FWER without any assumption on dependence among the p-values.

A distribution $P$ has the [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md) $G$ when every [D-separation](../../../../../d-separation.md) statement $A\mathrel{\perp_G}B\mid C$ implies the corresponding [conditional independence](../../../../../conditional-independence.md) $Z_A\perp\!\!\!\perp Z_B\mid Z_C$ under $P$.

If $G\in\mathcal S$ has nonadjacent vertices $j,k$, choose a [topological ordering](../../../../../topological-ordering.md). Suppose $j$ precedes $k$. Then $j$ is a non-descendant and non-parent of $k$, so the directed local Markov property gives

$$
Z_j\perp\!\!\!\perp Z_k\mid Z_{\operatorname{pa}_G(k)}.
$$

The reversed ordering case is analogous. Hence

$$
H_0\subseteq\bigcup_{S\subseteq[p]\setminus\{j,k\}}H_S.
$$

Use the [intersection-union test](../../../../../intersection-union-test.md): reject $H_0$ exactly when $p_S\leq\alpha$ for every $S$. Under $H_0$, at least one $H_{S_*}$ is true, so

$$
\mathbb P(\text{false rejection of }H_0)
\leq\mathbb P(p_{S_*}\leq\alpha)\leq\alpha.
$$

This is nontrivial because it rejects whenever every tested conditional independence is rejected.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
