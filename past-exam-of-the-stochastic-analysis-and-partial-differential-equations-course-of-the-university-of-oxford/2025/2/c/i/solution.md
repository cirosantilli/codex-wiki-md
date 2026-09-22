<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here the [diffusion generator](../../../../../diffusion-generator.md) is $\mathcal L=ax\partial_x+\tfrac12\sigma^2\partial_{xx}$. The [Feynman-Kac formula](../../../../../feynman-kac-formula.md) gives

$$
F_t+axF_x+\tfrac12\sigma^2F_{xx}=0,\qquad F(T,x)=e^{iux}.
$$

Try $F(t,x)=\exp[iu\alpha(t)x+\beta(t)]$, where $\alpha(T)=1$ and $\beta(T)=0$. Substitution and collection of the coefficients of $x$ and the constant term give

$$
\alpha'(t)+a\alpha(t)=0,\qquad
\beta'(t)=\frac12\sigma^2u^2\alpha(t)^2.
$$

The solutions of these [ordinary differential equations](../../../../../ordinary-differential-equation.md), with the terminal conditions imposed, are

$$
\alpha(t)=e^{a(T-t)},\qquad
\beta(t)=-\frac12\sigma^2u^2\int_t^Te^{2a(T-s)}\,ds.
$$

For $\Delta=T-t$, define the conditional [variance](../../../../../variance-split.md)

$$
v_\Delta=\begin{cases}
\displaystyle\frac{\sigma^2}{2a}(e^{2a\Delta}-1),&a\ne0,\\
\sigma^2\Delta,&a=0.
\end{cases}
$$

Then the required [conditional characteristic function](../../../../../conditional-characteristic-function.md) is

$$
\boxed{\mathbb E[e^{iuX_T}\mid X_t=x]
=\exp\left(iue^{a\Delta}x-\frac12u^2v_\Delta\right).}
$$

In particular, for $a\ne0$ this exponent is $iue^{a\Delta}x-\frac{\sigma^2u^2}{4a}(e^{2a\Delta}-1)$. The [variance](../../../../../variance-split.md) $v_\Delta$ is nonnegative for either sign of $a$, and its limit at $a=0$ is $\sigma^2\Delta$. Hence the solution is bounded in absolute value by one and the [Feynman-Kac formula](../../../../../feynman-kac-formula.md) identifies it with the required expectation. The value $u=0$ gives one directly, including that case without dividing by $u$.

For an independent check, the [integrating factor](../../../../../integrating-factor.md) $e^{-as}$ and the [Itô product rule](../../../../../ito-product-rule.md) give

$$
X_T=e^{a\Delta}x+\sigma\int_t^Te^{a(T-s)}\,dB_s.
$$

The [stochastic integral](../../../../../stochastic-integral.md) has a [normal distribution](../../../../../normal-distribution.md) because its integrand is deterministic; the [Itô isometry](../../../../../ito-isometry.md) gives its [variance](../../../../../variance-split.md) as $v_\Delta$. For $a<0$ this is the [Ornstein-Uhlenbeck transition distribution](../../../../../ornstein-uhlenbeck-transition-distribution.md). The formula also covers the unstable case $a>0$, and degenerates to deterministic motion when $\sigma=0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
