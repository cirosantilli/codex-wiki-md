<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [Poisson distribution](../../../../../../../poisson-distribution.md) of parameter $\lambda$, its [probability generating function](../../../../../../../probability-generating-function.md) is $\exp\{\lambda(z-1)\}$. Applying the [law of total expectation](../../../../../../../law-of-total-expectation.md) to the [Poisson mixture](../../../../../../../poisson-mixture.md) gives

$$
G_N(z)=\mathbb E\{\mathbb E(z^N\mid\lambda)\}=\mathbb E e^{(z-1)\lambda}.
$$

Thus

$$
\boxed{G_N(z)=M_\lambda(z-1).}
$$

For $|z|\le1$ the absolute value of the integrand is bounded by one, so this identity always exists as a [Laplace transform](../../../../../../../laplace-transform.md) of the positive mixing variable. An extension to $z>1$ requires the corresponding [moment-generating function](../../../../../../../moment-generating-function.md) to be finite; the conditional computation itself does not guarantee positive exponential moments.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
