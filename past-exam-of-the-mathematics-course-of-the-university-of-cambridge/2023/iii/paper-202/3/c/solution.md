<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [Reflection invariance of Brownian motion](../../../../../../reflection-invariance-of-brownian-motion.md), $-B$ is Brownian motion, and the first time $B_t-t$ reaches $b<0$ is the first time $-B_t+t$ reaches $-b>0$. Part b therefore gives

$$
\mathbb E e^{S_b/2}=e^{-b}.
$$

Now $L_t=\exp(B_t-t/2)$ is the [exponential Brownian martingale](../../../../../../exponential-brownian-martingale.md). At $S_b$, the identity $B_{S_b}=b+S_b$ gives $L_{S_b}=e^{b+S_b/2}$, so $\mathbb E L_{S_b}=1$. The nonnegative stopped martingale $(L_{t\wedge S_b})$ therefore loses no mass at infinity and is [uniformly integrable](../../../../../../uniform-integrability.md). The [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at any stopping time $R$ gives

$$
\boxed{\mathbb E\exp\!\left(B_{R\wedge S_b}-\frac12(R\wedge S_b)\right)=1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
