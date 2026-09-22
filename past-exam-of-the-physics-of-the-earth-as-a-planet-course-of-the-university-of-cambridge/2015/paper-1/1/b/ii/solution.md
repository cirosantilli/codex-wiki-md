<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a mode of positive [frequency](../../../../../../frequency.md), differentiation of the causal [convolution](../../../../../../convolution.md) gives

$$
\dot a(t)=\int_0^t\cos[\omega(t-s)]f(s)\,ds,
$$



$$
\ddot a(t)=f(t)-\omega\int_0^t\sin[\omega(t-s)]f(s)\,ds
=f(t)-\omega^2a(t).
$$

The first boundary term vanishes because $\sin0=0$; the second supplies $f(t)$ because $\cos0=1$. Both initial values vanish. This verifies the forced-oscillator equation and its [initial conditions](../../../../../../initial-condition.md), including a step source in the piecewise or distributional sense.

The spatial [Dirac delta function](../../../../../../dirac-delta-function.md) reduces the excitation to

$$
f_\alpha(t)=C_\alpha H(t-t_s),\qquad
C_\alpha=\mathbf M:\mathbf e_\alpha^*(\mathbf x_s).
$$

For an event at $t_s\ge0$, put $\tau=t-t_s$. Integrating the oscillator kernel from $t_s$ to $t$ gives the [normal-mode response to a step seismic moment](../../../../../../normal-mode-response-to-a-step-seismic-moment.md):

$$
a_\alpha(t)=\frac{C_\alpha}{\omega_\alpha^2}
[1-\cos(\omega_\alpha\tau)]H(\tau),
$$



$$
\boxed{\mathbf u(\mathbf x,t)=H(\tau)\sum_\alpha
\mathbf u_\alpha(\mathbf x)
\frac{\mathbf M:\mathbf e_\alpha^*(\mathbf x_s)}{\omega_\alpha^2}
[1-\cos(\omega_\alpha\tau)].}
$$

Non-unit mass normalization introduces the same factor $1/N_\alpha$ as above. Complex modes must be combined with their conjugate partners to produce a real displacement. The formal $\omega\to0$ limit is $a=C\tau^2H(\tau)/2$; for rigid-body modes here, $C=0$ because their [strain](../../../../../../strain.md) is zero.

The step produces a static component plus continuing oscillations in this lossless model. It does not predict physical damping. **A point source is appropriate when rupture dimensions are small compared with the [wavelengths](../../../../../../wavelength.md) being analysed and rupture duration is short compared with their [periods](../../../../../../period-of-a-function.md).** Long-period observations of a relatively small [earthquake](../../../../../../earthquake.md) can meet these conditions; high-frequency finite-fault directivity generally cannot. A finite source-time function replaces the ideal instantaneous step when its duration matters.

## ↑ Ancestors (15)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../../split.md)
7. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
