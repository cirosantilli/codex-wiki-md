<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [predictable](../../../../../../predictable-process.md) position $\pi$, the current net wealth increment $\pi\Delta S_t+Y_t-y$ is conditionally [Gaussian](../../../../../../normal-distribution.md) with mean $\pi\mu+a-y$ and [variance](../../../../../../variance-split.md) $\pi^2\sigma^2+2\pi\rho b\sigma+b^2$. Its exponential-loss multiplier is

$$
\exp\left[-\gamma(\pi\mu+a-y)+\tfrac12\gamma^2(\pi^2\sigma^2+2\pi\rho b\sigma+b^2)\right].
$$

Differentiate its quadratic exponent. The unique minimizing position is

$$
\boxed{\pi_t^{\mathrm{swap}}=\frac\mu{\gamma\sigma^2}-\frac{\rho b}{\sigma},\quad1\leq t\leq T.}
$$

The first term is the speculative demand; the second offsets the part of the income correlated with the tradable price increment. Independent period vectors and [backward induction](../../../../../../backward-induction.md) justify using this same position at every date. Completing the square gives minimal exponent $-\kappa-\gamma d(y)$, where

$$
d(y)=a-y-\frac{\mu\rho b}{\sigma}-\frac\gamma2b^2(1-\rho^2).
$$

Therefore [hedging a Gaussian income stream with exponential utility](../../../../../../hedging-a-gaussian-income-stream-with-exponential-utility.md) has value

$$
\boxed{V_0^{\mathrm{swap}}(x;y)=-\exp[-\gamma x-T\kappa-\gamma T d(y)].}
$$

The residual [variance](../../../../../../variance-split.md) is $b^2(1-\rho^2)$; it disappears for perfectly correlated income.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
