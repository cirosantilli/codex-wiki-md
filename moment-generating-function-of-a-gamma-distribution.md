# Moment-generating function of a gamma distribution

↑ **Parent:** [Gamma distribution](gamma-distribution.md)

For the rate-parameterized [Gamma distribution](gamma-distribution.md) with shape $r>0$ and rate $\lambda>0$, integration of its [probability density](probability-density.md) gives

$$
\mathbb E[e^{tX}]=\frac{\lambda^r}{\Gamma(r)}\int_0^\infty x^{r-1}e^{-(\lambda-t)x}\,dx=\left(\frac{\lambda}{\lambda-t}\right)^r
$$

when $t<\lambda$, by the [gamma function](gamma-function.md) integral and a [change of variables](change-of-variables-formula.md). The integral is infinite for $t\geq\lambda$. In particular the [moment-generating function](moment-generating-function.md) is finite on an open interval containing zero, so the [uniqueness theorem for moment-generating functions](uniqueness-theorem-for-moment-generating-functions.md) applies. Multiplication of these [moment-generating functions](moment-generating-function.md) proves [additivity of independent gamma distributions with a common rate](additivity-of-independent-gamma-distributions-with-a-common-rate.md).

## ↑ Ancestors (8)

1. [Gamma distribution](gamma-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2014/2/a/solution.md)
