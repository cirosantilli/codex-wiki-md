# Initially circular damped planar oscillator

↑ **Parent:** [Damped harmonic oscillator](damped-harmonic-oscillator.md)

For an isotropic [harmonic oscillator](simple-harmonic-motion.md) with [mass](mass.md) $m$, restoring constant $k$ and [linear drag](linear-drag.md) coefficient $b$, put $\omega=\sqrt{k/m}$ and $\gamma=b/(2m)$. Choose initial [position](position.md) $\mathbf r_0=(c,c)$ and tangential [velocity](velocity.md) $\mathbf v_0=\omega(-c,c)$, which would give anticlockwise [circular motion](circular-motion.md) without [damping](damping.md). For [underdamping](underdamping.md), $\nu=\sqrt{\omega^2-\gamma^2}$ gives

$$
\mathbf r(t)=e^{-\gamma t}\left[\mathbf r_0\cos\nu t+\frac{\mathbf v_0+\gamma\mathbf r_0}{\nu}\sin\nu t\right].
$$

Taking the squared norm and multiplying by $k/2$ gives the exact [potential energy](potential-energy.md)

$$
U(t)=kc^2e^{-2\gamma t}\left[1+\frac\gamma\nu\sin2\nu t+\frac{2\gamma^2}{\nu^2}\sin^2\nu t\right].
$$

Only to leading order in $\gamma/\omega\ll1$ does this reduce to $kc^2e^{-2\gamma t}$. The exact expression has $\dot U(0)=0$, consistent with the initially tangential [velocity](velocity.md), while the leading approximation does not reproduce this short-time derivative. Angular momentum obeys $L_z(t)=L_z(0)e^{-2\gamma t}$ by [angular momentum decay under uniform linear drag](angular-momentum-decay-under-uniform-linear-drag.md).

**Table of contents**

- [Non-spiralling overdamped central oscillator trajectory](non-spiralling-overdamped-central-oscillator-trajectory.md)

## ↑ Ancestors (5)

1. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Non-spiralling overdamped central oscillator trajectory](non-spiralling-overdamped-central-oscillator-trajectory.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/8/e/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/8/f/solution.md)
