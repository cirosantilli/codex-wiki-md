<h1 id="26j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $L_t=\int_0^t\Lambda(u)\,du$, finite almost surely. Conditional on the intensity process, $N(t)$ is Poisson with mean and variance $L_t$. The [law of total expectation](../../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../../law-of-total-variance.md) give

$$
\mathbb EN(t)=\mathbb EL_t,\qquad\operatorname{Var}N(t)=\mathbb E[\operatorname{Var}(N(t)\mid\Lambda)]+\operatorname{Var}[\mathbb E(N(t)\mid\Lambda)]=\mathbb EL_t+\operatorname{Var}L_t.
$$

Consequently for a [Cox process](../../../../../../cox-process.md),

$$
\boxed{\operatorname{Var}N(t)\geq\mathbb EN(t).}
$$

These identities apply when the moments are finite; if the mean is finite but the integrated intensity has infinite variance, the count variance is infinite and the inequality still holds.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
