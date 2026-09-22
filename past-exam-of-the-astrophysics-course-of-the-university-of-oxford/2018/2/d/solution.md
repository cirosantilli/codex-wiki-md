<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

When $k^{(p)}\gg k_J^{(p)}$, omit the gravitational term and define $\omega(t)=c_s(t)k/a(t)$. Then

$$
\boxed{\ddot\delta_{\mathbf k}+2H\dot\delta_{\mathbf k}+\omega^2\delta_{\mathbf k}=0.}
$$

This is an acoustic [damped harmonic oscillator](../../../../damped-harmonic-oscillator.md) with time-dependent coefficients. Freezing the background locally at $t_0$, its amplitude damping rate is $H_0$, so

$$
\boxed{\tau_{\mathrm{amp}}=H_0^{-1},\qquad
T_{\mathrm{osc}}=\frac{2\pi}{\sqrt{\omega_0^2-H_0^2}}
\simeq\frac{2\pi a_0}{c_{s0}k}\quad(\omega_0\gg H_0).}
$$

The oscillation-averaged quadratic oscillator [energy](../../../../energy-split.md) decays twice as fast in this frozen-frequency model, with time $1/(2H_0)$. Stating which quantity is damped avoids a factor-of-two convention error. Locally the solution is

$$
\delta_{\mathbf k}\simeq e^{-H_0(t-t_0)}
\left[C\cos\bigl(\omega_d(t-t_0)\bigr)+D\sin\bigl(\omega_d(t-t_0)\bigr)\right],
\quad\omega_d=\sqrt{\omega_0^2-H_0^2}.
$$

For evolution over many expansion times, retain the varying frequency. Put $\delta_{\mathbf k}=\chi/a$. Direct substitution gives

$$
\ddot\chi+\left(\omega^2-\frac{\ddot a}{a}\right)\chi=0.
$$

When $\omega\gg H$ and $|\dot\omega|\ll\omega^2$, the [WKB approximation](../../../../wkb-approximation.md) yields

$$
\boxed{\delta_{\mathbf k}(t)\simeq
\frac{1}{a(t)\sqrt{\omega(t)}}
\left[C\cos\!\left(\int^t\omega(s)\,ds\right)+
D\sin\!\left(\int^t\omega(s)\,ds\right)\right].}
$$

These are rapidly oscillating [sound waves](../../../../acoustic-wave.md) in comoving [density](../../../../density.md), diluted by the expanding background. For constant $c_s$ their envelope scales as $a^{-1/2}$, not universally as $a^{-1}$, because $\omega\propto a^{-1}$. In the [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md), introducing [conformal time](../../../../conformal-time.md) $d\eta=dt/a$ gives the exact constant-$c_s$ pressure-only solution $\delta_{\mathbf k}=[C\sin(kc_s\eta)+D\cos(kc_s\eta)]/\eta$, consistent with $a\propto\eta^2$. For that background the frozen-coefficient damping time is $3t/2$, while the slowly varying envelope has instantaneous decay time $2/H$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
