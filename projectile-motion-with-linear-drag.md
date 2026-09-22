# Projectile motion with linear drag

↑ **Parent:** [Linear drag](linear-drag.md)

For constant [acceleration](acceleration.md) vector $\mathbf g$ and $\gamma>0$, a projectile initially at $\mathbf r_0$ with [velocity](velocity.md) $\mathbf v_0$ has

$$
\mathbf v(t)=\frac{\mathbf g}{\gamma}+\left(\mathbf v_0-\frac{\mathbf g}{\gamma}\right)e^{-\gamma t},\qquad
\mathbf r(t)=\mathbf r_0+\frac{\mathbf g}{\gamma}t+
\frac{\mathbf v_0-\mathbf g/\gamma}{\gamma}(1-e^{-\gamma t}).
$$

The [integrating factor](integrating-factor.md) $e^{\gamma t}$ solves the first-order [linear ordinary differential equation](linear-ordinary-differential-equation-split.md) for the [velocity](velocity.md); one more integration proves the position formula. The terminal [velocity](velocity.md) is $\mathbf g/\gamma$, and $1/\gamma$ is the relaxation [time](time-in-physics.md). For $\mathbf g=(0,-g)$ and $\mathbf r_0=0$, eliminating time when $V_{0x}\ne0$ gives

$$
z(x)=\left(\frac{V_{0z}}{V_{0x}}+\frac{g}{\gamma V_{0x}}\right)x
+\frac{g}{\gamma^2}\ln\left(1-\frac{\gamma x}{V_{0x}}\right).
$$

For finite $t\geq0$, the physical domain is $0\leq\gamma x/V_{0x}<1$. If $V_{0x}=0$, the path is vertical and cannot generally be represented as a single-valued graph $z(x)$. Expanding at fixed $x$ as $\gamma\to0$ recovers $z=(V_{0z}/V_{0x})x-gx^2/(2V_{0x}^2)$.

## ↑ Ancestors (6)

1. [Linear drag](linear-drag.md)
2. [Drag (physics)](drag-physics.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/15/a/solution.md)
