<h1 id="section-b/b7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set the drive to zero and try $x=e^{st}$. The [characteristic equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
ms^2+bs+k=0,\qquad s_\pm=-\gamma\pm\sqrt{\gamma^2-\omega_0^2},
\quad\gamma=\frac b{2m},\quad\omega_0^2=\frac km.
$$

For [underdamping](../../../../../../underdamping.md), $\boxed{b^2<4mk}$, the roots are $-\gamma\pm i\omega_d$, with $\omega_d=\sqrt{\omega_0^2-\gamma^2}$. The displacement oscillates with an exponentially decaying envelope:

$$
x=e^{-\gamma t}[C\cos(\omega_dt)+D\sin(\omega_dt)].
$$

For [critical damping](../../../../../../critical-damping.md), $\boxed{b^2=4mk}$, there is a repeated root $-\omega_0$, giving $x=(C+Dt)e^{-\omega_0t}$. The motion is nonoscillatory and is the limiting case between oscillatory and overdamped response.

For [overdamping](../../../../../../overdamping.md), $\boxed{b^2>4mk}$, the roots are distinct negative real numbers and $x=C e^{s_+t}+D e^{s_-t}$. Both components decay without sustained oscillation; strong damping gives a particularly slow late-time relaxation. Constants $C,D$ depend on the initial conditions. A nonoscillatory solution can cross equilibrium once for some initial data, so “nonoscillatory” does not mean monotone for every possible initial condition.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
