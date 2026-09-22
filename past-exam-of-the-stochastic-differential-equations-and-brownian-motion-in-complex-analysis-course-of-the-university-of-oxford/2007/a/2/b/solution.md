<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $X$ is [Brownian motion](../../../../../brownian-motion-split.md) with respect to the given [filtration](../../../../../filtration-probability-theory.md), independent Gaussian increments give the identity immediately.

Conversely, fix $s<t$ and let $\Delta=X_t-X_s$. Taking expectations gives its [characteristic function](../../../../../characteristic-function-split.md) $e^{-\xi^2(t-s)/2}$, so $\Delta\sim N(0,t-s)$. To prove [independence](../../../../../independent-random-variables.md), for any $A\in\mathcal F_s$ define the [finite measure](../../../../../finite-measure.md) $\nu_A(E)=\mathbb P(A\cap\{\Delta\in E\})$. The conditional identity gives

$$
\int e^{i\xi u}\nu_A(du)
=\mathbb P(A)e^{-\xi^2(t-s)/2}.
$$

Uniqueness of [Fourier transforms](../../../../../fourier-transform-split.md) of [finite measures](../../../../../finite-measure.md) implies $\nu_A=\mathbb P(A)N(0,t-s)$. This is [independence](../../../../../independent-random-variables.md) of $\Delta$ from $\mathcal F_s$. Iterating over times proves [independent increments](../../../../../independent-increments.md). Together with the stated [continuity](../../../../../continuous-function.md) and $X_0=0$, this gives **standard [Brownian motion](../../../../../brownian-motion-split.md)**.

Here a process with the stated [filtration](../../../../../filtration-probability-theory.md) is understood to be [adapted](../../../../../adapted-process.md), as required when saying it is Brownian with respect to that [filtration](../../../../../filtration-probability-theory.md). If adaptedness is not implicit, it must be added: an ordinary [Brownian motion](../../../../../brownian-motion-split.md) with a trivial [filtration](../../../../../filtration-probability-theory.md) satisfies the displayed [conditional characteristic function](../../../../../conditional-characteristic-function.md) but is not [adapted](../../../../../adapted-process.md) to that [filtration](../../../../../filtration-probability-theory.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
