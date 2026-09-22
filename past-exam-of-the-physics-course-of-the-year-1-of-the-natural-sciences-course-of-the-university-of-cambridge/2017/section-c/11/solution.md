<h1 id="section-c/11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Use the diagram's downward displacement $z$, measured from the unloaded plate position, and take $z(0)=0$. The [mechanical energy](../../../../mechanical-energy.md), with gravitational potential zero at that reference, is

$$
\boxed{E=\frac12m\dot z^2+\frac12kz^2-mgz.}
$$

The loaded equilibrium follows from $kz_{\mathrm{eq}}=mg$, so its downward shift is $\boxed{z_{\mathrm{eq}}=mg/k}$.

The shock absorber's [force](../../../../force-split.md) is $-b\dot z$, hence its power is [force](../../../../force-split.md) times [velocity](../../../../velocity.md): $dE/dt=-b\dot z^2\leq0$. Differentiating the [energy](../../../../energy-split.md) gives $\dot z(m\ddot z+kz-mg)=-b\dot z^2$, which yields, with continuity through instants of zero [velocity](../../../../velocity.md),

$$
\boxed{m\ddot z+b\dot z+kz=mg.}
$$

Set $\omega_0=\sqrt{k/m}$ and $\gamma=b/(2m)$.

For release from rest, the three [step response of a damped oscillator](../../../../step-response-of-a-damped-oscillator.md) regimes are easy to compare after shifting to $z-z_{\mathrm{eq}}$. With light damping $0<\gamma<\omega_0$, write $\omega_d=\sqrt{\omega_0^2-\gamma^2}$:

$$
\frac z{z_{\mathrm{eq}}}=1-e^{-\gamma t}\left(\cos\omega_dt+\frac\gamma{\omega_d}\sin\omega_dt\right).
$$

It overshoots and oscillates around the loaded position with a decaying envelope. At [critical damping](../../../../critical-damping.md), $\gamma=\omega_0$, it becomes $z/z_{\mathrm{eq}}=1-(1+\gamma t)e^{-\gamma t}$, approaching monotonically from below. For heavy damping $\gamma>\omega_0$, set $\eta=\sqrt{\gamma^2-\omega_0^2}$ and replace the trigonometric bracket by $\cosh\eta t+(\gamma/\eta)\sinh\eta t$. This is also monotonic, but its slow exponential delays settling.

<a id="section-c/11/image-damping-controls-the-scale-s-settling-while-initial-impact-velocity-can-still-cause-overshoot"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017-damped-scale.png)

**[Figure 3](#section-c/11/image-damping-controls-the-scale-s-settling-while-initial-impact-velocity-can-still-cause-overshoot). Damping controls the scale's settling, while initial impact velocity can still cause overshoot**.

[Critical damping](../../../../critical-damping.md) gives the fastest nonoscillatory settling from the unloaded rest condition, avoiding a repeatedly swinging reading without the sluggishness of [overdamping](../../../../overdamping.md). Its required coefficient is

$$
\boxed{b_{\mathrm{crit}}=2\sqrt{km}.}
$$

At [critical damping](../../../../critical-damping.md) the repeated characteristic root is $-\gamma$. Thus the general displacement under constant load is $(A+Bt)e^{-\gamma t}+C$. The equilibrium and initial conditions give $C=z_{\mathrm{eq}}$, $A=-z_{\mathrm{eq}}$ and $B-\gamma A=v_0$, hence

$$
\boxed{A=-\frac{mg}{k},\qquad B=v_0-\gamma\frac{mg}{k},\qquad C=\frac{mg}{k},\qquad \gamma=\sqrt{\frac km}.}
$$

Subtracting the final position gives $z-z_{\mathrm{eq}}=[-z_{\mathrm{eq}}+(v_0-\gamma z_{\mathrm{eq}})t]e^{-\gamma t}$. The exponential is positive and the bracket starts negative. It becomes positive at some $t>0$ if and only if its slope is positive. Therefore [critical-damping overshoot from initial velocity](../../../../critical-damping-overshoot-from-initial-velocity.md) requires

$$
\boxed{v_0>\gamma z_{\mathrm{eq}}=g\sqrt{\frac mk}=\frac g\gamma,}
$$

with $v_0$ positive downwards. At equality the scale still approaches from below. [Critical damping](../../../../critical-damping.md) prevents oscillatory modes, but does not guarantee a non-overshooting response to an arbitrarily large impact [velocity](../../../../velocity.md).

## ↑ Ancestors (12)

1. [11](../11.md)
2. [Section C](../../section-c.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
