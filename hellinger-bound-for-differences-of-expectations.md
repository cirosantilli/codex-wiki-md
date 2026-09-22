# Hellinger bound for differences of expectations

↑ **Parent:** [Hellinger distance](hellinger-distance.md)

If $f$ is a measurable function into a separable [Banach space](banach-space-split.md) and has finite second [moments](moment.md) under [probability measures](probability-measure.md) $\mu,\mu'$, then their [Bochner integral](bochner-integral.md) [expected values](expected-value.md) satisfy

$$
\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|
\leq2\left(\mathbb E^\mu\|f\|^2+\mathbb E^{\mu'}\|f\|^2\right)^{1/2}d_{\mathrm{Hell}}(\mu,\mu').
$$

Here the [Hellinger distance](hellinger-distance.md) includes the factor $1/2$ in its square. For a proof, use $\nu=(\mu+\mu')/2$, $p=d\mu/d\nu$, and $q=d\mu'/d\nu$. Apply the norm bound for a [Bochner integral](bochner-integral.md) and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) to $f(p-q)=f(\sqrt p-\sqrt q)(\sqrt p+\sqrt q)$, then use $(\sqrt p+\sqrt q)^2\leq2(p+q)$. This explains why stability of a [Bayesian posterior](bayesian-posterior.md) in [Hellinger distance](hellinger-distance.md) controls posterior [expected values](expected-value.md) when the relevant second [moments](moment.md) remain bounded.

## ↑ Ancestors (7)

1. [Hellinger distance](hellinger-distance.md)
2. [Squared Hellinger distance](squared-hellinger-distance.md)
3. [f-divergence](f-divergence.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/3/c/solution.md)
