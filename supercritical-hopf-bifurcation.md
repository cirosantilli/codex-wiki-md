# Supercritical Hopf bifurcation

↑ **Parent:** [Hopf bifurcation](hopf-bifurcation.md)

In a supercritical [Hopf bifurcation](hopf-bifurcation.md), a small [periodic orbit](periodic-orbit.md) attracts within the critical [centre manifold](center-manifold.md) on the side where the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) repels within that manifold. Orient the parameter so that its critical [eigenvalue](eigenvalue.md) [real part](real-part.md) increases through zero. For the exact [Hopf normal form](hopf-normal-form.md) $\dot z=(\mu+i\omega)z-|z|^2z$, with $\omega>0$, the nonzero constant radius solves

$$
0=\mu r-r^3,\qquad r_*=\sqrt\mu\quad(\mu>0).
$$

For $0<r<r_*$ the radius grows; for $r>r_*$ it shrinks. A radial disturbance $\delta r$ therefore has leading equation $\dot{\delta r}=-2\mu\,\delta r$, since $\partial_r(\mu r-r^3)|_{r_*}=-2\mu<0$. This is [orbital stability](orbital-stability.md): nearby [orbits](orbit-dynamical-system.md) approach the circle, but their [phase](phase-waves.md) need not match a chosen representative. The exact [angular frequency](angular-frequency.md) is $\omega$, so the period is $2\pi/\omega$ and the [frequency](frequency.md) is $\omega/(2\pi)$.

The [Jacobian matrix](jacobian-matrix.md) at zero is $\begin{pmatrix}\mu&-\omega\\\omega&\mu\end{pmatrix}$, with [eigenvalues](eigenvalue.md) $\mu\pm i\omega$. Zero attracts for $\mu<0$ and repels for $\mu>0$. Exactly at $\mu=0$, $\dot r=-r^3$ gives

$$
r(t)=\frac{r_0}{\sqrt{1+2r_0^2t}},\qquad t\geq0.
$$

Thus zero still has [asymptotic stability](asymptotic-stability.md) in this model, with algebraic decay, and there is no nonzero [limit cycle](limit-cycle.md) at the threshold itself. As $\mu\downarrow0$ on the cycle branch, both its radius $\sqrt\mu$ and its radial attraction rate $2\mu$ vanish. Small cycles consequently become slow to settle in radius even though their [angular frequency](angular-frequency.md) stays fixed.

// Target: dynamical-systems.bigb

## ↑ Ancestors (6)

1. [Hopf bifurcation](hopf-bifurcation.md)
2. [Bifurcation theory](bifurcation-theory.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Hopf bifurcation](hopf-bifurcation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-58/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-60/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-85/1/b/solution.md)
- [Subcritical Hopf bifurcation](subcritical-hopf-bifurcation.md)
- [Three-neuron ring stability](three-neuron-ring-stability.md)
