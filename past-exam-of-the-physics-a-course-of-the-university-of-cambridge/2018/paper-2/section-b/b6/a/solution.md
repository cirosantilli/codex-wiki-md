<h1 id="section-b/b6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substituting $x=Ae^{pt}$ into the [damped harmonic oscillator](../../../../../../damped-harmonic-oscillator.md) equation gives

$$
p^2+\gamma p+\omega_0^2=0,\qquad p_\pm=-\frac\gamma2\pm\sqrt{\frac{\gamma^2}{4}-\omega_0^2}.
$$

For nonnegative [viscous damping](../../../../../../viscous-damping.md), the cases are

$$
\boxed{\begin{aligned}
\gamma>2\omega_0 &: \quad x=C_+e^{p_+t}+C_-e^{p_-t} &&\text{overdamping},\\
\gamma=2\omega_0 &: \quad x=(C_1+C_2t)e^{-\omega_0t} &&\text{critical damping},\\
0\leq\gamma<2\omega_0 &: \quad x=e^{-\gamma t/2}[C_1\cos\omega_dt+C_2\sin\omega_dt] &&\text{underdamping},
\end{aligned}}\qquad \omega_d=\sqrt{\omega_0^2-\gamma^2/4}.
$$

The PDF's request to express these conditions in terms of $\gamma/m$ is dimensionally inconsistent with its definition $\gamma=b/m$: $\gamma$ already has units $\mathrm{s^{-1}}$. With the unnormalised equation $m\ddot x+b\dot x+kx=0$, the equivalent comparisons are $b/m\gtrless2\omega_0$, or $b^2\gtrless4mk$. Also $\omega_0$ is the undamped natural [angular frequency](../../../../../../angular-frequency.md), not in general the driven displacement peak.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
