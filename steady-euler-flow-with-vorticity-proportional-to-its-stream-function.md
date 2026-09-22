# Steady Euler flow with vorticity proportional to its stream function

↑ **Parent:** [Stream function](stream-function.md)

For a smooth planar [incompressible flow](incompressible-flow.md), use $u=\psi_y$, $v=-\psi_x$, so its scalar [vorticity](vorticity-split.md) is $\omega=-\Delta\psi$. If $\omega=\lambda\psi$ for a constant $\lambda$, the flow solves the steady constant-density [Euler equations](euler-equations-for-an-inviscid-fluid-split.md) with a suitable pressure.

Indeed the vector identity for the convective acceleration gives

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)+\omega\nabla\psi.
$$

Therefore the pressure can be chosen so that the [Bernoulli function](bernoulli-function.md) satisfies $p/\rho+|\mathbf u|^2/2=C-\lambda\psi^2/2$. Its gradient is $-\omega\nabla\psi$, exactly the steady momentum equation. It is constant along each [streamline](streamline.md), since the stream function is constant there.

For example $\psi=\sin x\cos y$ satisfies $\omega=2\psi$. Its pressure is $p_0-\rho\sin^2x/2+\rho\sin^2y/2$. Thus a rotational flow can have an explicit pressure and a streamline-dependent Bernoulli constant.

## ↑ Ancestors (5)

1. [Stream function](stream-function.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2008/k/k1/iv/solution.md)
