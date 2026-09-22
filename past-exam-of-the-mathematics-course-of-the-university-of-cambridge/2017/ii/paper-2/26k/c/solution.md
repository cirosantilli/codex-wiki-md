<h1 id="26k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The support restricts $\theta$ to $\theta>0$, $\theta\leq X_{(1)}$ and $\theta\geq X_{(n)}-1$. Within its feasible interior, the [likelihood function](../../../../../../likelihood-function.md) is proportional to $\prod_i(X_i-\theta)^{-\alpha}$ and is strictly increasing in $\theta$, diverging as $\theta\uparrow X_{(1)}$. Under the printed infinite-endpoint-density, or extended-likelihood convention, the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta_n=X_{(1)}.}
$$

A density is defined only almost everywhere. If its value at the singular endpoint is reassigned a finite value, a finite maximum need not exist; the sample-minimum answer uses the stated endpoint/supremum convention.

Independence and $\mathbb P(Y\leq t)=t^r$ on $[0,1]$ give

$$
\boxed{\mathbb P(\widehat\theta_n-\theta>t)=\begin{cases}1,&t\leq0,\\(1-t^r)^n,&0<t<1,\\0,&t\geq1.\end{cases}}
$$

The error is positive almost surely, so the estimator is not an [unbiased estimator](../../../../../../unbiased-estimator.md). More explicitly its [bias](../../../../../../bias-of-an-estimator.md) is

$$
\mathbb E(\widehat\theta_n-\theta)=\int_0^1(1-t^r)^n\,dt
=\frac{\Gamma(1+1/r)\Gamma(n+1)}{\Gamma(n+1+1/r)}>0.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26K](../../26k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
