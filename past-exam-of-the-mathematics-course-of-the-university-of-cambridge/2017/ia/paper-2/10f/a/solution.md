<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Markov's inequality](../../../../../../markov-inequality.md) to the nonnegative [random variable](../../../../../../random-variable-split.md) $e^{\lambda X}$, since $X>t$ implies $e^{\lambda X}>e^{\lambda t}$:

$$
\boxed{\mathbb P(X>t)\leq e^{-\lambda t}\mathbb E[e^{\lambda X}].}
$$

This [exponential Markov bound](../../../../../../exponential-markov-bound.md) remains true, though uninformative, when the [expected value](../../../../../../expected-value.md) is infinite. For a [standard normal distribution](../../../../../../standard-normal-distribution.md), completion of the square gives its [moment-generating function](../../../../../../moment-generating-function.md)

$$
\mathbb E[e^{\lambda X}]
=\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{\lambda x-x^2/2}\,dx
=e^{\lambda^2/2}.
$$

Minimize $\lambda^2/2-\lambda t$ over positive $\lambda$; the choice $\lambda=t$ gives the [Chernoff bound](../../../../../../chernoff-bound.md)

$$
\boxed{\mathbb P(X>t)\leq e^{-t^2/2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
