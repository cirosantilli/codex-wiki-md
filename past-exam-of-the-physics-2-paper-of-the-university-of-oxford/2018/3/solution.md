<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [continuity equation for electric charge](../../../charge-continuity-equation.md) is $\nabla\cdot J=-\partial_t\rho$. Taking the [divergence](../../../divergence.md) of the magnetostatic [Ampère's law](../../../ampere-s-circuital-law.md) would instead require $\nabla\cdot J=0$. The [displacement current](../../../displacement-current.md) repairs this conflict: using [Gauss's law](../../../gauss-s-law.md), $\nabla\cdot(\epsilon_0\partial_tE)=\partial_t\rho$, so the [Ampère-Maxwell equation](../../../ampere-s-circuital-law.md) is

$$
\nabla\times B=\mu_0(J+\epsilon_0\partial_tE).
$$

In the [parallel-plate capacitor](../../../parallel-plate-capacitor.md), neglect [fringing fields](../../../fringing-field.md) and take $E_z=V_0e^{-i\omega t}/d$. A circular [Ampère loop](../../../amperian-loop.md) of radius $s<a$ encloses [displacement current](../../../displacement-current.md) $-i\omega\epsilon_0\pi s^2V_0e^{-i\omega t}/d$. Therefore the [magnetic field between circular capacitor plates](../../../magnetic-field-between-circular-capacitor-plates.md) has phasor and amplitude

$$
\widetilde B_\phi(s)=-\frac{i\omega\mu_0\epsilon_0V_0s}{2d},\qquad
\boxed{B_{\mathrm{amp}}(s)=\frac{\omega\mu_0\epsilon_0|V_0|}{2d}\,s,\quad0\leq s<a.}
$$

It is zero on the axis, grows linearly with radius, and is azimuthal by the [right-hand rule](../../../right-hand-rule.md). This is a [quasistatic approximation](../../../quasistatic-approximation-electromagnetism.md): in addition to $d\ll a$, the uniform-field model requires $\omega a/c\ll1$ and excludes the edge region. The answer gives the oscillation amplitude, rather than a time-independent instantaneous magnitude.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2018](../../2018-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
