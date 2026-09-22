<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After the sum-product messages have been computed, draw exact independent posterior configurations by sampling a root from its marginal and then sampling each child from its conditional distribution given its parent. For sample $m$, set

$$
I_m=\mathbf1\left\{\sum_{i\in V}X_i^{(m)}>2|V_2|\right\},
\qquad
\widehat q=\frac1N\sum_{m=1}^NI_m.
$$

Then $\widehat q$ is unbiased and

$$
\operatorname{Var}(\widehat q)=\frac{q(1-q)}N.
$$

Taking $N=1000$ attains the required bound. Message computation costs $O(|V|)$ and each exact sample costs $O(|V|)$, so with the prescribed fixed number of samples the overall cost is

$$
\boxed{O(|V|).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
