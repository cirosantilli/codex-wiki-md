<h1 id="1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [random walk](../../../../../../random-walk.md) $S_n$ is a [martingale](../../../../../../martingale-split.md), since its integrable increments are independent of the past and have mean zero. For the [bounded stopping time](../../../../../../bounded-stopping-time.md) $n\wedge\eta$, the bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md), proved in the next question, gives $\mathbb ES_{n\wedge\eta}=x$.

If $0<x<r$, the value immediately before exit lies in $(0,r)$, so

$$
|S_\eta|\leq r+|X_\eta|.
$$

Before exit the stopped value has absolute value less than $r$, and after exit it equals $S_\eta$. Consequently $|S_{n\wedge\eta}|\leq r+|X_\eta|$ for every $n$. This is an integrable dominating [random variable](../../../../../../random-variable-split.md) by the preceding part. Since $\eta<\infty$ with probability one, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{\mathbb ES_\eta=\lim_{n\to\infty}\mathbb ES_{n\wedge\eta}=x.}
$$

For $r\leq x$, $S_\eta=S_0=x$ directly, without any convention about $X_0$. Thus the expected stopped position is well-defined and has the stated value for every $r>0$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
