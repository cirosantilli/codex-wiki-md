<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) states that for independent identically distributed integrable random variables,

$$
\frac{S_n}{n}\longrightarrow\mu
\quad\text{almost surely}.
$$

To prove it, set $Y_n=X_n\mathbf1_{\{|X_n|\leq n\}}$. The tail-sum formula gives $\sum_n\mathbb P(X_n\ne Y_n)<\infty$, so the [Borel-Cantelli lemmas](../../../../../../borel-cantelli-lemmas.md) make the two sequences eventually equal. Also

$$
\sum_{n=1}^\infty\frac{\operatorname{Var}(Y_n)}{n^2}
\leq\mathbb E\left[
X_1^2\sum_{n\geq|X_1|}\frac1{n^2}\right]
\leq C\mathbb E|X_1|<\infty.
$$

The [Kolmogorov convergence theorem](../../../../../../kolmogorov-convergence-theorem.md) implies that $\sum_n(Y_n-\mathbb EY_n)/n$ converges almost surely, and [Kronecker lemma](../../../../../../kronecker-lemma.md) yields

$$
\frac1n\sum_{j=1}^n(Y_j-\mathbb EY_j)\to0.
$$

Finally $\mathbb EY_n\to\mu$, so the [Cesaro mean](../../../../../../cesaro-mean.md) of these expectations tends to $\mu$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
