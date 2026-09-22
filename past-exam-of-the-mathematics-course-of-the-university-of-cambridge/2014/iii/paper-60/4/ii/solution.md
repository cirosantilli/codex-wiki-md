<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $r$ be the input [Schmidt rank](../../../../../../schmidt-rank.md), so $\lambda_j=0$ for $j>r$ and $\sum_{j=1}^r\lambda_j=1$. If $r=d$, the output rank is already at most $r$. Otherwise, [Nielsen's pure-state conversion theorem](../../../../../../nielsen-s-pure-state-conversion-theorem.md) and [majorization](../../../../../../majorization.md) at $k=r$ give

$$
1=\sum_{j=1}^r\lambda_j\leq\sum_{j=1}^r\mu_j\leq\sum_{j=1}^d\mu_j=1.
$$

Thus all output coefficients beyond $r$ vanish, proving

$$
\boxed{\operatorname{Schmidt\ rank}(|\phi\rangle)\leq\operatorname{Schmidt\ rank}(|\psi\rangle).}
$$

This is [monotonicity of Schmidt rank under LOCC](../../../../../../monotonicity-of-schmidt-rank-under-locc.md). It also holds separately in any nonzero postselected branch: represent the input amplitudes by a matrix $C$; a local branch maps it to $ACB^T$, whose rank cannot exceed the rank of $C$. The deterministic result requested here follows already from the majorization criterion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
