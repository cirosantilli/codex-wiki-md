<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use positive initial asset prices and the usual augmentation of the [natural Brownian filtration](../../../../../../natural-brownian-filtration.md). Define the [market price of risk](../../../../../../market-price-of-risk.md)

$$
\boxed{\lambda_t=\frac{\mu_t-r_t}{\sigma_t}.}
$$

Continuity and strict positivity of $\sigma$ imply $\int_0^T\lambda_t^2dt<\infty$ on every finite horizon [almost surely](../../../../../../almost-sure-convergence.md), because each path has a positive minimum of $\sigma$ there. Hence the strictly positive [stochastic exponential](../../../../../../doleans-dade-exponential.md)

$$
\boxed{Y_t=\exp\!\left(-\int_0^tr_sds-\int_0^t\lambda_s\,dW_s-\frac12\int_0^t\lambda_s^2ds\right)}
$$

is defined and has $Y_0=1$ and $dY_t=-Y_t(r_tdt+\lambda_tdW_t)$. The [Itô product rule](../../../../../../ito-product-rule.md) gives

$$
d(Y_tB_t)=-Y_tB_t\lambda_t\,dW_t,\qquad d(Y_tS_t)=Y_tS_t(\sigma_t-\lambda_t)\,dW_t,
$$

so it is a [local martingale deflator](../../../../../../local-martingale-deflator.md).

For uniqueness, let $\widetilde Y$ be any normalized strictly positive [local martingale deflator](../../../../../../local-martingale-deflator.md). The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) makes $B\widetilde Y$ a continuous [local martingale](../../../../../../local-martingale.md) with a [Brownian motion](../../../../../../brownian-motion-split.md) integral representation. Dividing by $B$ therefore gives $d\widetilde Y=-r\widetilde Ydt+\eta dW$. The vanishing [drift](../../../../../../drift-coefficient.md) of $S\widetilde Y$ requires $\widetilde Y(\mu-r)+\eta\sigma=0$, so $\eta=-\widetilde Y\lambda$. This scalar linear [stochastic differential equation](../../../../../../stochastic-differential-equation.md) has exactly the exponential solution above, proving **the normalized [local martingale deflator](../../../../../../local-martingale-deflator.md) is unique.**

The assumptions do not make $\lambda$ deterministically bounded: $\sigma$ need not be bounded away from zero uniformly over outcomes. Thus a true [martingale](../../../../../../martingale-split.md) density or [Novikov condition](../../../../../../novikov-s-condition.md) is not inferred here; the required conclusion is local.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
