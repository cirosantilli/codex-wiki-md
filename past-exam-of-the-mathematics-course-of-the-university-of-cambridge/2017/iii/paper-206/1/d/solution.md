<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Introduce a latent [Bernoulli distribution](../../../../../../bernoulli-distribution.md) indicator $A_i$, with $A_i=1$ denoting a structural zero and $\Pr(A_i=1)=\pi$. Conditional on $A_i=0$, retain the [negative binomial regression](../../../../../../negative-binomial-regression.md) with $\lambda_i=e^{x_i^T\beta}$ and $x_i=(1,d_i)^T$. This gives a [zero-inflated negative binomial model](../../../../../../zero-inflated-negative-binomial-model.md):

$$
\boxed{\Pr(Y_i=0)=\pi+(1-\pi)f_{\rm NB}(0;r,\lambda_i),\quad \Pr(Y_i=y)=(1-\pi)f_{\rm NB}(y;r,\lambda_i)\quad(y>0).}
$$

A participant who fishes may still catch zero, so an observed zero does not reveal the latent class. This distinguishes [zero inflation](../../../../../../zero-inflation.md) from a [hurdle model](../../../../../../hurdle-model.md), which truncates the count component at zero. The marginal [expectation](../../../../../../expected-value.md) becomes $(1-\pi)\lambda_i$, and the [law of total variance](../../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}(Y_i)=(1-\pi)\left(\lambda_i+\frac{\lambda_i^2}{r}\right)+\pi(1-\pi)\lambda_i^2.
$$

A constant $\pi$ is a parsimonious starting model. If there is evidence that nonparticipation changes with day or other recorded predictors, use [logistic regression](../../../../../../logistic-regression.md) for $\pi_i$ instead. Conditional [independence](../../../../../../independent-random-variables.md) of visitors remains an assumption; extra zeros alone do not establish its validity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
