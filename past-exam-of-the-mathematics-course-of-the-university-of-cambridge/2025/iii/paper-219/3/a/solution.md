<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\rho=e^{-\Delta t/\tau}=e^{-x}$ and retain $R=k(0,0)$, which equals one for the stated [exponential covariance function](../../../../../../exponential-covariance-function.md). The covariance matrix of $(y_1,y_2,y_3)$ is

$$
R\begin{pmatrix}1&\rho&\rho^2\\\rho&1&\rho\\\rho^2&\rho&1\end{pmatrix}.
$$

Conditioning a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) and simplifying gives

$$
y_3\mid y_1,y_2
\sim N\!\left(\mu+\rho(y_2-mu),R(1-\rho^2)\right).
$$

The absence of $y_1$ from both conditional moments shows that $y_3$ and $y_1$ are conditionally independent given $y_2$. Equivalently, the exponential-kernel [Gaussian process](../../../../../../gaussian-process.md) is the stationary [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md), which is Markov.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
