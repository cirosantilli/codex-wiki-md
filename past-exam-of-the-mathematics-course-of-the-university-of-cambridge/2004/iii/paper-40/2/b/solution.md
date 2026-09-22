<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditionally on past observations, adding the [independent](../../../../../../independent-random-variables.md) state increment gives the prediction

$$
S_t\mid\mathcal F_{t-1}\sim N(\widehat S_{t-1},R_t),
\qquad R_t=P_{t-1}+W.
$$

The new observation then has [conditional distribution](../../../../../../conditional-distribution.md) $N(\widehat S_{t-1},R_t+V)$, and its conditional [covariance](../../../../../../covariance.md) with $S_t$ is $R_t$. Equivalently, multiplying the state prediction [probability density function](../../../../../../probability-density-function.md) by the observation [likelihood](../../../../../../likelihood-function.md) and completing the square gives

$$
\frac1{P_t}=\frac1{R_t}+\frac1V,
\qquad
\frac{\widehat S_t}{P_t}=\frac{\widehat S_{t-1}}{R_t}+\frac{X_t}V.
$$

For positive [variances](../../../../../../variance-split.md), rearrangement yields the [scalar Gaussian Kalman recursion](../../../../../../scalar-gaussian-kalman-recursion.md)

$$
\boxed{K_t=\frac{P_{t-1}+W}{P_{t-1}+W+V},\quad
\widehat S_t=\widehat S_{t-1}+K_t(X_t-\widehat S_{t-1}),\quad
P_t=\frac{V(P_{t-1}+W)}{P_{t-1}+W+V}.}
$$

Here the innovation is the observation minus its predicted [mean](../../../../../../expected-value.md). The displayed [covariance](../../../../../../covariance.md) formula also handles zero [variances](../../../../../../variance-split.md) whenever its denominator is nonzero; a completely deterministic prediction and observation require no probabilistic update. [Independence](../../../../../../independent-random-variables.md) of the new noises from the past and the initial state is the usual state-space assumption needed for this conditional calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
