<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Itô formula](../../../../../../ito-s-lemma.md) for $f(t,x)=e^{x+at}$ gives the **[stochastic differential equation](../../../../../../stochastic-differential-equation.md)**

$$
\boxed{dZ_t=Z_t\,dB_t+(a+\tfrac12)Z_t\,dt,\qquad Z_0=1.}
$$

Write $N_t=\int_0^t Z_u\,dB_u$ for its [continuous local martingale](../../../../../../continuous-local-martingale.md) part. Its clock is the [quadratic variation](../../../../../../quadratic-variation.md)

$$
A_t=[Z]_t=[N]_t=\int_0^t Z_u^2du.
$$

Because $Z_t>0$, $A$ is strictly increasing. For $s<A_\infty$, its inverse $\tau_s$ satisfies $A_{\tau_s}=s$ and $d\tau_s/ds=Z_{\tau_s}^{-2}$. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md), or the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) after the [optional time-change theorem](../../../../../../optional-time-change-theorem.md), makes $\beta_s=N_{\tau_s}$ a [Brownian motion](../../../../../../brownian-motion-split.md) for the time-changed [filtration](../../../../../../filtration-probability-theory.md). With $Y_s=Z_{\tau_s}$,

$$
Y_s=1+\beta_s+(a+\tfrac12)\int_0^sY_v^{-1}dv,
\qquad
\boxed{dY_s=d\beta_s+\frac{(2+2a)-1}{2Y_s}ds.}
$$

This is the [Bessel process](../../../../../../bessel-process.md) equation with **dimension $\boxed{2+2a}$**, on the positive stochastic interval. This establishes the [Exponential Brownian-to-Bessel time change](../../../../../../exponential-brownian-to-bessel-time-change.md).

The lifetime convention is important: the inverse is defined only for $s<A_\infty$. If $a<0$, the [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md) gives $B_t/t\to0$, so $Z_t\to0$ exponentially and $A_\infty<\infty$. Then $Y_s\to0$ as $s\uparrow A_\infty$, and this is its first hit of zero after continuous extension. If $a>0$ the clock diverges by the same strong law. If $a=0$ it diverges by [infinite occupation time of one-dimensional Brownian motion](../../../../../../infinite-occupation-time-of-one-dimensional-brownian-motion.md) on a bounded interval, since $e^{2B_t}$ is bounded below there. Thus the lifetime is infinite when $a\geq0$. Negative dimensions are interpreted by the same positive-state equation killed at zero; no post-zero [Bessel process](../../../../../../bessel-process.md) behavior is asserted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
