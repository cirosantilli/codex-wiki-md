<h1 id="section-d/d12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $v$ be the inverting-input potential. The non-inverting input is grounded, so the [ideal operational amplifier](../../../../../../ideal-operational-amplifier.md) rules give $v=0$ and no input current. [Kirchhoff's current law](../../../../../../kirchhoff-node-law.md) at that node therefore gives

$$
\frac{V_{\mathrm{in}}-v}{R}=C\frac{d(v-V_{\mathrm{out}})}{dt}=-C\frac{dV_{\mathrm{out}}}{dt}.
$$

Integrating from an initial time $t_0$,

$$
\boxed{V_{\mathrm{out}}(t)=V_{\mathrm{out}}(t_0)-\frac1{RC}\int_{t_0}^tV_{\mathrm{in}}(u)\,du.}
$$

This [op amp integrator](../../../../../../op-amp-integrator.md) performs inverted time integration; the initial [voltage](../../../../../../voltage.md) across the [capacitor](../../../../../../capacitor.md) supplies the integration constant. For zero initial conditions its [transfer function](../../../../../../transfer-function.md) is $H(s)=-1/(sRC)$. In sinusoidal steady state, with the convention $e^{i\omega t}$,

$$
\boxed{H(i\omega)=-\frac1{i\omega RC}=\frac{i}{\omega RC},\qquad |H|=\frac1{\omega RC},\qquad \arg H=+90^\circ.}
$$

For example, a cosine input produces a negative sine output after its constant component is set. The additional inversion makes the phase $+90^\circ$ modulo $360^\circ$, rather than the $-90^\circ$ of non-inverting integration.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
