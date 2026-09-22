# Finite lifetime threshold for a power diffusion

↑ **Parent:** [Power diffusion](power-diffusion.md)

For the positive-domain [power diffusion](power-diffusion.md) with $0<\alpha\leq1$, assuming the lifetime is the limit of the hitting times of $1/n$, it is finite [almost surely](almost-sure-convergence.md) exactly when $\alpha<1$. For $\alpha<1$, the [Itô formula](ito-s-lemma.md) gives

$$
d(X^{1-\alpha})=(1-\alpha)dB-\frac{\alpha(1-\alpha)}{2X^{1-\alpha}}dt.
$$

The negative drift bounds this positive process above by $X_0^{1-\alpha}+(1-\alpha)B$, whose first hit of zero is finite by [recurrence of one-dimensional Brownian motion](recurrence-of-one-dimensional-brownian-motion.md). The lifetime must precede that hit. At $\alpha=1$, $X_t=X_0e^{B_t-t/2}$ is positive and finite on every compact time interval, so the lifetime is infinite. Approaching zero only as $t\to\infty$ is not a finite boundary lifetime.

## ↑ Ancestors (10)

1. [Power diffusion](power-diffusion.md)
2. [Itô diffusion](ito-diffusion.md)
3. [Stochastic differential equation](stochastic-differential-equation.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202/5/e/solution.md)
