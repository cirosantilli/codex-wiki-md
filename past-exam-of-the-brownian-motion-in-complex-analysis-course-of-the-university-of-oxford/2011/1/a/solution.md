<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Z_t=z+B_t^1+iB_t^2$, where the coordinates are independent standard [Brownian motions](../../../../brownian-motion-split.md), and write $f=u+iv$. The [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) imply $\Delta u=\Delta v=0$. [Itô's formula](../../../../ito-s-lemma.md) therefore makes

$$
M_t=u(Z_t)-u(z),\qquad N_t=v(Z_t)-v(z)
$$

[continuous local martingales](../../../../continuous-local-martingale.md). Their [quadratic variations](../../../../quadratic-variation.md) and [quadratic covariation](../../../../quadratic-covariation.md) are

$$
\langle M\rangle_t=\langle N\rangle_t=A_t:=\int_0^t|f'(Z_s)|^2ds,\qquad
\langle M,N\rangle_t=0.
$$

Indeed the two gradient norms are equal to $|f'|$, and their dot product vanishes by the Cauchy-Riemann equations.

The clock is finite at every finite time, since a continuous Brownian path has compact range there and $f'$ is continuous. To show its lifetime is infinite, choose a small disc on which $|f'|^2\geq c>0$; such a disc exists because the [entire function](../../../../entire-function.md) is nonconstant. A supporting recurrence result is that planar Brownian motion spends infinite total time in every nonempty open disc almost surely. One proof combines recurrent returns to a smaller disc with the strong Markov property: each visit has a uniformly positive chance of lasting a fixed positive time in the larger disc. Equivalently, use the [divergence of a positive planar Brownian occupation integral](../../../../divergence-of-a-positive-planar-brownian-occupation-integral.md). Therefore

$$
\boxed{A_t\longrightarrow\infty\quad\text{almost surely}.}
$$

Finally the [common-clock time change of orthogonal local martingales](../../../../common-clock-time-change-of-orthogonal-local-martingales.md) states that two continuous local martingales starting at zero with common bracket $A$, zero cross bracket, and $A_\infty=\infty$ are the coordinates of a planar Brownian motion evaluated at $A_t$. Applying it gives a [planar Brownian motion](../../../../planar-brownian-motion.md) $\widetilde Z$ starting at zero with

$$
\boxed{f(Z_t)=f(z)+\widetilde Z_{A_t}.}
$$

This proves [conformal invariance of planar Brownian motion](../../../../conformal-invariance-of-planar-brownian-motion.md) in the entire-function setting, including the [divergence of the conformal Brownian clock for an entire function](../../../../divergence-of-the-conformal-brownian-clock-for-an-entire-function.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Brownian motion in complex analysis course of the University of Oxford](../../../split.md)
5. [Brownian motion in complex analysis course of the University of Oxford](../../../../brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
