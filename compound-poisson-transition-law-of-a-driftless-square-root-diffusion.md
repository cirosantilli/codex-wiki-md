# Compound Poisson transition law of a driftless square-root diffusion

↑ **Parent:** [Driftless square-root diffusion](driftless-square-root-diffusion.md)

The elapsed-time $h>0$ transition distribution of a [driftless square-root diffusion](driftless-square-root-diffusion.md) starting at $x$ is the [compound Poisson distribution](compound-poisson-distribution.md)

$$
X_h\ \stackrel{d}{=}\ \sum_{j=1}^{N}Y_j,\qquad N\sim\operatorname{Poisson}(2x/h),\quad Y_j\sim\operatorname{Exp}(2/h),
$$

where all variables on the right are independent and the empty sum is zero. Here the [exponential distribution](exponential-distribution.md) parameter is its rate. The [Laplace transform](laplace-transform.md) of this sum is

$$
\exp\left[\frac{2x}{h}\left(\frac{2/h}{2/h+u}-1\right)\right]=\exp\left(-\frac{xu}{1+uh/2}\right),
$$

which is the [Laplace transform](laplace-transform.md) of the [driftless square-root diffusion](driftless-square-root-diffusion.md); uniqueness of the [Laplace transform](laplace-transform.md) proves the distributional identity. In particular, for $0\leq v<2/h$, the [exponential moment](exponential-moment.md) is

$$
\mathbb E_x[e^{vX_h}]=\exp\left(\frac{xv}{1-vh/2}\right).
$$

For $x>0$ this [exponential moment](exponential-moment.md) is infinite when $v\geq2/h$, since the event $N=1$ has positive probability and one exponential jump already has an infinite moment there. At $x=0$ the process remains zero and every such moment is one.

## ↑ Ancestors (10)

1. [Driftless square-root diffusion](driftless-square-root-diffusion.md)
2. [Markov diffusion](markov-diffusion.md)
3. [Stochastic differential equation](stochastic-differential-equation.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Exponential claim in a driftless square-root model](exponential-claim-in-a-driftless-square-root-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/iii/solution.md)
