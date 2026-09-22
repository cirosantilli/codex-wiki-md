<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Markov chain Monte Carlo asymptotic variance](../../../../../../markov-chain-monte-carlo-asymptotic-variance.md) for a stationary [Markov chain](../../../../../../markov-chain.md) and $\psi\in L^2(\pi)$ is

$$
\sigma_K^2(\psi)
=\lim_{n\to\infty}n\operatorname{Var}\left(
\frac1n\sum_{j=1}^n\psi(X_j)\right)
=\operatorname{Var}_\pi(\psi)
+2\sum_{k=1}^{\infty}
\operatorname{Cov}_\pi(\psi(X_0),\psi(X_k)),
$$

whenever the limit and series exist. If a [reversible Markov chain](../../../../../../reversible-markov-chain.md) has positive $L^2_0(\pi)$ [spectral gap](../../../../../../spectral-gap.md) $\gamma$, then the [spectral theorem for normal operators on a separable Hilbert space](../../../../../../spectral-theorem-for-normal-operators-on-a-separable-hilbert-space.md) gives

$$
\boxed{\sigma_K^2(\psi)
\leq\left(\frac2\gamma-1\right)
\operatorname{Var}_\pi(\psi).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
