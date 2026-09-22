<h1 id="29j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $V_{YY}$ is invertible. Put

$$
R=X-\mu_X-V_{XY}V_{YY}^{-1}(Y-\mu_Y).
$$

This and $Y$ are jointly [multivariate normal](../../../../../../multivariate-normal-distribution.md), with $\operatorname{Cov}(R,Y)=0$ and $\operatorname{Cov}(R)=V_{XX}-V_{XY}V_{YY}^{-1}V_{YX}$. Their joint Gaussian [characteristic function](../../../../../../characteristic-function.md) factors when the cross covariance vanishes, so they are independent. Conditioning on $Y=y$ therefore leaves the law of $R$ unchanged, proving

$$
\boxed{X\mid Y=y\sim N(\mu_X+V_{XY}V_{YY}^{-1}(y-\mu_Y),\ V_{XX}-V_{XY}V_{YY}^{-1}V_{YX})}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29J](../../29j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
