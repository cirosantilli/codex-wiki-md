<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $F_t=e^{\alpha B_t-\alpha^2t/2}$, a positive [stochastic exponential](../../../../../../doleans-dade-exponential.md) with $dF_t=\alpha F_t\,dB_t$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(F_t^{-1})=-\alpha F_t^{-1}dB_t+\alpha^2F_t^{-1}dt.
$$

For $Y=X/F$, the [Itô product rule](../../../../../../ito-product-rule.md) and $d[X,F^{-1}]_t=-\alpha^2X_tF_t^{-1}dt$ cancel both the Brownian terms and the extra drift. Consequently

$$
\boxed{dY_t=F_t^{\delta-1}Y_t^\delta\,dt,\qquad Y_0=x_0.}
$$

This is an ordinary [Bernoulli differential equation](../../../../../../bernoulli-differential-equation.md) with continuous random coefficients. For $\delta\ne1$, separate variables to obtain

$$
Y_t^{1-\delta}=x_0^{1-\delta}+(1-\delta)\int_0^tF_s^{\delta-1}ds.
$$

Therefore the [Bernoulli stochastic differential equation](../../../../../../bernoulli-stochastic-differential-equation.md) has the explicit maximal positive solution

$$
\boxed{X_t=F_t\left[x_0^{1-\delta}+(1-\delta)\int_0^tF_s^{\delta-1}ds\right]^{1/(1-\delta)},\quad\delta\ne1,}
$$

valid while its bracket remains strictly positive. When $\delta=1$, the reduced equation is $dY_t=Y_tdt$, and

$$
\boxed{X_t=x_0\exp\!\left(\alpha B_t+\left(1-\frac{\alpha^2}{2}\right)t\right).}
$$

Substituting these expressions back through the product rule verifies the original [stochastic differential equation](../../../../../../stochastic-differential-equation.md), not just the reduced equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
