# Pearson correlation coefficient

↑ **Parent:** [Covariance matrix](covariance-matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)

The [Pearson correlation coefficient](pearson-correlation-coefficient.md) is the [covariance](covariance.md) divided by the product of the [standard deviations](standard-deviation.md). For real [random variables](random-variable-split.md) with finite, strictly positive [variances](variance-split.md),

$$
\rho_{X,Y}=\frac{\operatorname{Cov}(X,Y)}{\sqrt{\operatorname{Var}(X)\operatorname{Var}(Y)}}.
$$

It is the [expected value](expected-value-split.md) of the product of the two centered variables after dividing each by its [standard deviation](standard-deviation.md). The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $-1\leq\rho_{X,Y}\leq1$. This removes measurement units, while retaining the direction and strength of the linear relationship. Constant [random variables](random-variable-split.md) have zero [standard deviation](standard-deviation.md), so their [Pearson correlation coefficient](pearson-correlation-coefficient.md) is undefined.

For the [covariance](covariance.md) model $Y=2X+Z$, with $X,Z$ independently uniform on $\{-1,0,1\}$, the calculation gives

$$
\rho_{X,Y}=\frac{4/3}{\sqrt{(2/3)(10/3)}}=\frac2{\sqrt5}\approx0.894427.
$$

The positive [correlation](pearson-correlation-coefficient.md) is less than one because the independent $Z$ term introduces extra variation. For $Y=-2X+Z$ the [correlation](pearson-correlation-coefficient.md) is $-2/\sqrt5$. Both examples appear in the [covariance](covariance.md) diagram.

For nonzero real $a,c$, the [correlation](pearson-correlation-coefficient.md) of $aX+b$ and $cY+d$ is $\operatorname{sgn}(ac)\rho_{X,Y}$. Positive rescaling and added offsets therefore leave the [correlation](pearson-correlation-coefficient.md) unchanged; reversing one scale reverses its sign. Equality $|\rho_{X,Y}|=1$ means that one [random variable](random-variable-split.md) is an [affine function](affine-function.md) of the other [almost surely](almost-sure-convergence.md), with a nonzero slope of the corresponding sign. This is the equality condition in the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md), and includes [perfect positive correlation](perfect-positive-correlation.md).

Zero [correlation](pearson-correlation-coefficient.md) says that the centered variables are [orthogonal](orthogonal-vectors.md) in their square-integrable [inner product](inner-product-split.md). It permits nonlinear [statistical dependence](statistical-dependence.md), as the example $Y=X^2$ in [uncorrelated random variables](uncorrelated-random-variables.md) demonstrates. More generally, a [correlation](pearson-correlation-coefficient.md) is a statement about a [joint probability distribution](joint-probability-distribution.md); identifying effects of interventions is the separate task of [causal inference](causal-inference-split.md). This distinction keeps an observed association from being mistaken for a demonstrated mechanism.

An early source for standardized association is [Francis Galton](francis-galton.md)'s 1888 paper “Co-relations and their Measurement, chiefly from Anthropometric Data”. He compared stature and forearm measurements and changed each measurement to units of its own variability so the two regression directions could be compared. His scale used [probable error](probable-error.md), so it should not be identified word for word with the modern [standard deviation](standard-deviation.md) formula above. [Galton's original paper, Proceedings of the Royal Society 45, 135–145](https://galton.org/essays/1880-1889/galton-1888-co-relations-royal-soc/galton_corr.html).

**Table of contents**

- [Conditional correlation](conditional-correlation.md)
- [Partial correlation](partial-correlation.md)
- [Perfect positive correlation](perfect-positive-correlation.md)
  - [Terminal proportionality identifies bounded stock volatility](terminal-proportionality-identifies-bounded-stock-volatility.md)
  - [Terminal correlation does not identify adapted stock volatility](terminal-correlation-does-not-identify-adapted-stock-volatility.md)
- [Serial correlation](serial-correlation.md)
- [Intraclass correlation coefficient](intraclass-correlation-coefficient.md)

## ↑ Ancestors (9)

1. [Covariance matrix](covariance-matrix.md)
2. [Covariance](covariance.md)
3. [Variance](variance-split.md)
4. [Expected value](expected-value-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Covariance](covariance.md)
- [Galton's stature regression](galton-s-stature-regression.md)
- [Gaussian regression toward the mean](gaussian-regression-toward-the-mean.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1/2/a/solution.md)
- [Pearson correlation coefficient](pearson-correlation-coefficient.md)
- [Repeated-measurement latent signal model](repeated-measurement-latent-signal-model.md)
- [Sample correlation coefficient](sample-correlation-coefficient.md)
