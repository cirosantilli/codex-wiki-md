<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

A [generalized linear model](../../../../../generalized-linear-model.md) has independent responses whose distributions belong to an [exponential family](../../../../../exponential-family-split.md):

$$
f_i(y_i;\theta_i,\phi)=\exp\left\{\frac{y_i\theta_i-b(\theta_i)}{a_i(\phi)}+c_i(y_i,\phi)\right\}.
$$

Here the [expected value](../../../../../expected-value.md) and [variance](../../../../../variance-split.md) are $\mu_i=b'(\theta_i)$ and $\operatorname{Var}(Y_i)=a_i(\phi)b''(\theta_i)$. A specified one-to-one [link function](../../../../../link-function.md) $g$ connects the mean to the [linear predictor](../../../../../linear-predictor.md): $g(\mu_i)=x_i^T\beta$. The [canonical link function](../../../../../canonical-link-function.md) is $g(\mu_i)=\theta_i$.

In [binomial regression](../../../../../binomial-regression.md), $Y_i\sim\operatorname{Bin}(m_i,p_i)$ independently, with known trial counts $m_i$ and probabilities related to the predictor. The [logistic regression](../../../../../logistic-regression.md) and [probit regression](../../../../../probit-model.md) specifications are respectively

$$
\boxed{\log\frac{p_i}{1-p_i}=x_i^T\beta,\quad p_i=\frac{e^{x_i^T\beta}}{1+e^{x_i^T\beta}};\qquad \Phi^{-1}(p_i)=x_i^T\beta,\quad p_i=\Phi(x_i^T\beta).}
$$

Here $\Phi$ is the standard [normal distribution](../../../../../normal-distribution.md) function. The binomial log-density contains $y_i\log(p_i/(1-p_i))+m_i\log(1-p_i)$, so its natural parameter is the log-odds: the logistic link is canonical. If the response mean is written as $\mu_i=m_ip_i$, the canonical link is $g_i(\mu_i)=\log(\mu_i/(m_i-\mu_i))$.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
