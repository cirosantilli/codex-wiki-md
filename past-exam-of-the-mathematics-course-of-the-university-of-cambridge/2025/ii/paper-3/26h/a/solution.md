<h1 id="26h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $Z_n=|X_n-X|$. If $Z_n\to0$ in probability, then for $0<\varepsilon<1$,

$$
\mathbb E(Z_n\wedge1)
\leq\varepsilon+\mathbb P(Z_n>\varepsilon).
$$

Taking the upper limit and then letting $\varepsilon\downarrow0$ proves that the expectations tend to zero. Conversely,

$$
\mathbb P(Z_n>\varepsilon)
\leq\frac{\mathbb E(Z_n\wedge1)}{\varepsilon\wedge1},
$$

so expectation convergence implies convergence in probability. This proves the [bounded-metric characterization of convergence in probability](../../../../../../bounded-metric-characterization-of-convergence-in-probability.md).

For the subsequence assertion, choose $n_k$ so that

$$
\mathbb P(|X_{n_k}-X|>2^{-k})<2^{-k}.
$$

The first [Borel-Cantelli lemmas](../../../../../../borel-cantelli-lemmas.md) then says that only finitely many of these events occur almost surely. Hence

$$
|X_{n_k}-X|\leq2^{-k}
$$

eventually almost surely, and $X_{n_k}\to X$ almost surely. This is the [almost-sure subsequence from convergence in probability](../../../../../../almost-sure-subsequence-from-convergence-in-probability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26H](../../26h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
