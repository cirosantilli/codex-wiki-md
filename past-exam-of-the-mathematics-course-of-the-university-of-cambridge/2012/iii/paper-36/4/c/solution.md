<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Now $p_{\theta,\eta}(x,y)=v(x)f(y-g_\theta(x))$. With $h_\theta=\partial_\theta g_\theta$ and the [location score](../../../../../../location-score.md) $\rho(e)=-f'(e)/f(e)$, differentiation of the [log-likelihood](../../../../../../log-likelihood.md) gives

$$
\boxed{\dot\ell_{\theta,\eta}(x,y)=-h_\theta(x)\frac{f'(e)}{f(e)}=h_\theta(x)\rho(e).}
$$

Take the usual regularity conditions $h_\theta\in L^2(v)$ and $\rho\in L^2(f)$ so that this [score function](../../../../../../informant-function.md) belongs to [L2 space](../../../../../../l2-space-is-a-hilbert-space.md).

For the specified nuisance [statistical path](../../../../../../statistical-path.md), differentiating $\log(1+t\gamma(e))$ at zero gives the [score function](../../../../../../informant-function.md) $\gamma(e)$. Normalization requires $E_f\gamma=0$. There is a second constraint: the [statistical path](../../../../../../statistical-path.md) must preserve the model's zero error [expected value](../../../../../../expected-value.md). Thus

$$
0=\int e f(e)(1+t\gamma(e))\,de=t\int e\gamma(e)f(e)\,de,
\qquad\boxed{E_f[\varepsilon\gamma(\varepsilon)]=0.}
$$

This constraint follows from being a path through the model, rather than from normalization alone. For a centered symmetric [logistic distribution](../../../../../../logistic-distribution.md), for example, $\gamma(e)=\tanh(e)$ is bounded and has zero [expected value](../../../../../../expected-value.md), but $E[\varepsilon\tanh(\varepsilon)]>0$; it would not preserve the mean.

For any $\psi\in L^2(v)$, [independence](../../../../../../independent-random-variables.md) implies

$$
E[\gamma(\varepsilon)\varepsilon\psi(X)]
=E_f[\varepsilon\gamma(\varepsilon)]E_v\psi(X)=\boxed{0}.
$$

All these products are integrable by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), since $\varepsilon\psi(X)$ is [square-integrable](../../../../../../square-integrable-function.md). Thus every such error-density [score function](../../../../../../informant-function.md) is orthogonal to every $e\psi(x)$. Covariate-density nuisance [score functions](../../../../../../informant-function.md) $b(X)$ are also orthogonal to these [functions](../../../../../../function-split.md), since $E\varepsilon=0$. This is the [mean-preserving error tangent space](../../../../../../mean-preserving-error-tangent-space.md) orthogonality used in the final calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
