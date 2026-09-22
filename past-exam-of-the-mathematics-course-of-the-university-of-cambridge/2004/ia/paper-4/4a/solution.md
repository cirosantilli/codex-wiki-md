<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Let $z$ measure height above the release point, and use $\mathcal V=4\pi a^3/3$ for the bubble volume to avoid confusing it with a [speed](../../../../../speed.md). For constant radius, [Newton's second law](../../../../../newton-s-second-law.md), the specified [buoyancy](../../../../../buoyancy.md) and the given [Stokes law](../../../../../stokes-s-law.md) give

$$
\alpha\rho\mathcal V\dot u=\rho g\mathcal V-6\pi\mu au.
$$

With positive $\alpha,\rho,\mu,a$, define

$$
\tau=\frac{\alpha\rho\mathcal V}{6\pi\mu a}
=\frac{2\alpha\rho a^2}{9\mu},\qquad
U=\frac{\rho g\mathcal V}{6\pi\mu a}
=\frac{2\rho g a^2}{9\mu}.
$$

The [differential equation](../../../../../differential-equation-split.md) becomes $\dot u+(u/\tau)=U/\tau$. Its solution with $u(0)=0$ is $u(t)=U(1-e^{-t/\tau})$. Integration using $z(0)=0$ yields

$$
\boxed{z(t)=U\left[t-\tau\left(1-e^{-t/\tau}\right)\right],\qquad
\lim_{t\to\infty}u(t)=U=\frac{2\rho g a^2}{9\mu}.}
$$

An arbitrary initial height is added to this expression. The effective inertia changes the relaxation time $\tau$, but not the [terminal velocity](../../../../../terminal-velocity.md) obtained by balancing [buoyancy](../../../../../buoyancy.md) and drag.

For the dissolving bubble assume $\beta>0$ and use the specified instantaneous [terminal velocity](../../../../../terminal-velocity.md), rather than the constant-radius transient formula. The bubble disappears at $t_*=a_0^2/\beta$, and

$$
z(t)=\frac{2\rho g}{9\mu}\int_0^t(a_0^2-\beta s)\,ds
=\frac{2\rho g}{9\mu}\left(a_0^2t-\frac{\beta t^2}{2}\right),\qquad0\leq t\leq t_*.
$$

Its total rise is therefore $\boxed{z(t_*)=\rho g a_0^4/(9\mu\beta)}$. This second model neglects the initial [acceleration](../../../../../acceleration.md) and uses exactly the terminal-speed approximation stipulated for the shrinking bubble.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
