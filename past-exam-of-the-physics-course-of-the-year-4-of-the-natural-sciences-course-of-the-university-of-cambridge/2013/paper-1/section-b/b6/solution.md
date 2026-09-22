<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For charge per length $\lambda_q$, [Gauss's law](../../../../../gauss-s-law.md) gives $E_r=\lambda_q/(2\pi\epsilon_0r)$ between the conductors. Integration gives $V=\lambda_q\ln(b/a)/(2\pi\epsilon_0)$. Similarly [Ampère's law](../../../../../ampere-s-circuital-law.md) gives $B_\phi=\mu_0I/(2\pi r)$; integrating the magnetic [energy](../../../../../energy-split.md) per length and setting it equal to $LI^2/2$ gives

$$
\boxed{C=\frac{2\pi\epsilon_0}{\ln(b/a)},\qquad L=\frac{\mu_0}{2\pi}\ln(b/a).}
$$

Here $C,L$ are per unit length. The displayed $L$ is the external TEM inductance, appropriate to the ideal surface-current/high-frequency model. Internal magnetic [energy](../../../../../energy-split.md) in conductors with appreciable current penetration adds internal inductance; it cannot be determined fully from an outer conductor with unspecified wall geometry.

The distributed series resistance and inductance, with shunt capacitance and negligible leakage, give the [telegrapher's equations](../../../../../telegrapher-s-equations.md)

$$
\partial_xV=-L\partial_tI-RI,\qquad\partial_xI=-C\partial_tV.
$$

Differentiate the first with respect to $x$ and substitute the second to obtain

$$
\boxed{\partial_x^2V=LC\partial_t^2V+RC\partial_tV.}
$$

For $V\propto e^{ikx-i\omega t}$ the forward attenuating branch has $k^2=\omega^2LC+i\omega RC$. When $R\ll\omega L$,

$$
\boxed{k\simeq\omega\sqrt{LC}+i\frac R2\sqrt{\frac CL},\qquad
v_{\rm ph}\simeq\frac1{\sqrt{LC}}=c,\qquad
\ell_{\rm amp}=\frac2R\sqrt{\frac LC}.}
$$

The positive imaginary part gives amplitude $e^{-x/\ell_{\rm amp}}$. Power decays twice as fast in its exponent, so its attenuation length is $\ell_{\rm amp}/2$. Finite conductivity changes the speed only at higher order in this constant-parameter weak-loss expansion, apart from any separately retained internal inductance or dielectric response.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
