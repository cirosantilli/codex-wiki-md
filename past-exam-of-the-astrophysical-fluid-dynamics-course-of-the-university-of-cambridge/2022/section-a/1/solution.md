<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A fluid particle follows a [Lagrangian trajectory](../../../../lagrangian-trajectory.md), so its position satisfies $\dot x=u(x,t)$ rather than the [velocity](../../../../velocity.md) evaluated permanently at its initial position. Assume $\omega\ne0$, and write

$$
x(t)=X_0+u_0a(t)+u_0^2b(t)+O(u_0^3),\qquad a(0)=b(0)=0.
$$

Set $\alpha=kX_0$ and $\theta=\alpha-\omega t$. A [Taylor expansion](../../../../taylor-expansion.md) of the [velocity](../../../../velocity.md) about $X_0$ gives

$$
u_0\dot a+u_0^2\dot b=u_0\sin\theta+ku_0^2a\cos\theta+O(u_0^3).
$$

Thus $\dot a=\sin\theta$, and

$$
a(t)=\frac{\cos\theta-\cos\alpha}{\omega}.
$$

At the next order,

$$
\dot b=\frac k\omega(\cos^2\theta-\cos\alpha\cos\theta),
$$

so the required [second-order trajectory in a sinusoidal velocity field](../../../../second-order-trajectory-in-a-sinusoidal-velocity-field.md) is

$$
\boxed{\begin{aligned}
x(t)={}&X_0+\frac{u_0}{\omega}(\cos\theta-\cos\alpha)\\
&+\frac{ku_0^2}{\omega}\left[\frac t2+
\frac{\sin2\alpha-\sin2\theta}{4\omega}
-\frac{\cos\alpha(\sin\alpha-\sin\theta)}{\omega}\right]+O(u_0^3).
\end{aligned}}
$$

Both corrections vanish at $t=0$. All retained terms have units of length. The secular contribution gives the [Stokes drift](../../../../stokes-drift.md)

$$
\boxed{\overline{\dot x}=\frac{ku_0^2}{2\omega}+O(u_0^3),}
$$

although the [Eulerian time average](../../../../eulerian-time-average.md) of the given [velocity](../../../../velocity.md) is zero. The particle samples the [wave](../../../../wave-split.md) at its displaced position, producing this second-order drift. The expansion is in the dimensionless parameter $|ku_0/\omega|\ll1$, for fixed times; it ceases to be uniform when the accumulated drift changes the [wave](../../../../wave-split.md) phase by order unity.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
