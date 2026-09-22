# Weak surface-shear perturbation of stagnation flow

↑ **Parent:** [Stress-driven stagnation-point boundary layer](stress-driven-stagnation-point-boundary-layer.md)

For the [stress-driven stagnation-point boundary layer](stress-driven-stagnation-point-boundary-layer.md) on $\zeta<0$, a [regular perturbation](regular-perturbation.md) $f=\zeta+\gamma f_1+O(\gamma^2)$ gives $g=f_1'$ satisfying $g''+\zeta g'-2g=0$, $g'(0)=1$ and $g(-\infty)=0$. [Reduction of order](reduction-of-order.md) with the known solution $1+\zeta^2$ gives

$$
g(\zeta)=(1+\zeta^2)\int_{-\infty}^{\zeta}
\frac{e^{-s^2/2}}{(1+s^2)^2}\,ds.
$$

Indeed, writing $g=(1+\zeta^2)v$ gives $v'=C e^{-\zeta^2/2}/(1+\zeta^2)^2$; decay at $-\infty$ fixes the lower endpoint and $g'(0)=1$ fixes $C=1$. The [integral](integral-split.md) at zero is $\sqrt{2\pi}/4=\sqrt{\pi/8}$, as follows by differentiating the antiderivative

$$
\frac14\left[\frac{2s}{1+s^2}e^{-s^2/2}
+\sqrt{2\pi}\operatorname{erf}(s/\sqrt2)\right].
$$

Here $\operatorname{erf}$ is the [error function](error-function.md). Thus positive imposed outward [shear stress](shear-stress.md) increases the outward surface [velocity](velocity.md) by the displayed first-order factor. Replacing decay at $-\infty$ by decay at $+\infty$ while leaving the equation and wall [derivative](derivative.md) unchanged reverses this coefficient and describes a different problem.

## ↑ Ancestors (7)

1. [Stress-driven stagnation-point boundary layer](stress-driven-stagnation-point-boundary-layer.md)
2. [Boundary-layer equation](boundary-layer-equation.md)
3. [Boundary layer](boundary-layer.md)
4. [Continuum mechanics](continuum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-viscous-flow-course-of-the-university-of-oxford/2023/2/c/ii/solution.md)
