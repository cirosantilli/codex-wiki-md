<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the first equation use an integrating factor. The [Itô product rule](../../../../../ito-product-rule.md) gives $d(e^{\lambda t}X_t)=\sigma e^{\lambda t}dB_t$, so

$$
X_t=e^{-\lambda t}\left(1+\sigma\int_0^t e^{\lambda s}\,dB_s\right).
$$

The [Gaussianity of deterministic Brownian stochastic integrals](../../../../../gaussianity-of-deterministic-brownian-stochastic-integrals.md) follows by approximating its deterministic integrand by step functions and using the [Itô isometry](../../../../../ito-isometry.md). Hence

$$
\boxed{X_t\sim N\left(e^{-\lambda t},\begin{cases}\displaystyle\frac{\sigma^2(1-e^{-2\lambda t})}{2\lambda},&\lambda\ne0,\\\sigma^2t,&\lambda=0.\end{cases}\right).}
$$

The variance is positive also when $\lambda<0$, since numerator and denominator then both have negative sign. This is the [explicit Ornstein-Uhlenbeck solution](../../../../../explicit-ornstein-uhlenbeck-solution.md) with initial value one.

For the second equation, take independent standard [Brownian motions](../../../../../brownian-motion-split.md) $U,V$ and define $R_t=\sqrt{(1+U_t)^2+V_t^2}$. The associated planar Brownian motion does not hit the origin. To check this rather than silently differentiate at zero, stop its radius upon hitting $\varepsilon$ or $L$, with $0<\varepsilon<1<L$. The function $\log r$ is harmonic on that annulus, so the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\mathbb P_1(T_\varepsilon<T_L)=\frac{\log L}{\log L-\log\varepsilon}.
$$

Let $\varepsilon\downarrow0$: hitting zero before $T_L$ has probability zero. Taking integer $L\to\infty$ covers every possible finite hitting time, since continuous paths are bounded on compact intervals. Thus [planar Brownian motion avoids a fixed point](../../../../../planar-brownian-motion-avoids-a-fixed-point.md) and $R$ stays positive.

The radial [Itô formula](../../../../../ito-s-lemma.md) is now legitimate and gives

$$
dR_t=\frac{1+U_t}{R_t}\,dU_t+\frac{V_t}{R_t}\,dV_t+\frac{1}{2R_t}\,dt.
$$

The sum of the two martingale terms has bracket $t$ and starts at zero, so it is a standard Brownian motion $\beta$ by [Lévy characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md). Thus $dR=d\beta+(2R)^{-1}dt$ with $R_0=1$. The law-determination assumption permitted in the question identifies the law of $Y$ with that of this dimension-two [Bessel process](../../../../../bessel-process.md). For independent standard [normal random variables](../../../../../gaussian-random-variable.md) $G_1,G_2$,

$$
\boxed{Y_t\overset d=\sqrt{(1+\sqrt t\,G_1)^2+tG_2^2}.}
$$

This is the [two-dimensional Bessel transition law](../../../../../two-dimensional-bessel-transition-law.md) and answers the requested distribution without needing a special-function density.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
