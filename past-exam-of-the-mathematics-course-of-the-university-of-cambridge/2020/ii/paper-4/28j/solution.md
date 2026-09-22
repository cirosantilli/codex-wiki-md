<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

Write $\ell(x,\theta)=\log f(x,\theta)$ and let $\dot\ell_{\theta_0}(x)$ be its [score function](../../../../../informant-function.md). A second-order [Taylor expansion](../../../../../taylor-expansion.md) around $\theta_0$ gives, for fixed $h$,

$$
Z_n(h)=h^T\Delta_n+\frac1{2n}\sum_{i=1}^nh^T\ddot\ell(X_i,\theta_{i,n})h,
\qquad
\Delta_n=\frac1{\sqrt n}\sum_{i=1}^n\dot\ell_{\theta_0}(X_i),
$$

where every $\theta_{i,n}$ lies between $\theta_0$ and $\theta_0+h/\sqrt n$. The [mean-zero score identity](../../../../../mean-zero-score-identity.md), the [Fisher information matrix](../../../../../fisher-information-matrix.md), and the [multivariate central limit theorem](../../../../../multivariate-central-limit-theorem.md) give

$$
\Delta_n\xrightarrow{d}N(0,I(\theta_0)).
$$

The assumed regularity and a [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) give

$$
\frac1n\sum_{i=1}^n\ddot\ell(X_i,\theta_{i,n})\xrightarrow{p}-I(\theta_0).
$$

Consequently, by the [Slutsky theorem](../../../../../slutsky-theorem.md),

$$
Z_n(h)\xrightarrow{d}h^T\Delta-\frac12h^TI(\theta_0)h,
\qquad
\Delta\sim N(0,I(\theta_0)).
$$

For the stated [Gaussian shift model](../../../../../gaussian-shift-model.md), direct expansion of the two [normal distribution](../../../../../normal-distribution.md) densities gives

$$
Z(h)=h^TI(\theta_0)X-\frac12h^TI(\theta_0)h,
\qquad
X\sim N(0,I(\theta_0)^{-1}).
$$

Since $I(\theta_0)X\sim N(0,I(\theta_0))$, this has exactly the limiting distribution above. Equivalently, both limits are normal with mean $-\tfrac12h^TI(\theta_0)h$ and variance $h^TI(\theta_0)h$. This is the [local asymptotic normality](../../../../../local-asymptotic-normality.md) of the model at $\theta_0$.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
