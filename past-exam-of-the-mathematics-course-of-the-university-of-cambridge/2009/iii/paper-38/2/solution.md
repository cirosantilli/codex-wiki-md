<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work at a regular admissible parameter value with $\phi\ne0$, so the score identities in the question apply. For one observation from the [exponential dispersion family](../../../../../exponential-dispersion-model.md), the [score function](../../../../../informant-function.md) and second derivative are

$$
\partial_\theta l_1=\frac{Y-b'(\theta)}{\phi},\qquad
\partial_\theta^2l_1=-\frac{b''(\theta)}{\phi}.
$$

The zero expected score immediately gives $\mathbb EY=b'(\theta)$. The equality between expected negative curvature and score variance then gives

$$
\frac{b''(\theta)}{\phi}
=\mathbb E\left[\frac{Y-b'(\theta)}{\phi}\right]^2
=\frac{\operatorname{var}Y}{\phi^2}.
$$

Thus

$$
\boxed{\mathbb EY=b'(\theta),\qquad \operatorname{var}Y=\phi b''(\theta).}
$$

The admissible density parameters necessarily make this [variance](../../../../../variance-split.md) nonnegative; the algebra does not require an unstated sign assumption beyond the regular family and $\phi\ne0$.

With independent observations and canonical parameters $\theta_i=x_i^T\beta$, the chain rule gives the vector [score function](../../../../../informant-function.md)

$$
\nabla_\beta l_n=\frac1\phi\sum_ix_i(Y_i-\mu_i)=\frac1\phi X^T(Y-\mu).
$$

A finite interior [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) satisfies its [score equation](../../../../../score-equation.md), proving

$$
\boxed{X^T(Y-\widehat\mu)=0.}
$$

Differentiating again, using $\nabla_\beta\mu_i=b''(x_i^T\beta)x_i$, gives

$$
-\nabla_\beta^2l_n=\sum_i\frac{b''(x_i^T\beta)}{\phi}x_ix_i^T=X^TVX,
\qquad
\boxed{V_{ii}=\frac{b''(\theta_i)}{\phi}=\frac{\operatorname{var}Y_i}{\phi^2},\quad V_{ij}=0\ (i\ne j).}
$$

This Hessian is independent of the observations, so taking expectation gives exactly the requested [Fisher information matrix](../../../../../fisher-information-matrix.md). In particular, $V$ is not the inverse observation-variance matrix: the linear predictor here is the canonical parameter, not the mean.

For the two-group [Poisson regression](../../../../../poisson-regression.md), $\phi=1$, $b(\theta)=e^\theta$, and $\mu_i=e^{x_i^T\beta}$. Put $a=e^\alpha$, $b=e^{\alpha+\nu}$, using $b$ here for the second group's mean. There are $2n$ observations, and

$$
\boxed{X=\begin{pmatrix}\mathbf1_n&\mathbf0_n\\\mathbf1_n&\mathbf1_n\end{pmatrix},\qquad
V=\operatorname{diag}(aI_n,bI_n).}
$$

Hence the total [Fisher information matrix](../../../../../fisher-information-matrix.md) and its inverse are

$$
I_{2n}(\beta)=n\begin{pmatrix}a+b&b\\b&b\end{pmatrix},\qquad
I_{2n}(\beta)^{-1}=\frac1n\begin{pmatrix}a^{-1}&-a^{-1}\\-a^{-1}&a^{-1}+b^{-1}\end{pmatrix}.
$$

The theorem on [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) says that in a regular identifiable model with nonsingular information the estimator is approximately multivariate normal, centred at the true parameter and with covariance equal to the inverse total information. Here one can regard one observation from each group as an independent pair and apply its usual iid version to $n$ such pairs. Therefore

$$
\boxed{\widehat\nu\ \dot\sim\ N\left(\nu,\frac{e^{-\alpha}+e^{-\alpha-\nu}}{n}\right).}
$$

For a direct check, the second score equation gives the fitted second-group mean $\overline Y_B$, and the first then gives the fitted first-group mean $\overline Y_A$. Thus the [Poisson log-rate ratio](../../../../../poisson-log-rate-ratio.md) estimate is $\widehat\nu=\log\overline Y_B-\log\overline Y_A$. The [delta method](../../../../../delta-method.md), using independent sample-mean variances $a/n$ and $b/n$, gives the same variance $(a^{-1}+b^{-1})/n$. If a group total is zero, its finite log-mean estimator fails to exist; with fixed positive true means this event has probability tending to zero exponentially as $n$ grows.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
