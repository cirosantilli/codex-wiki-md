<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $I_0=B^c$ and $m_0=|I_0|$. Each $q_j$ with $j\in I_0$ is a valid [p-value](../../../../../../p-value.md) by the argument in part c. If the [Holm step-down procedure](../../../../../../holm-bonferroni-method.md) selects any index from $I_0$, let $r$ be the rank of the first such index. All $r-1$ earlier selections belong to $B$, so

$$
r\leq|B|+1=p-m_0+1,
\qquad p-r+1\geq m_0.
$$

Selection through rank $r$ implies

$$
q_{\tau(r)}\leq\frac\alpha{p-r+1}\leq\frac\alpha{m_0}.
$$

Consequently

$$
\mathbb P(\widehat B\not\subseteq B)
\leq\mathbb P\!\left(\min_{j\in I_0}q_j\leq\frac\alpha{m_0}\right)
\leq\sum_{j\in I_0}\mathbb P\!\left(q_j\leq\frac\alpha{m_0}\right)
\leq\alpha.
$$

**Thus the procedure controls the [familywise error rate](../../../../../../familywise-error-rate.md) without requiring independence among the p-values.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
