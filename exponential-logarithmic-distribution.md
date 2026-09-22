# Exponential-logarithmic distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)

For $0<p<1$, $\beta>0$ and $x>0$, this [probability density function](probability-density-function.md) has [cumulative distribution function](cumulative-distribution-function.md) $F(x)=1-\log(1-(1-p)e^{-\beta x})/\log p$. Differentiating gives the density, while the endpoint limits are zero and one. Its [quantile function](quantile-function.md) is $F^{-1}(u)=\beta^{-1}[\log(1-p)-\log(1-p^{1-u})]$ for $0<u<1$, enabling [inverse transform sampling](inverse-transform-sampling.md).

Expanding the denominator as a [geometric series](geometric-series.md) gives

$$
f_{p,\beta}(x)=-\frac{\beta}{\log p}\sum_{k\geq1}(1-p)^ke^{-k\beta x}.
$$

Termwise integration, justified by the [monotone convergence theorem](monotone-convergence-theorem.md), and the [gamma function](gamma-function.md) integral yield [raw moments](raw-moment.md) $\mathbb E[X^j]=-j!\operatorname{Li}_{j+1}(1-p)/(\beta^j\log p)$. Thus the [polylogarithm](polylogarithm.md) expresses its [mean](expected-value-split.md), [variance](variance-split.md) and higher [moments](moment.md). Here $p$ is the complement of the series parameter $1-p$; parameter conventions must be checked when comparing formulas.

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/3/a/i/solution.md)
