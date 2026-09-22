<h1 id="5/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With $A_t=\int_0^t\mu(s)ds$, the product rule gives

$$
d(e^{-A_t}X_t)=e^{-A_t}X_t\sigma(t)dB_t,
$$

so $X_te^{-A_t}$ is a local martingale under $\mathbb P$.

Set $\theta(t)=\mu(t)/\sigma(t)$. This is bounded and compactly supported, so [Novikov condition](../../../../../../novikov-s-condition.md) holds and

$$
Z_\infty=\exp\left(-\int_0^\infty\theta(s)dB_s
-\frac12\int_0^\infty\theta(s)^2ds\right)
$$

defines a probability measure $d\mathbb Q=Z_\infty d\mathbb P$. By the [Girsanov theorem](../../../../../../girsanov-theorem.md), $W_t=B_t+\int_0^t\theta(s)ds$ is Brownian under $\mathbb Q$, and

$$
dX_t=X_t\sigma(t)dW_t.
$$

Thus **$X$ is a local martingale under $\mathbb Q$**.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
