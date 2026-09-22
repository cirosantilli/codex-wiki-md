<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [K-nearest neighbors algorithm](../../../../../../k-nearest-neighbors-algorithm.md) takes the majority label among the $k$ training features closest to the query, with a stated tie rule. Its data-dependent risk is the conditional test error given the training sample, and $R_n$ denotes its expectation over that sample.

For one nearest neighbour, condition on a feature value $X=x$ and couple the coincident nearest feature as $X_1=x$. The two labels are conditionally independent Bernoulli$(\eta(x))$, so their mismatch probability is

$$
2\eta(x)\{1-\eta(x)\}
\leq2\min\{\eta(x),1-\eta(x)\}.
$$

Integration over $X$ gives

$$
\boxed{R_n(\psi^{1\mathrm{NN}})\leq2R(\psi^{\mathrm{Bayes}}).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
