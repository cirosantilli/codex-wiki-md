<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $0<\alpha<1$, use the power transformation $Y=X^{1-\alpha}$ on the positive [stochastic interval](../../../../../../stochastic-interval.md). The [Itô formula](../../../../../../ito-s-lemma.md), with $d[X]=X^{2\alpha}dt$, gives

$$
dY_t=(1-\alpha)\,dB_t-\frac{\alpha(1-\alpha)}{2Y_t}\,dt,\qquad Y_0=x_0^{1-\alpha}.
$$

Thus $Y_t\leq x_0^{1-\alpha}+(1-\alpha)B_t$ simultaneously for $t<T$. The right side reaches zero [almost surely](../../../../../../almost-sure-convergence.md) by [recurrence of one-dimensional Brownian motion](../../../../../../recurrence-of-one-dimensional-brownian-motion.md), and the same positive-path contradiction proves $T$ cannot exceed that [Brownian first-passage time](../../../../../../brownian-first-passage-time.md). This establishes the [finite lifetime threshold for a power diffusion](../../../../../../finite-lifetime-threshold-for-a-power-diffusion.md) throughout $0<\alpha<1$.

At $\alpha=1$, the solution is the [geometric Brownian motion](../../../../../../geometric-brownian-motion.md)

$$
X_t=x_0\exp(B_t-t/2).
$$

It is finite and positive at every finite time. On every compact time interval it has a positive minimum, so the hitting times of $1/n$ tend to infinity. Although the [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md) implies $X_t\to0$ as $t\to\infty$, this is not a finite lifetime. Therefore

$$
\boxed{\mathbb P(T<\infty)=\begin{cases}1,&0<\alpha<1,\\0,&\alpha=1.\end{cases}}
$$

The power transformation is a rescaled [Lamperti transform](../../../../../../lamperti-transform-diffusion.md); at $\alpha=1$ the corresponding transformation is the [logarithm](../../../../../../logarithm.md). No claim about [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) after adjoining the boundary zero is needed: the coefficients are locally [Lipschitz continuous](../../../../../../lipschitz-continuity.md) inside the positive domain, which is the domain of the given [maximal local solution of a stochastic differential equation](../../../../../../maximal-local-solution-of-a-stochastic-differential-equation.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
