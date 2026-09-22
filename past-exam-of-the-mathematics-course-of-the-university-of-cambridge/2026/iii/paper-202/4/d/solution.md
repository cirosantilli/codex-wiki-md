<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For this square-root payoff, the time-zero [Black-Scholes model](../../../../../../black-scholes-model.md) price at volatility $\widehat\sigma$ is

$$
C_0=\sqrt{S_0}\exp\!\left(-\frac18T\widehat\sigma^2\right).
$$

Parts (a)(i) and (a)(ii), together with $a\leq[M]_T\leq b$, give

$$
\sqrt{S_0}e^{-b/8}
\leq C_0
\leq\sqrt{S_0}e^{-a/8}.
$$

The exponential is strictly decreasing, so comparison with the defining Black-Scholes price gives

$$
a\leq T\widehat\sigma^2\leq b.
$$

**Thus the [Black-Scholes implied volatility](../../../../../../black-scholes-implied-volatility.md) lies between the lower and upper realized-variance bounds.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
