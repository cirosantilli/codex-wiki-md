<h1 id="1/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $\theta>0$, the [Exponential martingale for Brownian motion](../../../../../../../exponential-martingale-for-brownian-motion.md) and the [Doob maximal inequality for a nonnegative submartingale](../../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) give

$$
\mathbb P\left(\sup_{t\leq s}B_t\geq a\right)
\leq\exp\left(-\theta a+\frac12\theta^2s\right).
$$

Taking $\theta=a/s$ gives $e^{-a^2/(2s)}$. Apply the same argument to $-B$ and use the [union bound](../../../../../../../boole-s-inequality.md):

$$
\boxed{\mathbb P\left(\sup_{t\leq s}|B_t|\geq a\right)
\leq2e^{-a^2/(2s)}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
