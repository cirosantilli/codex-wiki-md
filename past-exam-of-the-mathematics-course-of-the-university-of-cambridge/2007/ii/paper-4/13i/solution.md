<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

Use the [exponential dispersion family](../../../../../exponential-dispersion-model.md) convention $f(y)=\exp\{[y\theta-b(\theta)]/\phi+c(y,\phi)\}$. For the [Gamma distribution](../../../../../gamma-distribution.md), take

$$
\phi=\alpha^{-1},\qquad \theta=-\lambda/\alpha<0,
\qquad b(\theta)=-\log(-\theta),
$$



$$
c(y,\phi)=(\alpha-1)\log y+\alpha\log\alpha-\log\Gamma(\alpha).
$$

Substitution reproduces the gamma density exactly. Differentiating its normalization with respect to $\theta$ yields $\mathbb EY=b'(\theta)$ and $\operatorname{Var}Y=\phi b''(\theta)$: the first identity follows from zero mean score, and differentiation again gives the variance. Therefore

$$
\boxed{\mathbb EY=\alpha/\lambda,\qquad\operatorname{Var}Y=\alpha/\lambda^2.}
$$

The [canonical link function](../../../../../canonical-link-function.md) is $g(\mu)=\theta=-1/\mu$. Some conventions reverse the sign and call $1/\mu$ the reciprocal link; this only reverses the regression coefficients. We retain the genuine natural parameter $\theta=-1/\mu$.

In the [Gamma regression with canonical link](../../../../../gamma-regression-with-canonical-link.md), $\eta_i=x_i^T\beta<0$ and $\mu_i=-1/\eta_i$. Differentiating the independent-observation log-likelihood gives

$$
\boxed{U(\beta)=\phi^{-1}X^T(y-\mu),\qquad
I(\beta)=\phi^{-1}X^T\operatorname{diag}(\mu_i^2)X.}
$$

Here $d\mu_i/d\eta_i=\mu_i^2$, so the negative Hessian equals this information matrix. [Fisher scoring](../../../../../scoring-algorithm.md) or Newton iteration is

$$
\beta_{\rm new}=\beta+I(\beta)^{-1}U(\beta),
$$

with the means and information recalculated at each iteration; damping can preserve $X\beta<0$ and increase the likelihood. Full column rank makes the information positive definite for positive means.

The saturated model has mean $y_i$. Subtracting fitted from saturated log-likelihood yields the unscaled [deviance](../../../../../exponential-family-deviance.md)

$$
\boxed{D=2\sum_i\left[\frac{y_i-\widehat\mu_i}{\widehat\mu_i}
-\log\frac{y_i}{\widehat\mu_i}\right].}
$$

Twice the actual log-likelihood ratio is $D/\phi$. In particular, the printed parenthetical $\widehat\mu=X\widehat\beta$ is incorrect for this nonidentity link: **$X\widehat\beta$ estimates $\eta$, and $\widehat\mu_i=-1/(x_i^T\widehat\beta)$**.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
