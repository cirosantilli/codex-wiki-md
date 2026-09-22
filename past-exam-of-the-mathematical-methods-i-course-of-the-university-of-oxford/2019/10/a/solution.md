<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a physical [mass](../../../../mass.md) $m>0$, [spring constant](../../../../spring-constant.md) $k>0$, and nonnegative viscous damping parameter $\gamma$. The homogeneous [damped harmonic oscillator](../../../../damped-harmonic-oscillator.md) has [characteristic equation](../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md)

$$
r^2+\gamma r+\omega_0^2=0,\qquad\omega_0^2=\frac{k}{m}.
$$

Its roots are $r=-\gamma/2\pm\sqrt{\gamma^2/4-\omega_0^2}$. They have nonzero imaginary parts precisely when $\gamma^2<4k/m$. Defining $\Omega=\sqrt{k/m-\gamma^2/4}$, the real oscillatory solutions are

$$
\boxed{z_h(t)=e^{-\gamma t/2}\big(C\cos\Omega t+D\sin\Omega t\big),\qquad\gamma^2<\frac{4k}{m}.}
$$

For strictly decaying oscillations also require $\gamma>0$. The limiting $\gamma=0$ case is an undamped [harmonic oscillator](../../../../simple-harmonic-motion.md). Equality gives critical damping with $z_h=(C+Dt)e^{-\gamma t/2}$, and a larger positive $\gamma$ gives two real decaying exponentials rather than oscillations.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
