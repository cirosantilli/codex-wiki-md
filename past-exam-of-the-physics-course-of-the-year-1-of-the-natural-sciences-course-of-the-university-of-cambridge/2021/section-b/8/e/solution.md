<h1 id="section-b/8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $\gamma=b/(2m)$ and $\nu=\sqrt{\omega^2-\gamma^2}$, where $\omega=\sqrt{k/m}$ is the undamped [angular frequency](../../../../../angular-frequency.md). The [linear drag](../../../../../linear-drag.md) gives the vector [damped harmonic oscillator](../../../../../damped-harmonic-oscillator.md) equation

$$
\ddot{\mathbf r}+2\gamma\dot{\mathbf r}+\omega^2\mathbf r=0.
$$

For the original circular [initial conditions](../../../../../initial-condition.md), $\mathbf r_0=(c,c)$ and $\mathbf v_0=\omega(-c,c)$, the exact [underdamped](../../../../../underdamping.md) solution is

$$
\mathbf r(t)=e^{-\gamma t}\left[\mathbf r_0\cos\nu t+\frac{\mathbf v_0+\gamma\mathbf r_0}{\nu}\sin\nu t\right].
$$

Using $|\mathbf r_0|^2=2c^2$, $|\mathbf v_0|^2=2\omega^2c^2$ and $\mathbf r_0\cdot\mathbf v_0=0$ gives

$$
\boxed{U(t)=kc^2e^{-2\gamma t}\left[1+\frac\gamma\nu\sin2\nu t+\frac{2\gamma^2}{\nu^2}\sin^2\nu t\right].}
$$

This exact [potential energy](../../../../../potential-energy.md) is useful because it satisfies the prescribed [initial conditions](../../../../../initial-condition.md), including $\dot U(0)=k\mathbf r_0\cdot\mathbf v_0=0$. In the stated weak-[damping](../../../../../damping.md) limit $\gamma\ll\omega$, $\nu\simeq\omega$ and the square bracket differs from one by a small oscillatory term. The leading approximation is therefore

$$
\boxed{U(t)\simeq kc^2e^{-bt/m}.}
$$

The radius is approximately $\sqrt2\,c\,e^{-bt/(2m)}$, so the trajectory is approximately a shrinking [logarithmic spiral](../../../../../logarithmic-spiral.md). The exactly exponential result would require slightly adjusted initial [velocity](../../../../../velocity.md); with the specified undamped circular [velocity](../../../../../velocity.md), the small modulation above is real. This is the [initially circular damped planar oscillator](../../../../../initially-circular-damped-planar-oscillator.md).

## ↑ Ancestors (13)

1. [E](../e.md)
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
