<h1 id="section-b/8/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For [overdamping](../../../../../overdamping.md), $\gamma=b/(2m)>\omega$. Put $\alpha=\sqrt{\gamma^2-\omega^2}>0$. Both [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) $-\gamma\pm\alpha$ are negative real numbers. Replacing trigonometric functions by [hyperbolic functions](../../../../../hyperbolic-function.md) gives the exact trajectory

$$
\boxed{\mathbf r(t)=e^{-\gamma t}\left[\mathbf r_0\cosh\alpha t+\frac{\mathbf v_0+\gamma\mathbf r_0}{\alpha}\sinh\alpha t\right].}
$$

It starts from $(c,c)$ with tangent $(-\omega c,\omega c)$, bends anticlockwise toward the origin, and approaches it without repeated revolutions. The right panel gives a representative choice $\gamma=1.5\omega$; the paper does not specify one particular value of $b$ in this regime.

One can make the qualitative shape precise. In radial and tangential directions relative to the initial radius, the angle turned from the starting direction obeys

$$
\tan\Delta\phi(t)=\frac{\omega\sinh\alpha t}{\alpha\cosh\alpha t+\gamma\sinh\alpha t}\quad\Longrightarrow\quad\boxed{\Delta\phi(\infty)=\arctan\frac\omega{\gamma+\alpha}<\frac\pi4.}
$$

For $c>0$, both coordinates stay positive, and the approach is along the fixed ray with $y/x\to(\gamma+\alpha+\omega)/(\gamma+\alpha-\omega)$. The initial [velocity](../../../../../velocity.md) is tangential, so an immediately straight radial return would be incorrect. The absence of oscillatory [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) prevents repeated revolutions. This is a [non-spiralling overdamped central oscillator trajectory](../../../../../non-spiralling-overdamped-central-oscillator-trajectory.md).

## ↑ Ancestors (13)

1. [G](../g.md)
2. [8](../../8.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
