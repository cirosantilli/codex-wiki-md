# Critical-damping overshoot from initial velocity

↑ **Parent:** [Critical damping](critical-damping.md)

A mass-spring-damper subject to a constant load obeys $\ddot z+2\gamma\dot z+\gamma^2z=\gamma^2z_{\mathrm{eq}}$ at [critical damping](critical-damping.md). With $z(0)=0$ and $\dot z(0)=v_0$,

$$
z(t)=z_{\mathrm{eq}}+[-z_{\mathrm{eq}}+(v_0-\gamma z_{\mathrm{eq}})t]e^{-\gamma t}.
$$

For $z_{\mathrm{eq}}>0$, the displacement exceeds its final value at a positive time exactly when $v_0>\gamma z_{\mathrm{eq}}$. Thus a critically damped step response released from rest is non-overshooting, but critical damping alone does not forbid overshoot from arbitrary initial momentum. For a vertical scale with downward coordinate, $z_{\mathrm{eq}}=mg/k$ and $\gamma=\sqrt{k/m}$, making the threshold $v_0>g\sqrt{m/k}$.

## ↑ Ancestors (8)

1. [Critical damping](critical-damping.md)
2. [Damping](damping.md)
3. [Wave equation](wave-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-c/11/solution.md)
