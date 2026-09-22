<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $q>p$, let $M=\sup_{n\geq0}S_n$, including $S_0=0$. It is a nonnegative integer-valued [random variable](../../../../../../../random-variable-split.md), possibly infinite before the following estimate. The [tail-sum formula for expectation](../../../../../../../tail-sum-formula-for-expectation.md) and part (i) give

$$
\mathbb EM=\sum_{k\geq1}\mathbb P(M\geq k)
\leq\sum_{k\geq1}(p/q)^k
=\frac{p/q}{1-p/q}=\frac p{q-p}.
$$

Thus $\boxed{\mathbb E\sup_{n\geq0}S_n\leq p/(q-p)}$, and the supremum is finite [almost surely](../../../../../../../almost-sure-convergence.md). The sum identity follows by writing $M=\sum_{k\geq1}\mathbf1_{\{M\geq k\}}$ and applying [monotone convergence theorem](../../../../../../../monotone-convergence-theorem.md). If the printed supremum is read literally over $n\geq1$, its positive part has exactly the same positive-level tails and its negative part is bounded by one. The same upper bound on its [expected value](../../../../../../../expected-value.md) remains valid.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
