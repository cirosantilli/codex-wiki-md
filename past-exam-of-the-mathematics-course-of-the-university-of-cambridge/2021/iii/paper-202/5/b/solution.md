<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md)

$$
g(x)=\int_0^x\exp\left(-2\int_0^yb(z)dz\right)dy.
$$

Then $g'>0$, so $g$ is strictly increasing, and

$$
\frac12g''+bg'=0.
$$

By [Itô formula](../../../../../../ito-s-lemma.md),

$$
dY_t=d(g(X_t))=g'(X_t)dW_t,
$$

so $Y=g(X)$ is a [local martingale](../../../../../../local-martingale.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
