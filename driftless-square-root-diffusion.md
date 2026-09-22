# Driftless square-root diffusion

↑ **Parent:** [Markov diffusion](markov-diffusion.md)

A driftless square-root [diffusion process](markov-diffusion.md) is the nonnegative solution of $dX_t=\sqrt{X_t}\,dW_t$, with zero an absorbing boundary. For elapsed time $h>0$, starting from $x\geq0$, its [Laplace transform](laplace-transform.md) is

$$
\mathbb E_x[e^{-uX_h}]=\exp\left(-\frac{xu}{1+uh/2}\right),\qquad u\geq0.
$$

To prove this, fix the final time $h$ and set $F(t,x)=\exp[-xu/(1+u(h-t)/2)]$. Differentiation gives $F_t+\tfrac12xF_{xx}=0$, while $F(h,x)=e^{-ux}$. By [Itô formula](ito-s-lemma.md), $F(t,X_t)$ is a [local martingale](local-martingale.md); it takes values in $[0,1]$, so localization and bounded convergence make it a true [martingale](martingale-split.md). Taking expectations at the two endpoints proves the formula. The [Markov property](markov-property.md) gives the same formula conditionally at any starting time.

**Table of contents**

- [Compound Poisson transition law of a driftless square-root diffusion](compound-poisson-transition-law-of-a-driftless-square-root-diffusion.md)

## ↑ Ancestors (9)

1. [Markov diffusion](markov-diffusion.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Compound Poisson transition law of a driftless square-root diffusion](compound-poisson-transition-law-of-a-driftless-square-root-diffusion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/iii/solution.md)
