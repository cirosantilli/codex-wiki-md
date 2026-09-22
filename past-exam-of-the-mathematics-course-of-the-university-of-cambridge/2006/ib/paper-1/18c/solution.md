<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

A [sufficient statistic](../../../../../sufficient-statistic.md) $T(X)$ for $\theta$ is a function of the observations whose conditional distribution of $X$ given $T(X)$ does not depend on $\theta$, whenever that conditioning event is possible. It retains all parameter dependence of the [likelihood](../../../../../likelihood-function.md).

In the discrete case the [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) provides a direct criterion: $f(x\mid\theta)=g(T(x),\theta)h(x)$, where $h$ is independent of the parameter. To justify sufficiency, for a value $t$ with positive probability, sum this expression over its fiber and divide:

$$
\mathbb P_\theta(X=x\mid T=t)=\frac{h(x)}{\sum_{y:T(y)=t}h(y)},\qquad T(x)=t.
$$

The parameter-dependent factor cancels. Conversely, parameter-independent conditional probabilities $h_t(x)$ give the factorization $f(x\mid\theta)=\mathbb P_\theta(T=t)h_t(x)$ with $t=T(x)$. Thus the criterion is both necessary and sufficient, with conditional laws only required on fibers of positive probability.

For the shifted exponential sample the [likelihood](../../../../../likelihood-function.md) is

$$
f(x\mid\theta)=\lambda^n e^{-\lambda\sum_i x_i}e^{n\lambda\theta}\mathbf1_{\{\theta\le\min_i x_i\}},\qquad\theta\ge0.
$$

It factors through $T=X_{(1)}=\min_iX_i$, so **the sample minimum is a [sufficient statistic](../../../../../sufficient-statistic.md)**. Writing $Y_i=X_i-\theta$, independence gives for $t\ge0$

$$
\mathbb P(T-\theta>t)=\prod_i\mathbb P(Y_i>t)=e^{-n\lambda t}.
$$

Therefore $T-\theta$ is exponential with rate $n\lambda$. Its [mean](../../../../../expected-value.md) is $(n\lambda)^{-1}$ and its [variance](../../../../../variance-split.md) is $(n\lambda)^{-2}$. The [unbiased endpoint estimator for a shifted exponential sample](../../../../../unbiased-endpoint-estimator-for-a-shifted-exponential-sample.md) is consequently

$$
\boxed{\widehat\theta=X_{(1)}-\frac1{n\lambda},\quad
\mathbb E_\theta[\widehat\theta]=\theta,\quad
\operatorname{Var}_\theta(\widehat\theta)=\frac1{(n\lambda)^2}.}
$$

Although the parameter is nonnegative, this [unbiased estimator](../../../../../unbiased-estimator.md) can be negative. Truncating it at zero would change its expectation and lose the requested property of an [unbiased estimator](../../../../../unbiased-estimator.md).

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
