<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [exponential dispersion family of order one](../../../../../exponential-dispersion-family-of-order-one.md) has density or mass function, relative to a fixed dominating measure, of the form

$$
p(y;\theta,\phi)=\exp\!\left\{\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)\right\},
$$

where $\theta$ is a scalar [natural parameter](../../../../../natural-parameter-of-an-exponential-family.md), $\phi>0$ is the [dispersion parameter](../../../../../dispersion-parameter.md), and the support does not depend on $\theta$. For regular families, $b$ is twice differentiable on an open natural-parameter domain and $b''>0$. Known observation weights $w$ replace $\phi$ by $\phi/w$. “Order one” refers to the scalar canonical [statistic](../../../../../statistic.md) $y$, rather than an arbitrary vector of canonical [statistics](../../../../../statistic.md).

Differentiate the normalization $\int p(y;\theta,\phi)\,dy=1$, or its discrete counterpart, assuming differentiation under the integral is valid. The first [derivative](../../../../../derivative.md) gives $\mathbb E(Y-b'(\theta))=0$. The second [derivative](../../../../../derivative.md) gives

$$
0=\mathbb E\!\left[\frac{(Y-b'(\theta))^2}{\phi^2}-\frac{b''(\theta)}\phi\right].
$$

Consequently,

$$
\boxed{\mu=\mathbb E Y=b'(\theta),\qquad \operatorname{Var}(Y)=\phi b''(\theta).}
$$

The [variance function](../../../../../variance-function.md) expresses the second [derivative](../../../../../derivative.md) in terms of the mean:

$$
\boxed{V(\mu)=b''((b')^{-1}(\mu)),\qquad \operatorname{Var}(Y)=\phi V(\mu)/w.}
$$

A [generalized linear model](../../../../../generalized-linear-model.md) specifies independent responses from an [exponential dispersion family](../../../../../exponential-dispersion-model.md), a [linear predictor](../../../../../linear-predictor.md) $\eta_i=x_i^T\beta$, and a differentiable monotone [link function](../../../../../link-function.md) relating it to the response mean by $g(\mu_i)=\eta_i$. The family, [variance function](../../../../../variance-function.md), covariate design, [link function](../../../../../link-function.md) and dispersion specification together define the model. The [canonical link function](../../../../../canonical-link-function.md) identifies the [linear predictor](../../../../../linear-predictor.md) with the [natural parameter](../../../../../natural-parameter-of-an-exponential-family.md):

$$
\boxed{g(\mu)=(b')^{-1}(\mu),\qquad\theta_i=x_i^T\beta.}
$$

One advantage is that the [likelihood](../../../../../likelihood-function.md) equations become particularly simple. With known weights $w_i$ and common dispersion $\phi$, the [score function](../../../../../informant-function.md) and negative [Hessian matrix](../../../../../hessian-matrix.md) for $\beta$ are

$$
U_\beta=\frac1\phi\sum_i w_ix_i(Y_i-\mu_i),\qquad
-\ell_{\beta\beta}=\frac1\phi\sum_iw_iV(\mu_i)x_ix_i^T.
$$

The latter does not explicitly depend on the responses, so it equals the expected [Fisher information matrix](../../../../../fisher-information-matrix.md) at the same parameter. With full-rank design and positive [variances](../../../../../variance-split.md) the [likelihood](../../../../../likelihood-function.md) is strictly concave in $\beta$, simplifying optimization. These statements concern the coefficient block at a fixed dispersion value.

Three explicit examples, taking unit weights, are as follows.

For a [normal distribution](../../../../../normal-distribution.md) with mean $\mu$ and [variance](../../../../../variance-split.md) $\phi$,

$$
\log p(y)=\frac{y\mu-\mu^2/2}{\phi}-\frac{y^2}{2\phi}-\frac12\log(2\pi\phi).
$$

Thus $\theta=\mu$, $b(\theta)=\theta^2/2$, $c(y,\phi)=-y^2/(2\phi)-\tfrac12\log(2\pi\phi)$, and $V(\mu)=1$. Its [canonical link function](../../../../../canonical-link-function.md) is $\boxed{g(\mu)=\mu}$, the [identity link](../../../../../identity-link.md).

For a [Poisson distribution](../../../../../poisson-distribution.md) with mean $\mu>0$ and support $\{0,1,\ldots\}$,

$$
\log p(y)=y\log\mu-\mu-\log(y!).
$$

Here $\phi=1$, $\theta=\log\mu$, $b(\theta)=e^\theta$, and $c(y,1)=-\log(y!)$. Therefore $b'(\theta)=b''(\theta)=e^\theta$, $V(\mu)=\mu$, and the [Poisson canonical link](../../../../../poisson-canonical-link.md) is $\boxed{g(\mu)=\log\mu}$.

For a [Bernoulli distribution](../../../../../bernoulli-distribution.md) with success probability $\mu\in(0,1)$,

$$
\log p(y)=y\log\frac\mu{1-\mu}+\log(1-\mu),\qquad y\in\{0,1\}.
$$

Taking $\phi=1$, $\theta=\log(\mu/(1-\mu))$, $b(\theta)=\log(1+e^\theta)$, and $c(y,1)=0$ gives the required form. Its mean and [variance function](../../../../../variance-function.md) are $b'(\theta)=e^\theta/(1+e^\theta)=\mu$ and $V(\mu)=\mu(1-\mu)$. Its [canonical link function](../../../../../canonical-link-function.md) is $\boxed{g(\mu)=\log(\mu/(1-\mu))}$, the [logit link](../../../../../logit.md). The fixed dispersion values in the Poisson and Bernoulli cases are part of those models; an arbitrary continuous dispersion is not being asserted for them.

To test $H_0:\beta_j=0$, first fit the unrestricted model and then the restricted model with that component fixed at zero, estimating all [nuisance parameters](../../../../../nuisance-parameter.md), including dispersion when applicable, in each fit. If $\widehat\vartheta$ and $\widetilde\vartheta$ denote their full fitted parameter vectors, the [likelihood-ratio test](../../../../../likelihood-ratio-test.md) uses

$$
\boxed{D=2\{\ell(\widehat\vartheta)-\ell(\widetilde\vartheta)\}.}
$$

For identifiable regular models, an interior null parameter and a fixed-dimensional full-rank design with increasing information, the [Wilks theorem](../../../../../wilks-theorem.md) gives $D\xrightarrow{d}\chi_1^2$ under $H_0$. A level-$\alpha$ test rejects for $D$ greater than the $(1-\alpha)$-[quantile](../../../../../quantile-function.md) of the [chi-squared distribution](../../../../../chi-squared-distribution.md) with one [degree of freedom](../../../../../degree-of-freedom.md).

Alternatively the [Wald test](../../../../../wald-test.md) uses $W=\widehat\beta_j^2/\widehat{\operatorname{Var}}(\widehat\beta_j)$, with the [variance](../../../../../variance-split.md) obtained from the appropriate inverse full [Fisher information matrix](../../../../../fisher-information-matrix.md); it has the same limiting $\chi_1^2$ null law. The [score test](../../../../../score-test.md) fits only the restricted model. If $\lambda$ collects its [nuisance parameters](../../../../../nuisance-parameter.md), its efficient information is $I_{jj\cdot\lambda}=I_{jj}-I_{j\lambda}I_{\lambda\lambda}^{-1}I_{\lambda j}$, and the [statistic](../../../../../statistic.md) is $U_j(\widetilde\vartheta)^2/I_{jj\cdot\lambda}(\widetilde\vartheta)$, again asymptotically $\chi_1^2$. Accounting for the nuisance block is necessary rather than using the unadjusted diagonal information.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
