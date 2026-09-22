# Log-linear exponential-decay fit

↑ **Parent:** [Linear regression](linear-regression-split.md)

An [exponential decay](exponential-decay.md) rate $R=R_0e^{-t/\tau}$ becomes a straight line in $x=t$ and $y=\ln(R/R_*)$, where $R_*$ is a fixed reference rate. Constant small fractional rate errors become approximately constant vertical errors $s\simeq\sigma_R/R$ by [propagation of uncertainty](propagation-of-uncertainty.md). With independent Gaussian log-rate errors, [linear least squares](linear-least-squares.md) gives $\widehat m=S_{xy}/S_{xx}$ and $\widehat c=\bar y-\widehat m\bar x$.

The [covariance matrix](covariance-matrix.md) is obtained by applying the variance rules to these linear estimators:

$$
\operatorname{Var}\widehat m=\frac{s^2}{S_{xx}},\quad
\operatorname{Var}\widehat c=s^2\left(\frac1n+\frac{\bar x^2}{S_{xx}}\right),\quad
\operatorname{Cov}(\widehat m,\widehat c)=-\frac{s^2\bar x}{S_{xx}}.
$$

Transforming back gives $\widehat\tau=-1/\widehat m$, $\sigma_\tau\simeq\sigma_m/\widehat m^2$, $\widehat R_0=R_*e^{\widehat c}$ and $\sigma_{R_0}\simeq\widehat R_0\sigma_c$. If a candidate lifetime fixes the slope $m_a$, the intercept must be refitted as $c_a=\bar y-m_a\bar x$. The profiled objective obeys

$$
\chi^2(m_a,c_a)=\chi^2_{\min}+\frac{S_{xx}}{s^2}(m_a-\widehat m)^2.
$$

This follows by separating the centred slope residual from the unrestricted [regression residual](regression-residual.md), whose inner product with the design columns is zero by the [normal equations for linear least squares](normal-equations-for-linear-least-squares.md). Known supplied measurement errors are not rescaled by the observed reduced chi-squared. This log-error model is an approximation for proportional errors, not an exact replacement for every raw-count likelihood.

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-c/c8/c/solution.md)
