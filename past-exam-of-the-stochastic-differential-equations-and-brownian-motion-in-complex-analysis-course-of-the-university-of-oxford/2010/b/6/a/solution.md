<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use first that [planar Brownian motion avoids a fixed point](../../../../../planar-brownian-motion-avoids-a-fixed-point.md), so the path starting at $1$ never reaches zero. Its continuous logarithmic lift, initialized at zero, has real part $U_t=\log|Z_t|$ and imaginary part the continuous unwrapped angle $\Theta_t$. Local branches of the complex logarithm, patched along the path, and the [Itô formula](../../../../../ito-s-lemma.md) show that both coordinates are [continuous local martingales](../../../../../continuous-local-martingale.md) with

$$
\langle U\rangle_t=\langle\Theta\rangle_t=\int_0^t\frac{ds}{|Z_s|^2}=:\tau(t),\qquad
\langle U,\Theta\rangle_t=0.
$$

The clock is finite on every compact time interval, since a continuous nonvanishing path stays a positive distance from zero there. It is continuous and strictly increasing. Moreover $\tau(\infty)=\infty$: by recurrence, planar Brownian motion spends infinite total time in a fixed disk, and inside the unit disk the clock integrand is at least one. This is the [divergence of a positive planar Brownian occupation integral](../../../../../divergence-of-a-positive-planar-brownian-occupation-integral.md).

The [common-clock time change of orthogonal local martingales](../../../../../common-clock-time-change-of-orthogonal-local-martingales.md), using the [Lévy characterization of multidimensional Brownian motion](../../../../../levy-characterization-of-multidimensional-brownian-motion.md), supplies independent Brownian coordinates $\zeta^1,\zeta^2$ such that $U_t+i\Theta_t=\zeta_{\tau(t)}$. Exponentiating gives

$$
\boxed{Z_t=\exp(\zeta_{\tau(t)}),\qquad\zeta_0=0.}
$$

To identify the inverse clock, write $A=\tau^{-1}$. The derivative of an inverse function and the representation just obtained give

$$
A'(s)=|Z_{A(s)}|^2=e^{2\zeta_s^1},\qquad
A(s)=\int_0^s e^{2\zeta_u^1}du.
$$

Consequently

$$
\boxed{\tau(t)=\int_0^t|Z_s|^{-2}ds
=\inf\left\{s\geq0:\int_0^s e^{2\zeta_u^1}du>t\right\}.}
$$

The strict inequality in this generalized inverse has the same infimum as the unique inverse value, since $A$ is continuous and strictly increasing onto the half-line.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
