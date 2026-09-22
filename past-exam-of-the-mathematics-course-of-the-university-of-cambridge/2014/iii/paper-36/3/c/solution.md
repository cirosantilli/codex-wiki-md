<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the chain rule for conditional densities. With $x_0=x_1=0$, the [likelihood function](../../../../../../likelihood-function.md) of the nondegenerate observations is

$$
\boxed{L(a,b;x_1,\ldots,x_n)=(2\pi)^{-(n-1)/2}\exp\left[-\frac12\sum_{t=0}^{n-2}(x_{t+2}-ax_{t+1}-bx_t)^2\right].}
$$

The first residual is $x_2$ and carries no parameter information. There is no ordinary joint Lebesgue density for $X_1,\ldots,X_n$ because $X_1=0$ deterministically; this expression is the conditional [likelihood function](../../../../../../likelihood-function.md) given the fixed initial values, or the [likelihood function](../../../../../../likelihood-function.md) on $x_2,\ldots,x_n$. The initial point mass is parameter independent and has no effect on inference. This is the [conditional likelihood of an initialized Gaussian AR(2) process](../../../../../../conditional-likelihood-of-an-initialized-gaussian-ar-2-process.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
