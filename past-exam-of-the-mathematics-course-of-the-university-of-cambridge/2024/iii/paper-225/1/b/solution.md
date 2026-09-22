<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $x\otimes y$ for the [rank-one operator](../../../../../../rank-one-operator.md) $h\mapsto\langle h,y\rangle x$. The estimator is the kernel representation of the [empirical covariance operator](../../../../../../empirical-covariance-operator.md)

$$
\widehat C_{\mu_0}=\frac1n\sum_{i=1}^n(X_i-\mu_0)\otimes(X_i-\mu_0).
$$

Since $\mathbb EX=0$,

$$
\mathbb E\widehat C_{\mu_0}=C_X+\mu_0\otimes\mu_0.
$$

Thus the estimator has the fixed [bias of an estimator](../../../../../../bias-of-an-estimator.md) $\mu_0\otimes\mu_0$ for $C_X$.

The fourth-moment assumption makes $(X_i-\mu_0)\otimes(X_i-\mu_0)$ square-integrable in the Hilbert space of [Hilbert-Schmidt operators](../../../../../../hilbert-schmidt-operator.md). The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) therefore gives

$$
\widehat C_{\mu_0}\xrightarrow{p}C_X+\mu_0\otimes\mu_0.
$$

Consequently [consistency](../../../../../../consistency-statistics.md) for $C_X$ holds exactly when $\mu_0=0$. More precisely, if $Y=(X-\mu_0)\otimes(X-\mu_0)$, then

$$
\mathbb E\lVert\widehat C_{\mu_0}-C_X\rVert_{\mathrm{HS}}^2
=\lVert\mu_0\otimes\mu_0\rVert_{\mathrm{HS}}^2
+\frac1n\mathbb E\lVert Y-\mathbb EY\rVert_{\mathrm{HS}}^2
=\lVert\mu_0\rVert^4+O(n^{-1}).
$$

The [Hilbert-space central limit theorem](../../../../../../hilbert-space-central-limit-theorem.md) also yields

$$
\sqrt n\{\widehat C_{\mu_0}-(C_X+\mu_0\otimes\mu_0)\}
\xrightarrow dG,
$$

where $G$ is a centered [Gaussian random element](../../../../../../gaussian-random-element.md) in the Hilbert-Schmidt operator space with covariance determined by $Y$. Relative to $C_X$, the same fluctuation is displaced by $\sqrt n(\mu_0\otimes\mu_0)$ and hence does not have a finite centered limit when $\mu_0\ne0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
