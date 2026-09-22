# Laplace location and scale maximum likelihood

↑ **Parent:** [Laplace distribution](laplace-distribution.md)

Suppose $X_1,\ldots,X_n$, $n\geq1$, are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) with [Laplace distribution](laplace-distribution.md) $\operatorname{Laplace}(\mu,b)$, where $b>0$. For realized values $x_1,\ldots,x_n$, the [likelihood function](likelihood-function.md) and [log-likelihood function](log-likelihood.md) are

$$
L(\mu,b)=(2b)^{-n}e^{-S(\mu)/b},\qquad \ell(\mu,b)=-n\log(2b)-\frac{S(\mu)}b,\qquad S(a)=\sum_{i=1}^n|x_i-a|.
$$

For fixed $b$, [maximum likelihood estimation](maximum-likelihood-estimation-split.md) of the location therefore minimizes the sum of [absolute losses](absolute-error-loss.md). This connects the [Laplace distribution](laplace-distribution.md) to [robust statistics](robust-statistics-split.md): each observation contributes a cost growing linearly with its distance, whereas [squared-error loss](squared-error-loss.md) grows quadratically.

Why does a [sample median](sample-median.md) minimize $S$? Between successive [order statistics](order-statistic.md), moving $a$ a little to the right increases each distance to a value on the left and decreases each distance to a value on the right. Hence the slope is the number on the left minus the number on the right. It changes from negative to positive at the middle. More precisely, if $x_{(1)}\leq\cdots\leq x_{(n)}$, all minimizing locations are

$$
\arg\min_a S(a)=\begin{cases}
\{x_{(m+1)}\},&n=2m+1,\\
[x_{(m)},x_{(m+1)}],&n=2m.
\end{cases}
$$

For an even [sample size](sample-size.md), the objective is flat throughout the interval between the two central [order statistics](order-statistic.md). The midpoint convention for the [sample median](sample-median.md) selects one solution; it does not prove uniqueness. [SciPy 1.18.0 documentation; SciPy reference guide, Laplace distribution, ML location estimator and the even-N interval between the two central order statistics](scipy-1-18-0-documentation/laplace-double-exponential-bilateral-exponential-distribution.md) This is the finite-sample counterpart of [median minimizes expected absolute loss](median-minimizes-expected-absolute-loss.md).

If $S(\widehat\mu)>0$, maximizing over $b>0$ gives

$$
\frac{\partial\ell}{\partial b}=-\frac nb+\frac{S(\widehat\mu)}{b^2}=0,\qquad \widehat b=\frac{S(\widehat\mu)}n.
$$

The [derivative](derivative.md) is positive below this value and negative above it. Moreover the maximized [likelihood function](likelihood-function.md) is proportional to $S(\mu)^{-n}$ wherever $S(\mu)>0$, so the same minimizing locations give the joint [maximum-likelihood estimates](maximum-likelihood-estimator.md). [NIST and SEMATECH e-Handbook of Statistical Methods; NIST/SEMATECH e-Handbook, Section 1.3.6.6.12, Parameter Estimation; median and average absolute deviation formulas](nist-and-sematech-e-handbook-of-statistical-methods/1-3-6-6-12-double-exponential-distribution.md) The scale estimate divides by $n$; this formula is not an assertion that it is an [unbiased estimator](unbiased-estimator.md).

The boundary case matters: if all observations equal $c$, choose $\mu=c$. Then $S(c)=0$ and $L(c,b)=(2b)^{-n}\to\infty$ as $b\downarrow0$. There is no finite joint [maximum-likelihood estimate](maximum-likelihood-estimator.md) in the parameter space $b>0$. In particular, this always occurs for $n=1$. Writing $\widehat b=0$ does not produce an admissible [Laplace distribution](laplace-distribution.md).

**Table of contents**

- [Laplace median robustness example](laplace-median-robustness-example.md)

## ↑ Ancestors (8)

1. [Laplace distribution](laplace-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Laplace regression](laplace-regression.md)
