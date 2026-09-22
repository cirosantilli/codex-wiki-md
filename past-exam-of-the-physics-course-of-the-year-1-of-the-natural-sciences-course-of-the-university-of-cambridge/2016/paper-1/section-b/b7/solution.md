<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

The [moment of inertia](../../../../../moment-of-inertia.md) about a specified axis is $I=\int s^2\,dm$, where $s$ is perpendicular distance from the axis. The [parallel axis theorem](../../../../../parallel-axis-theorem.md) states $I=I_{\rm cm}+md^2$ for two parallel axes separated by $d$, one passing through the [centre of mass](../../../../../center-of-mass.md) of a body of [mass](../../../../../mass.md) $m$.

It is easiest to calculate the eccentric disc by subtraction. Let $m_f$ be the [mass](../../../../../mass.md) of the unperforated disc and $m_h$ the removed [mass](../../../../../mass.md). Uniform thickness and [density](../../../../../density.md) give $m_h=m_f/4$ and $m_f-m_h=M$, hence $m_f=4M/3$ and $m_h=M/3$. The hole is tangent to the rim, so its centre, and therefore the shaft axis, lies $R/2$ from the original disc centre. About the shaft axis,

$$
I_{\rm perforated}=\frac{4M}{3}\left(\frac{R^2}{2}+\frac{R^2}{4}\right)-\frac12\frac M3\left(\frac R2\right)^2=\frac{23}{24}MR^2.
$$

The shaft contributes $I_{\rm shaft}=M(R/2)^2/2=MR^2/8$. Thus

$$
\boxed{I=I_{\rm perforated}+I_{\rm shaft}=\frac{13}{12}MR^2.}
$$

The motor's [torque](../../../../../torque.md) is $P/\omega$ at nonzero [angular velocity](../../../../../angular-velocity.md), while the resisting [torque](../../../../../torque.md) is $-\gamma\omega$. The [rotational equation of motion](../../../../../rotational-equation-of-motion.md) and its equivalent [energy balance](../../../../../energy-balance.md) are

$$
I\dot\omega=\frac P\omega-\gamma\omega,\qquad \frac{d}{dt}\left(\frac12I\omega^2\right)=P-\gamma\omega^2.
$$

At the [steady state](../../../../../steady-state.md), input [power](../../../../../power.md) equals dissipated [power](../../../../../power.md), giving

$$
\boxed{\omega_0=\sqrt{P/\gamma}.}
$$

For the acceleration, use $u=\omega^2$. Then $\dot u+(2\gamma/I)u=2P/I$ with $u(0)=0$, so

$$
u(t)=\omega_0^2(1-e^{-2\gamma t/I}),\qquad \boxed{t=-\frac I{2\gamma}\ln\left(1-\frac{\omega^2}{\omega_0^2}\right),\quad0\leq\omega<\omega_0.}
$$

The approach to $\omega_0$ takes infinite time. This [constant-power rotational acceleration](../../../../../constant-power-rotational-acceleration.md) idealizes the start: $P/\omega$ diverges at rest, although the [energy balance](../../../../../energy-balance.md) has a well-defined limiting solution. A real motor has finite starting [torque](../../../../../torque.md).

## ↑ Ancestors (13)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
