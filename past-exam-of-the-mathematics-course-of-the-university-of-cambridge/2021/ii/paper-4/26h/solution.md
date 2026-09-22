<h1 id="26h/solution">Solution</h1>

↑ **Parent:** [26H](../26h.md)

The union bound gives $\mathbb P(\bigcup_{n\geq m}A_n)\leq\sum_{n\geq m}\mathbb P(A_n)\to0$. Taking the decreasing intersection proves the first [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md).

If $X_n\to X$ almost surely, then $1_{\{|X_n-X|>ε\}}\to0$ almost surely; [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives convergence of its expectation, hence convergence in probability.

If convergence in probability holds, any subsequence has a further one with $\mathbb P(|X_{n(k_r)}-X|>2^{-r})<2^{-r}$. Borel-Cantelli then gives almost-sure convergence. Conversely, failure in probability supplies a subsequence with probabilities bounded below by some positive constant, and no further subsequence can converge almost surely because that would imply convergence in probability.

## ↑ Ancestors (10)

1. [26H](../26h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
