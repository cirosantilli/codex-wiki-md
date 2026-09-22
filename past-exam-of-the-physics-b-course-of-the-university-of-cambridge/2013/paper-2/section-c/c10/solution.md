<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For [speed](../../../../../speed.md) distribution $f(v)$ normalized to one and isotropic directions, the incident number flux is

$$
J=n\int_0^\infty vf(v)\,dv\,
\frac1{4\pi}\int_0^{2\pi}d\phi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta
=\boxed{\frac14n\overline v.}
$$

The positive normal [velocity](../../../../../velocity.md) weights the population reaching the wall. Consequently its mean translational [energy](../../../../../energy-split.md) is

$$
\langle E\rangle_{\rm hit}=\frac m2\frac{\int_0^\infty v^5e^{-av^2}\,dv}{\int_0^\infty v^3e^{-av^2}\,dv}
=\frac m2\frac{a^{-3}}{(2a^2)^{-1}}
=\boxed{2k_BT},\qquad a=\frac{m}{2k_BT}.
$$

The bulk value $3k_BT/2$ would omit the arrival weighting.

For the two vessels, let $r=\sqrt{T_1/T_0}$, with subscripts h and c for hot and cold. Equal opposing [effusion](../../../../../effusion.md) rates give $p_h/\sqrt{T_1}=p_c/\sqrt{T_0}$. Number conservation in equal, fixed volumes adds $p_h/T_1+p_c/T_0=2p_0/T_0$. Hence

$$
\boxed{p_c=\frac{2p_0r}{1+r},\quad p_h=\frac{2p_0r^2}{1+r},\quad
p_h-p_c=\frac{2p_0r(r-1)}{1+r}.}
$$

Both final [pressures](../../../../../pressure-split.md) must be determined; holding the cold [temperature](../../../../../temperature-split.md) fixed does not hold its [particle number](../../../../../particle-number.md) fixed.

For aperture [area](../../../../../surface-area.md) $A_h=\pi d^2/4$, the common one-way flux is $J=p_c/\sqrt{2\pi m k_BT_0}$. The translational [heat](../../../../../heat-split.md) transfer from hot to cold is therefore

$$
\boxed{\dot Q=2k_B(T_1-T_0)A_hJ.}
$$

This is the total [heat](../../../../../heat-split.md) transfer for a monatomic gas with no active internal modes, neglecting radiation and conduction through vessel walls. For a molecular gas, add $A_hJ[u_{\rm int}(T_1)-u_{\rm int}(T_0)]$ for its [internal energy](../../../../../internal-energy-split.md) per molecule. The maintained unequal [temperatures](../../../../../temperature-split.md) describe a stationary nonequilibrium state even though the net particle current is zero.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
