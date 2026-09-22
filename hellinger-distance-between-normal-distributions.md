# Hellinger distance between normal distributions

↑ **Parent:** [Hellinger distance](hellinger-distance.md)

With the convention $d_{\mathrm{Hell}}^2=\frac12\int(\sqrt p-\sqrt q)^2$, the [Hellinger distance](hellinger-distance.md) between two [normal distributions](normal-distribution.md) with $\sigma_1,\sigma_2>0$ is

$$
d_{\mathrm{Hell}}^2=1-\sqrt{\frac{2\sigma_1\sigma_2}{\sigma_1^2+\sigma_2^2}}
\exp\left[-\frac{(\theta_1-\theta_2)^2}{4(\sigma_1^2+\sigma_2^2)}\right].
$$

To prove it, integrate the geometric mean of their [probability density functions](probability-density-function.md). [Completing the square](completing-the-square.md) makes that geometric mean the density of a [normal distribution](normal-distribution.md) times the displayed prefactor and exponential. For example, writing $S=\sigma_1^2+\sigma_2^2$, that [normal distribution](normal-distribution.md) has mean $(\theta_1\sigma_2^2+\theta_2\sigma_1^2)/S$ and [variance](variance-split.md) $2\sigma_1^2\sigma_2^2/S$. The identity $d_{\mathrm{Hell}}^2=1-\int\sqrt{pq}$ then proves the formula.

For equal unit [variances](variance-split.md), this becomes $1-e^{-(\theta_1-\theta_2)^2/8}$. More generally, put $B=\sqrt{2\sigma_1\sigma_2/S}\leq1$ and $x=(\theta_1-\theta_2)^2/(4S)$. Then $1-Be^{-x}=(1-B)+B(1-e^{-x})$, $1-B=(\sigma_1-\sigma_2)^2/[S(1+B)]$, and $1-e^{-x}\leq x$, proving

$$
d_{\mathrm{Hell}}^2\leq\frac{(\sigma_1-\sigma_2)^2+(\theta_1-\theta_2)^2}{\sigma_1^2+\sigma_2^2}.
$$

## ↑ Ancestors (7)

1. [Hellinger distance](hellinger-distance.md)
2. [Squared Hellinger distance](squared-hellinger-distance.md)
3. [f-divergence](f-divergence.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/1/c/solution.md)
