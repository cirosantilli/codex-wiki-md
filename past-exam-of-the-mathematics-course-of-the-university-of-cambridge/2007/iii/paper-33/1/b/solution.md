<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) in the form needed here states that a nonnegative [supermartingale](../../../../../../supermartingale.md) with uniformly bounded [expectations](../../../../../../expected-value.md) converges almost surely to a finite integrable limit. Here $\mathbb E X_n=\mu([0,1))$ for all $n$, so it applies to $X_n$. The ordinary [Fatou lemma](../../../../../../fatou-s-lemma.md) gives

$$
X_n\longrightarrow X_\infty\quad\lambda\text{-almost surely},\qquad
\mathbb E X_\infty\leq\mu([0,1)).
$$

For fixed $n$, apply the [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md) to the nonnegative variables $X_m$, $m\geq n$. The [martingale](../../../../../../martingale-split.md) property makes each $\mathbb E[X_m\mid\mathcal F_n]$ equal to $X_n$, hence

$$
\boxed{\mathbb E[X_\infty\mid\mathcal F_n]\leq X_n\quad\lambda\text{-almost surely}.}
$$

The inequality is simultaneous for all $n$ after removing a countable union of null sets. Equality of [expectations](../../../../../../expected-value.md) in the limit has not been assumed; it can fail for a [measure](../../../../../../measure.md) with a singular component.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
