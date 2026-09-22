# Repeated-measurement latent signal model

↑ **Parent:** [Regression toward the mean](regression-toward-the-mean.md)

Imagine an instrument measuring the same fixed quantity twice on each unit. Across units the persistent signal $T$ is a [latent variable](latent-variable-split.md); the two [measurement errors](measurement-error.md) $\varepsilon_1,\varepsilon_2$ are fresh, mutually [independent random variables](independent-random-variables.md), also independent of $T$. Assume they have [mean](expected-value-split.md) zero and common finite [variance](variance-split.md) $v$, while $T$ has [mean](expected-value-split.md) $\mu$ and [variance](variance-split.md) $s$. Then

$$
X=T+\varepsilon_1,\qquad Y=T+\varepsilon_2,\qquad
\mathbb E[X]=\mathbb E[Y]=\mu,\qquad
\operatorname{Var}(X)=\operatorname{Var}(Y)=s+v,\qquad
\operatorname{Cov}(X,Y)=s.
$$

Thus the [Pearson correlation coefficient](pearson-correlation-coefficient.md) is $\rho=s/(s+v)$ when $s+v>0$. Both measurements retain the same marginal [mean](expected-value-split.md) and [variance](variance-split.md). Repetition does not make the entire population collapse toward $\mu$; it changes what we expect after selecting on $X$.

For $s,v>0$, further assuming [normal distributions](normal-distribution.md) for $T$ and both [measurement errors](measurement-error.md) gives the [conditional expectation](conditional-expectation.md)

$$
\mathbb E[Y\mid X=x]=\mu+\rho(x-\mu).
$$

Since $0<\rho<1$, this predicted reading is closer to $\mu$ than $x$ is. Independence and zero [mean](expected-value-split.md) errors alone do not justify this linear [conditional expectation](conditional-expectation.md): without the [normal distribution](normal-distribution.md) assumption the same expression is the [linear least-squares projection](linear-least-squares-projection.md), and the actual [conditional expectation](conditional-expectation.md) can be nonlinear. Correlated errors, a changing signal, or different error [variances](variance-split.md) require their own model; a noisy reading by itself supplies no universal shrinkage factor.

**Table of contents**

- [Gaussian regression toward the mean](gaussian-regression-toward-the-mean.md)
  - [Selection on an extreme first measurement](selection-on-an-extreme-first-measurement.md)

## ↑ Ancestors (5)

1. [Regression toward the mean](regression-toward-the-mean.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
