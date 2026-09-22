<h1 id="4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The solution is the [geometric Brownian motion](../../../../../../geometric-brownian-motion.md)

$$
X_t=x\exp\left((\beta-\tfrac12\sigma^2)t+\sigma B_t\right)>0.
$$

Its [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) is

$$
Lf(x)=\beta xf'(x)+\frac12\sigma^2x^2f''(x).
$$

For $\gamma=1-2\beta/\sigma^2\ne0$, one has $L(x^\gamma)=0$. Optional stopping of $X_{t\wedge T_r\wedge T_R}^\gamma$ and the boundary values therefore give

$$
\boxed{\mathbb P_x(T_r<T_R)=
\frac{R^\gamma-x^\gamma}{R^\gamma-r^\gamma},
\qquad \gamma=1-\frac{2\beta}{\sigma^2}.}
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
