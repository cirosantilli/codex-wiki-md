<h1 id="section-b/21b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let the Maxwell branch contain [spring](../../../../../../spring.md) modulus $G$ and series viscosity $\eta_M$, in parallel with a [dashpot](../../../../../../dashpot.md) of viscosity $\eta_s$. The branch [strains](../../../../../../strain.md) are equal and stresses add. Writing $\sigma_M$ for the Maxwell [stress](../../../../../../stress.md),

$$
\dot\gamma=\frac{\dot\sigma_M}{G}+\frac{\sigma_M}{\eta_M},
\qquad \sigma=\sigma_M+\eta_s\dot\gamma.
$$

For $\gamma=\operatorname{Re}(\gamma_0e^{i\omega t})$ and $\tau=\eta_M/G$,

$$
\boxed{G^*(\omega)=i\omega\eta_s+
G\frac{i\omega\tau}{1+i\omega\tau}}.
$$

Multiplying the Maxwell fraction by $1-i\omega\tau$ gives

$$
\boxed{G'=\frac{G(\omega\tau)^2}{1+(\omega\tau)^2},\qquad
G''=\omega\eta_s+\frac{G\omega\tau}{1+(\omega\tau)^2}}.
$$

The sign of the imaginary coefficient depends on the phasor convention; these expressions use $e^{i\omega t}$, so $G''>0$ represents dissipation. In the time domain, the equivalent constitutive relation is

$$
\sigma+\tau\dot\sigma=(\eta_M+\eta_s)\dot\gamma+\tau\eta_s\ddot\gamma.
$$

The original mechanical schematic shows the series [spring](../../../../../../spring.md)/[dashpot](../../../../../../dashpot.md) branch separately from the parallel [dashpot](../../../../../../dashpot.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [21B](../../21b.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
