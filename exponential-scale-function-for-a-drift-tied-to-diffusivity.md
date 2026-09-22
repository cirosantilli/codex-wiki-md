# Exponential scale function for a drift tied to diffusivity

↑ **Parent:** [Scale function (stochastic processes)](scale-function-stochastic-processes.md)

For the displayed [stochastic differential equation](stochastic-differential-equation.md), the [infinitesimal generator](infinitesimal-generator-stochastic-processes.md) is $\mathcal Lg=(f^2/2)(g''-g')$, so $\mathcal Ls=0$ and the [Itô formula](ito-s-lemma.md) makes $e^{X_t}$ a positive [local martingale](local-martingale.md). If $f$ is bounded, strictly positive, and [globally Lipschitz](globally-lipschitz-function.md), the equation has a unique global [strong solution of a stochastic differential equation](strong-solution-of-a-stochastic-differential-equation.md). For $a<x<b$ and $T_y=\inf\{t:X_t=y\}$, the [Itô isometry](ito-isometry.md) for the bounded stopped exponential gives finite mean exit time: the bracket density $e^{2z}f(z)^2$ has a positive minimum on $[a,b]$. The [optional stopping theorem](optional-sampling-theorem-for-a-supermartingale.md) then yields the [boundary hitting probability from a diffusion scale function](boundary-hitting-probability-from-a-diffusion-scale-function.md)

$$
\mathbb P_x(T_b<T_a)=\frac{e^x-e^a}{e^b-e^a}.
$$

Taking $a\to-\infty$ gives $\mathbb P_x(T_b<\infty)=e^{x-b}$ for $b>x$. Passing to strict exceedances and then to their limits shows that $\sup_{t\geq0}X_t-x$ has the [exponential distribution](exponential-distribution.md) of rate one. The [probability distribution](probability-distribution-split.md) of the maximum is independent of the particular $f$; changing the speed of motion preserves this [scale function](scale-function-stochastic-processes.md).

## ↑ Ancestors (9)

1. [Scale function (stochastic processes)](scale-function-stochastic-processes.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2025/3/c/solution.md)
