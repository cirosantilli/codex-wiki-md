<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a genuinely second-order [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md), assume $a_2\ne0$. Substituting the [exponential function](../../../../exponential-function.md) $f=e^{rt}$ into the [homogeneous linear differential equation](../../../../homogeneous-linear-differential-equation.md) gives $a_2r^2+a_1r+a_0=0$. Oscillations arise precisely when its two [roots of a polynomial](../../../../root-of-a-polynomial.md) have nonzero [imaginary parts](../../../../imaginary-part.md), namely

$$
\boxed{a_1^2-4a_0a_2<0.}
$$

In that case, writing $\omega=\sqrt{4a_0a_2-a_1^2}/(2|a_2|)>0$, the real [complementary function](../../../../homogeneous-solution.md) is

$$
f(t)=e^{-a_1t/(2a_2)}\bigl(C_1\cos\omega t+C_2\sin\omega t\bigr).
$$

Every nonzero such solution has an oscillatory factor; the oscillation may decay, grow, or keep constant amplitude according to the sign of $a_1/a_2$. This is the [oscillatory-root criterion for a real second-order equation](../../../../oscillatory-root-criterion-for-a-real-second-order-equation.md); decay is not a prerequisite for oscillation.

For completeness, if $a_2=0$ and $a_1\ne0$, only real [exponential functions](../../../../exponential-function.md) occur. If $a_2=a_1=0$ and $a_0\ne0$, only $f=0$ is allowed. If all three coefficients vanish, every twice-differentiable function is allowed, including oscillatory ones; the second-order criterion does not apply to this degenerate identity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
