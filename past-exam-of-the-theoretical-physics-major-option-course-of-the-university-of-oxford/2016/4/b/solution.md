<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the unwrapped angle on the real line. Integrating its [Langevin equation](../../../../langevin-dynamics.md) gives $\theta(t)-\theta(0)=\omega t+\eta(t)$, where $\eta=\int_0^t\beta(s)ds$ is a centered [Gaussian random variable](../../../../gaussian-random-variable.md) with variance $2D_rt$. Therefore

$$
\boxed{\langle[\theta(t)-\theta(0)]^2\rangle=\omega^2t^2+2D_rt.}
$$

A wrapped angular difference is bounded and would not satisfy this formula.

For the orientation correlation, $\mathbf n(t)\cdot\mathbf n(0)=\cos[\theta(t)-\theta(0)]$. The [characteristic function](../../../../characteristic-function-split.md) gives $\langle e^{i\eta}\rangle=e^{-\langle\eta^2\rangle/2}=e^{-D_rt}$, so

$$
\langle\mathbf n(t)\cdot\mathbf n(0)\rangle=e^{-D_rt}\cos\omega t.
$$

The translational noise is independent of the orientation, hence the cross terms vanish. Summing its two component correlations gives $\langle\mathbf u(t)\cdot\mathbf u(0)\rangle=4D\delta(t)$. Consequently, for $t\ge0$,

$$
\boxed{\langle\mathbf v(t)\cdot\mathbf v(0)\rangle=4D\delta(t)+v^2e^{-D_rt}\cos\omega t.}
$$

The extension to negative time uses $e^{-D_r|t|}$. Because the position contains [Brownian motion](../../../../brownian-motion-split.md), the instantaneous noise velocity and its correlation are [distributions](../../../../distribution-mathematical-analysis.md); the delta contribution is not a finite ordinary velocity at $t=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
