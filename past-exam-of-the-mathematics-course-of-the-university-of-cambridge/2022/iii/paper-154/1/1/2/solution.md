<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On the unit ball, part 1 controls the $L^2$ norm. Outside it, $|x|^\alpha\geq1$, so

$$
\int_{|x|>1}|u|^2\leq\int|x|^\alpha|u|^2.
$$

Hence $\|u\|_2\leq C\|u\|_\Sigma$, proving that the [embedding](../../../../../../../linear-map.md) $\Sigma\hookrightarrow L^2$ is [continuous](../../../../../../../continuous-function.md).

For compactness, let $(u_n)$ be bounded in $\Sigma$. On each ball, it is bounded in $H^1$, so the [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) gives a subsequence convergent in local $L^2$. The tail estimate

$$
\int_{|x|>R}|u_n|^2
\leq R^{-\alpha}\int|x|^\alpha|u_n|^2
$$

is uniform in $n$ and tends to zero as $R\to\infty$. A [diagonal argument](../../../../../../../diagonal-argument.md) therefore gives convergence in all of $L^2$. This is the [compact embedding of a confining-potential energy space](../../../../../../../compact-embedding-of-a-confining-potential-energy-space.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
