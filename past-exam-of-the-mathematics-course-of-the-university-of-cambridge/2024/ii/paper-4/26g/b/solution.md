<h1 id="26g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Y_n=n^{-1}\sum_{i=1}^n|X_i|$. Truncate each $|X_i|$ at a level $K$. The average of the truncated parts is at most $K$, while the expected average of the tails is

$$
\mathbb E[|X_1|\mathbf1_{|X_1|>K}],
$$

independently of $n$. Markov's inequality then shows that $(Y_n)$ is uniformly integrable as $K\to\infty$. Since $|S_n|/n\leq Y_n$, the [sequence](../../../../../../sequence.md) $(S_n/n)$ is uniformly integrable.

Convergence in probability to the constant $\mathbb EX_1$, together with uniform integrability, implies convergence of first absolute moments by the Vitali convergence theorem. Hence

$$
\boxed{\mathbb E\left|\frac{S_n}{n}-\mathbb EX_1\right|\to0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26G](../../26g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
