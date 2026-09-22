# Potential-source and wake decomposition of sphere Oseen flow

↑ **Parent:** [Oseen approximation](oseen-approximation.md)

Let $U=|\mathbf U|$, $\nu=\mu/\rho$, and $r=|\mathbf x|$. A decaying outer disturbance matched to the leading [translating sphere in Stokes flow](translating-sphere-in-stokes-flow.md) is

$$
\phi=-\frac{3a\nu}{2r},\qquad\chi=\frac{3a}{2r}\exp\left[\frac{\mathbf U\cdot\mathbf x-Ur}{2\nu}\right],\qquad\mathbf u=\nabla\phi+\nu\nabla\chi-\mathbf U\chi.
$$

Here $\Delta\phi=0$ and $(\nu\Delta-\mathbf U\cdot\nabla)\chi=0$ away from zero. The substitution $\chi=h e^{\mathbf U\cdot\mathbf x/(2\nu)}$ reduces the latter equation to $(\Delta-U^2/(4\nu^2))h=0$, whose decaying radial solution is proportional to $e^{-Ur/(2\nu)}/r$. In the inner overlap, cancellation of the potential monopole gives $\mathbf u\sim-3a[\mathbf U+\mathbf n(\mathbf U\cdot\mathbf n)]/(4r)$. The potential source's [volume flux](volumetric-flow-rate.md) is $6\pi\nu a$, and its [mass flux](mass-flux.md) is $6\pi\mu a$. Downstream, the [fluid wake](wake-physics.md) width grows as $\sqrt{\nu x/U}$; its mass deficit balances this source, while its [momentum](momentum.md) deficit is $6\pi\mu aU$, the [Stokes drag law](stokes-s-law.md).

## ↑ Ancestors (7)

1. [Oseen approximation](oseen-approximation.md)
2. [Stokes flow](stokes-flow-split.md)
3. [Viscous fluid flow](viscous-fluid-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-86/3/solution.md)
