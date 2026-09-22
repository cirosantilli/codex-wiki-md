<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [semimartingale integration by parts](../../../../../semimartingale-integration-by-parts.md) gives

$$
d(X_tM_t)=X_t\,dM_t+M_t\,dX_t+d\langle X,M\rangle_t,
\qquad M_t=M(h)_t.
$$

Here $d\langle X,M\rangle_t=h(t)M_tdt$. Substitution therefore gives cancellation of the drift:

$$
dY_t=X_th(t)M_t\,dB_t+M_t(-h(t)dt+dB_t)+h(t)M_tdt
=\boxed{M_t(1+h(t)X_t)\,dB_t.}
$$

The continuous [adapted](../../../../../adapted-process.md) [integrand](../../../../../integrand.md) is locally square integrable. Stopping when $|X|+M$ first exceeds an integer produces true stochastic-integral [martingales](../../../../../martingale-split.md), hence $Y$ is a **[local martingale](../../../../../local-martingale.md)**. No unproved global integrability of the product is needed.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
