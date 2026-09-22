<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [Markov property](../../../../../../markov-property.md), all factors in the stationary [likelihood function](../../../../../../likelihood-function.md) that involve $X_2$ are the transitions from $X_1$ to $X_2$ and from $X_2$ to $X_3$. Hence conditioning on later observations adds no information once the two neighbors are known. Writing $u=X_2-\mu$, $u_1=x_1-\mu$ and $u_3=x_3-\mu$, its conditional density is proportional to

$$
\exp\left[-\frac{(u-\phi u_1)^2+(u_3-\phi u)^2}{2\sigma^2}\right].
$$

The quadratic coefficient of $u$ is $1+\phi^2$ and the linear coefficient is $-2\phi(u_1+u_3)$. [Completing the square](../../../../../../completing-the-square.md) therefore gives the [Gaussian AR1 bridge](../../../../../../gaussian-ar1-bridge.md)

$$
\boxed{X_2\mid X_1=x_1,X_3=x_3,\ldots,X_n=x_n\sim N\left(\mu+\frac{\phi(x_1+x_3-2\mu)}{1+\phi^2},\frac{\sigma^2}{1+\phi^2}\right).}
$$

Here $\sigma^2$ is the innovation variance, not the marginal stationary variance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
