<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $a(t)=e^{\int_0^t\mu(s)ds}$ and $q(t)=a(t)^{-1}$. Since $q'=-\mu q$ and $q$ has [finite variation](../../../../../total-variation-of-a-function.md), the product rule has no quadratic-covariation contribution:

$$
d(qX)=q\,dX+X\,dq=q(t)\sigma(t)dB_t.
$$

Integrating and multiplying by $a(t)$ yields

$$
\boxed{X(t,x)=a(t)\left[x+\int_0^ta(s)^{-1}\sigma(s)dB_s\right].}
$$

The deterministic [integrand](../../../../../integrand.md) is square integrable on every [compact](../../../../../compact-space.md) interval. This constructs a strong solution. Two solutions driven by the same [Brownian motion](../../../../../brownian-motion-split.md) have difference solving $dD=\mu Ddt$, $D_0=0$, hence their difference vanishes, proving [pathwise uniqueness](../../../../../pathwise-uniqueness.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
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
