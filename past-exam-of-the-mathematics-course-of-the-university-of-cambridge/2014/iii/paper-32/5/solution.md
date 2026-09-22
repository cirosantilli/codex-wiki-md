<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a proper continuous event time, the [survival function](../../../../../survival-function.md) is $S(t)=e^{-H(t)}$. The assumed invertibility of the [cumulative hazard function](../../../../../cumulative-hazard-function.md) gives, for $u\ge0$,

$$
P\{H(T)>u\}=P\{T>H^{-1}(u)\}=e^{-H(H^{-1}(u))}=e^{-u}.
$$

Therefore

$$
\boxed{U=H(T)\sim\operatorname{Exp}(1).}
$$

This is the [cumulative hazard probability transformation](../../../../../cumulative-hazard-probability-transformation.md); it applies also conditionally on a subject's covariates, using that subject's correctly specified [cumulative hazard function](../../../../../cumulative-hazard-function.md).

The fitted transformed times are [Cox–Snell residuals](../../../../../cox-snell-residual.md). They retain their event/[right censoring](../../../../../right-censoring.md) indicators, so a [right-censored](../../../../../right-censoring.md) residual represents an exponential observation known only to exceed its displayed value. Under the fitted model and independent [right censoring](../../../../../right-censoring.md), calculate the [Kaplan–Meier estimator](../../../../../kaplan-meier-estimator.md) of residual survival and compare it with $e^{-y}$, or calculate the residual [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md) and compare its [cumulative hazard](../../../../../cumulative-hazard-function.md) with the diagonal $H(y)=y$. Systematic departures reveal model inadequacy; sparse extreme residual [risk sets](../../../../../risk-set.md) and parameter estimation require caution. Treating all censored residuals as observed event times would invalidate this diagnostic.

Without [right censoring](../../../../../right-censoring.md), the residual mean should be approximately one. With [right censoring](../../../../../right-censoring.md), use the [modified Cox–Snell residual](../../../../../modified-cox-snell-residual.md)

$$
\boxed{y_i^*=y_i+(1-v_i).}
$$

For a true unit-rate [exponential distribution](../../../../../exponential-distribution.md), the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) gives $E(U\mid U>c)=c+1$. Thus an event keeps its known transformed time, while a censored observation is replaced by the conditional expected event time. Under independent [right censoring](../../../../../right-censoring.md), iterated [expectation](../../../../../expected-value.md) makes the mean of these adjusted values one when the true hazards are used, and approximately one when fitted hazards are used. These mean-imputed values do not themselves have an exponential distribution, so the survival-curve diagnostic should still use the original censored residual dataset. Moreover fitting equations can force the adjusted sample mean to one, making its mean alone a weak diagnostic.

For the proposed mixture of a finite [right censoring](../../../../../right-censoring.md) time $c\ge0$ and no [right censoring](../../../../../right-censoring.md), $P(C<U)=\pi e^{-c}$ and

$$
E\{\min(U,C)\}=(1-\pi)E(U)+\pi\int_0^cP(U>u)\,du=1-\pi e^{-c}.
$$

Consequently

$$
\boxed{E(U^*)=1+(k-1)\pi e^{-c},\qquad k=1.}
$$

When [right censoring](../../../../../right-censoring.md) has positive [probability](../../../../../probability.md) this choice is unique; if $\pi e^{-c}=0$, no correction is needed and any $k$ has the same effect. Its independence from $c$ is the content of exponential memorylessness: the expected extra lifetime after any [right censoring](../../../../../right-censoring.md) time is one. Conditioning on an arbitrary independent [right censoring](../../../../../right-censoring.md) time proves the same correction beyond this special two-point mixture.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
