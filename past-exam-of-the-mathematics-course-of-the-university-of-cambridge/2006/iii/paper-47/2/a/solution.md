<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Only overlapping innovations contribute to the [autocovariance function](../../../../../../autocovariance.md) of the [moving-average process](../../../../../../moving-average-model.md). Set $c_0=1,c_1=\theta_1,c_2=\theta_2$. The overlap formula is $\gamma_k=\sigma^2\sum_jc_jc_{j+|k|}$, with coefficients outside $0,1,2$ set to zero. Thus

$$
\boxed{\gamma_k=\begin{cases}
\sigma^2(1+\theta_1^2+\theta_2^2),&k=0,\\
\sigma^2\theta_1(1+\theta_2),&|k|=1,\\
\sigma^2\theta_2,&|k|=2,\\
0,&|k|>2.
\end{cases}}
$$

The [time-series spectral density](../../../../../../spectral-density-of-a-stationary-process.md) is the Fourier sum of this finite [covariance](../../../../../../covariance.md) sequence:

$$
\boxed{f(\lambda)=\frac{\sigma^2}{2\pi}\left[1+\theta_1^2+\theta_2^2+
2\theta_1(1+\theta_2)\cos\lambda+2\theta_2\cos2\lambda\right].}
$$

It also equals $\sigma^2|1+\theta_1e^{-i\lambda}+\theta_2e^{-2i\lambda}|^2/(2\pi)$, which directly verifies nonnegativity. Integrating from $-\pi$ gives the requested [time-series spectral distribution](../../../../../../spectral-distribution-function-of-a-stationary-time-series.md):

$$
\boxed{F(\lambda)=\frac{\sigma^2}{2\pi}\left[(1+\theta_1^2+\theta_2^2)(\lambda+\pi)
+2\theta_1(1+\theta_2)\sin\lambda+\theta_2\sin2\lambda\right],\quad -\pi\le\lambda\le\pi.}
$$

Extend it by zero below $-\pi$ and by $\gamma_0$ above $\pi$. In particular its total mass is the process [variance](../../../../../../variance-split.md), not necessarily one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
