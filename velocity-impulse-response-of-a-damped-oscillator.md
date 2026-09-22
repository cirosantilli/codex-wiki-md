# Velocity-impulse response of a damped oscillator

↑ **Parent:** [Damped harmonic oscillator](damped-harmonic-oscillator.md)

For $\ddot x+2\gamma\dot x+\omega_0^2x=0$, an initial [velocity](velocity.md) $v_0$ at zero displacement gives

$$
x(t)=\begin{cases}
(v_0/\omega_d)e^{-\gamma t}\sin(\omega_dt),&\gamma<\omega_0,\quad\omega_d=\sqrt{\omega_0^2-\gamma^2},\\
v_0t e^{-\omega_0t},&\gamma=\omega_0,\\
(v_0/s)e^{-\gamma t}\sinh(st),&\gamma>\omega_0,\quad s=\sqrt{\gamma^2-\omega_0^2}.
\end{cases}
$$

All three cases begin with slope $v_0$. Only [underdamping](underdamping.md) produces repeated crossings through equilibrium; [critical damping](critical-damping.md) and [overdamping](overdamping.md) remain on the initial side of equilibrium for this particular initial condition. The overdamped long-time tail decays at rate $\gamma-s$, which becomes slow for strong [damping](damping.md).

## ↑ Ancestors (5)

1. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-b/b7/c/solution.md)
