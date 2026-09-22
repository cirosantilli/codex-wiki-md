<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Young permutation module](../../../../../../young-permutation-module.md) $M^\lambda$ has a [basis](../../../../../../basis.md) of [tabloids](../../../../../../tabloid.md), equivalently ordered row sets of sizes $\lambda_1,\ldots,\lambda_r$. A tabloid is fixed by $\sigma$ precisely when every cycle of $\sigma$ lies entirely in one row. Assigning a length-$q$ cycle to row $j$ contributes $x_j^q$. Distinct cycles can be assigned independently, so the [character](../../../../../../character-of-a-representation.md) is

$$
\boxed{\chi_{M^\lambda}(\sigma)=[x_1^{\lambda_1}\cdots x_r^{\lambda_r}]\prod_{q=1}^n(x_1^q+\cdots+x_r^q)^{m_q}.}
$$

Padding to $n$ variables with zero row sizes gives exactly the same coefficient. Explicitly, the [character of a Young permutation module](../../../../../../character-of-a-young-permutation-module.md) is

$$
\sum_{\substack{a_{qj}\ge0\colon\ \sum_j a_{qj}=m_q\\ \sum_q q a_{qj}=\lambda_j}}
\prod_q\frac{m_q!}{\prod_j a_{qj}!}.
$$

Here $a_{qj}$ counts the length-$q$ cycles assigned to row $j$. Rows remain distinguished even when their sizes are equal, so there is no further division by permutations of equal rows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
