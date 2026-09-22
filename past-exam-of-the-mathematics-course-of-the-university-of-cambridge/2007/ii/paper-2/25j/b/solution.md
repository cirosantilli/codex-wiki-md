<h1 id="25j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Convergence in probability](../../../../../../convergence-in-probability.md) supplies a subsequence $X_{n_k}$ converging [almost surely](../../../../../../almost-sure-convergence.md) to $X$: choose it so $\Pr(|X_{n_k}-X|>2^{-k})<2^{-k}$, then apply the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md). For each fixed $N$, the tail of this subsequence lies in $\sigma(X_n:n\ge N)$, and its almost sure limit is $X$. Thus $X$ has a version measurable with respect to the completed tail sigma-field of the independent sequence.

By [Kolmogorov's zero–one law](../../../../../../kolmogorov-s-zero-one-law.md), every event in that tail sigma-field has [probability](../../../../../../probability.md) zero or one. Consequently $\Pr(X\le r)\in\{0,1\}$ for every rational $r$. Since $X$ is a finite real [random variable](../../../../../../random-variable-split.md), its distribution function has limits zero and one at the two infinities; monotonicity then identifies a single threshold $c$ with $\Pr(X=c)=1$. Hence **$X$ is [almost surely](../../../../../../almost-sure-convergence.md) constant**. Completion only adds null events and does not alter the zero-one conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25J](../../25j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
