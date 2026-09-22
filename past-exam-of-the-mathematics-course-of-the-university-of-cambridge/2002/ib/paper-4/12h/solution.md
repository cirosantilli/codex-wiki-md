<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

A [prior distribution](../../../../../prior-probability.md) assigns uncertainty to a parameter before observing data. Multiplying its density by the [likelihood](../../../../../likelihood-function.md) and normalizing gives the [posterior distribution](../../../../../bayesian-posterior.md). A [Bayes estimator](../../../../../bayes-estimator.md) minimizes the posterior expected [loss function](../../../../../loss-function.md) for each observed sample, and therefore minimizes integrated Bayes risk when the expectations exist.

For [quadratic loss](../../../../../squared-error-loss.md) $(d-\theta)^2$, the conditional risk is $\operatorname{Var}(\theta\mid x)+(d-E(\theta\mid x))^2$, so its minimizer is the posterior mean. For [absolute loss](../../../../../absolute-error-loss.md) $|d-\theta|$, the one-sided derivatives or subgradients show that a minimizer is any posterior median, characterized by $P(\theta<d\mid x)\le1/2$ and $P(\theta>d\mid x)\le1/2$.

For the stated [uniform distribution](../../../../../continuous-uniform-distribution.md) sampling model, let $x_{\min}=\min_i x_i$, $x_{\max}=\max_i x_i$. The [likelihood](../../../../../likelihood-function.md) is $2^{-n}$ on $x_{\max}-1<\theta<x_{\min}+1$ and zero elsewhere. Intersecting this interval with the [uniform prior](../../../../../uniform-prior.md) gives

$$
A=\max(20,x_{\max}-1),\qquad B=\min(50,x_{\min}+1).
$$

When $A<B$, the [bounded uniform-location posterior](../../../../../bounded-uniform-location-posterior.md) is

$$
\boxed{\pi(\theta\mid\mathbf x)=\frac1{B-A}\mathbf1_{(A,B)}(\theta),\qquad \widehat\theta_{\rm quadratic}=\widehat\theta_{\rm absolute}=\frac{A+B}{2}.}
$$

The posterior is symmetric, so its mean and unique median coincide. If $A\ge B$, the data have zero marginal [likelihood](../../../../../likelihood-function.md) under the stipulated prior/sampling model and this posterior density cannot be normalized. An empty or singleton intersection is not an ordinary uniform posterior of positive width.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
