<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

Measure $x$ from the static equilibrium position, so the constant gravitational [force](../../../../../force-split.md) has already cancelled the equilibrium [spring](../../../../../spring.md) [force](../../../../../force-split.md). With stationary oil, [Newton's second law](../../../../../newton-s-second-law.md) gives $m\ddot x=-b\dot x-kx$. The characteristic exponents are $-\gamma\pm i\omega_1$, where

$$
\boxed{\gamma=\frac{b}{2m},\qquad\omega_1=\sqrt{\frac{k}{m}-\frac{b^2}{4m^2}},\qquad b^2<4mk.}
$$

For the stipulated [phase](../../../../../phase-waves.md) of the damped cosine,

$$
U(t)=\frac12kA^2e^{-2\gamma t}\cos^2(\omega_1t),\qquad
K(t)=\frac12mA^2e^{-2\gamma t}[\gamma\cos(\omega_1t)+\omega_1\sin(\omega_1t)]^2.
$$

At $t_n=2\pi n/\omega_1$, the [velocity](../../../../../velocity.md) is not zero: $\dot x=-\gamma Ae^{-\gamma t_n}$. Thus

$$
E_n=\tfrac12(k+m\gamma^2)A^2e^{-2\gamma t_n},\qquad
\boxed{\frac{E_{n+1}}{E_n}=e^{-4\pi\gamma/\omega_1},\quad
\frac{E_n-E_{n+1}}{E_n}=1-e^{-4\pi\gamma/\omega_1}.}
$$

Expanding $e^{-z}$ at small $z=4\pi\gamma/\omega_1$ gives the requested light-damping loss $z$. The exact instantaneous [energy](../../../../../energy-split.md) also satisfies $dE/dt=-b\dot x^2\leq0$.

From the static extension, $k=mg/(0.20\,\mathrm m)=44.145\,\mathrm{N\,m^{-1}}$; the instantaneous drag measurement gives $b=0.10\,\mathrm{N\,s\,m^{-1}}$. Consequently $\gamma=0.05556\,\mathrm{s^{-1}}$ and $\omega_1=7.003\,\mathrm{s^{-1}}$. Two successive downward equilibrium crossings are one damped period apart, so the same [energy](../../../../../energy-split.md) ratio applies. At the first crossing $E=mv^2/2=1.125\times10^{-3}\,\mathrm J$. Therefore

$$
\boxed{\Delta E=1.07\times10^{-4}\,\mathrm J,\qquad
v_{\rm next}=v e^{-2\pi\gamma/\omega_1}=0.04757\,\mathrm{m\,s^{-1}}.}
$$

The [speed](../../../../../speed.md) has **decreased by $2.43\times10^{-3}\,\mathrm{m\,s^{-1}}=0.243\,\mathrm{cm\,s^{-1}}$**. These values use the exact decay factor, not the first-order approximation.

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
