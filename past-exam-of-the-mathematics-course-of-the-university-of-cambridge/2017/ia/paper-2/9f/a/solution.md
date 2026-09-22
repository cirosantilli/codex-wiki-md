<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [binomial theorem](../../../../../../binomial-theorem.md) makes the sum of the proposed [probability mass function](../../../../../../probability-mass-function.md) equal to $(p+1-p)^N=1$; every term is nonnegative. Realize the associated [binomial distribution](../../../../../../binomial-distribution.md) as $K=B_1+\cdots+B_N$, where the $B_j$ are [independent](../../../../../../independent-random-variables.md) variables with the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $p$. Each has [expected value](../../../../../../expected-value.md) $p$ and [variance](../../../../../../variance-split.md) $p(1-p)$. [Linearity of expectation](../../../../../../linearity-of-expectation.md) and [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md) yield

$$
\boxed{\mathbb EK=Np,\qquad\operatorname{Var}K=Np(1-p).}
$$

At $p=0$ or $p=1$ this is a constant [random variable](../../../../../../random-variable-split.md); the same formulas apply, with the endpoint mass understood by continuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
