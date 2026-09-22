<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Put $\omega_0=\sqrt{k/m}$ and $\gamma=b/(2m)$. The characteristic roots are $-\gamma\pm\sqrt{\gamma^2-\omega_0^2}$. For release from rest at [displacement](../../../../../displacement.md) $x_0>0$, the three regimes are

$$
x(t)=
\begin{cases}
x_0e^{-\gamma t}\left[\cos(\omega_dt)+\dfrac{\gamma}{\omega_d}\sin(\omega_dt)\right],
&0<\gamma<\omega_0,\quad \omega_d=\sqrt{\omega_0^2-\gamma^2},\\
x_0(1+\omega_0t)e^{-\omega_0t},
&\gamma=\omega_0,\\
x_0e^{-\gamma t}\left[\cosh(st)+\dfrac{\gamma}{s}\sinh(st)\right],
&\gamma>\omega_0,\quad s=\sqrt{\gamma^2-\omega_0^2}.
\end{cases}
$$

[underdamping](../../../../../underdamping.md) produces decaying oscillations; [critical damping](../../../../../critical-damping.md) is the repeated-root boundary; [overdamping](../../../../../overdamping.md) has two real decay rates. The critical and overdamped curves from rest approach equilibrium without crossing it. All three initially have zero slope and negative [acceleration](../../../../../acceleration.md). A sufficiently strong initial kick can cause a single crossing even without an oscillatory mode.

For the critical oscillator with initial [velocity](../../../../../velocity.md) $-v_0$, the repeated-root solution is

$$
x(t)=\left[x_0+(\omega_0x_0-v_0)t\right]e^{-\omega_0t}.
$$

Its exponential is positive at finite time. Therefore the bracket has a positive-time zero precisely when

$$
\boxed{v_0>\omega_0x_0,\qquad
t_{\rm cross}=\frac{x_0}{v_0-\omega_0x_0}.}
$$

Equality gives a pure positive exponential and no finite-time crossing.

For the specified numerical oscillator, $\omega_0=1\ {\rm s^{-1}}$ and $\gamma=2/\sqrt3\ {\rm s^{-1}}>1\ {\rm s^{-1}}$, verifying [overdamping](../../../../../overdamping.md). Its two roots are $-1/\sqrt3$ and $-\sqrt3$ in inverse seconds. The initial conditions give

$$
\boxed{x(t)=
(0.015-0.015\sqrt3)e^{-t/\sqrt3}
+(0.015\sqrt3-0.005)e^{-\sqrt3t}\quad{\rm m},}
$$

with $t$ in seconds. The slow component has a negative coefficient; the fast positive component initially dominates.

The values for the requested plot are

$$
\begin{array}{c|rrrrrrr}
t\ ({\rm s})&0&0.5&1.0&1.5&2.0&2.5&3.0\\
x\ ({\rm mm})&10.000&0.598&-2.452&-3.057&-2.804&-2.317&-1.827
\end{array}
$$

The curve crosses near $0.56\ {\rm s}$ and then returns toward zero from below. The exact expression provides a check on the graphical estimate:

$$
\boxed{t_{\rm cross}=\frac{\sqrt3}{2}
\ln\!\left(\frac{0.015\sqrt3-0.005}{0.015\sqrt3-0.015}\right)
\simeq0.561\ {\rm s}.}
$$

<a id="section-b/b6/image-original-damped-oscillator-solutions-and-clamped-sheet-waveguide-calculations"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2-damping-and-guidance.png)

**[Figure 2](#section-b/b6/image-original-damped-oscillator-solutions-and-clamped-sheet-waveguide-calculations). Original damped-oscillator solutions and clamped-sheet waveguide calculations**. Rest-release curves compare three [damping](../../../../../damping.md) regimes; the separate kicked overdamped trajectory includes the requested sampling times. The guided-mode panel plots the dispersion branches, and the profile panel compares the two-mode input with its first phase-reversed transverse profile.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
