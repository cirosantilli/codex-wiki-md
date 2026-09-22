<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Itô's formula](../../../../../ito-s-lemma.md) identifies the [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) on twice continuously differentiable functions:

$$
\boxed{(Lf)(z)=rzf'(z)+\tfrac12\sigma^2z^2f''(z).}
$$

Subtract the [drift coefficient](../../../../../drift-coefficient.md) integral from that formula to obtain

$$
M_t^f=\int_0^t\sigma X_s f'(X_s)\,dB_s.
$$

Stopping when $|X|$ leaves a bounded interval makes the integrand bounded on each finite time interval. Therefore $M^f$ is a continuous [local martingale](../../../../../local-martingale.md). In fact $f'\in L^\infty$ and the [lognormal distribution](../../../../../log-normal-distribution.md) solution has finite second moments on finite intervals, so here it is square integrable on each such interval as well.

The [quadratic covariation](../../../../../quadratic-covariation.md) of two [stochastic integrals](../../../../../stochastic-integral.md) against the same [Brownian motion](../../../../../brownian-motion-split.md) is the integral of the product of their integrands. Consequently

$$
\boxed{\langle M^f,M^g\rangle_t
=\sigma^2\int_0^tX_s^2 f'(X_s)g'(X_s)\,ds.}
$$

This is the [quadratic covariation](../../../../../quadratic-covariation.md), which agrees with the pathwise [quadratic covariation](../../../../../quadratic-covariation.md) for these continuous [local martingales](../../../../../local-martingale.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
