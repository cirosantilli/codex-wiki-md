# Joint Laplace transform of Brownian square and its time integral

↑ **Parent:** [Laplace transform of the integrated square of Brownian motion](laplace-transform-of-the-integrated-square-of-brownian-motion.md)

For standard [Brownian motion](brownian-motion-split.md) and $\alpha,t\geq0$, $\beta>0$, the title gives the joint [Laplace transform](laplace-transform.md) of the terminal square and the [integrated square of Brownian motion](integrated-square-of-brownian-motion.md). At $\beta=0$ the answer is $(1+2\alpha t)^{-1/2}$. To prove the formula, use the [stochastic exponential](doleans-dade-exponential.md)

$$
Z_t=\exp\!\left[-\beta\int_0^tB_s\,dB_s-\frac{\beta^2}{2}\int_0^tB_s^2ds\right]
=\exp\!\left[\frac{\beta t}{2}-\frac\beta2B_t^2-\frac{\beta^2}{2}\int_0^tB_s^2ds\right].
$$

On every finite interval $[0,T]$, $0<Z_t\leq e^{\beta T/2}$, so the [bounded local martingale criterion](bounded-local-martingale-criterion.md) makes it a [martingale](martingale-split.md). The [Girsanov theorem](girsanov-theorem.md) changes $B$ into the zero-started [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md) $dB=dW-\beta Bdt$ under the terminal density $Z_t$. Its terminal [variance](variance-split.md) is $v=(1-e^{-2\beta t})/(2\beta)$. Multiplying $Z_t$ by $\exp[(\beta/2-\alpha)B_t^2-\beta t/2]$ recovers the integrand on the left of the title. The [Gaussian quadratic exponential moment](gaussian-quadratic-exponential-moment.md) then gives $e^{-\beta t/2}[1-(\beta-2\alpha)v]^{-1/2}$, which simplifies to the title formula. At $\alpha=0$ this reduces to the [Laplace transform of the integrated square of Brownian motion](laplace-transform-of-the-integrated-square-of-brownian-motion.md) after [Brownian scaling](brownian-scaling.md).

## ↑ Ancestors (9)

1. [Laplace transform of the integrated square of Brownian motion](laplace-transform-of-the-integrated-square-of-brownian-motion.md)
2. [Integrated square of Brownian motion](integrated-square-of-brownian-motion.md)
3. [Brownian motion](brownian-motion-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2025/2/c/ii/solution.md)
