<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

Use peak-amplitude [phasors](../../../../../phasor.md) with time factor $e^{-i\omega t}$ and $\mu=\mu_0$. [Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) and the [Ampere-Maxwell law](../../../../../ampere-s-circuital-law.md) give

$$
\nabla\times\mathbf E=i\omega\mu_0\mathbf H,\qquad
\nabla\times\mathbf H=(\sigma-i\omega\epsilon)\mathbf E,
\qquad k^2=\mu_0\epsilon\omega^2+i\mu_0\sigma\omega.
$$

In the good-conductor limit $\sigma\gg\omega\epsilon$, take the root with positive attenuation into the slab:

$$
k\simeq\frac{1+i}{\delta},\qquad \delta=\sqrt{\frac2{\mu_0\sigma\omega}},
\qquad
\boxed{\widetilde E_y(x)=E_0 e^{(i-1)x/\delta}.}
$$

The real physical field is $\operatorname{Re}[\widetilde E_y e^{-i\omega t}]$. A thick slab excludes a returning wave from its rear face. The [skin depth](../../../../../skin-depth.md) is the electric-field [amplitude](../../../../../wave-amplitude.md) decay [length](../../../../../length.md); the intensity decay [length](../../../../../length.md) is $\delta/2$.

[Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) fixes $\widetilde H_z=k\widetilde E_y/(\mu_0\omega)$. The [surface impedance of a good conductor](../../../../../surface-impedance-of-a-good-conductor.md) and the complete transmitted [magnetic field](../../../../../magnetic-field-split.md) are consequently

$$
\boxed{Z=\frac{\widetilde E_y}{\widetilde H_z}
=\frac{\mu_0\omega}{k}\simeq(1-i)\sqrt{\frac{\mu_0\omega}{2\sigma}}
=\frac{1-i}{\sigma\delta},\qquad
\widetilde{\mathbf H}=\frac{1+i}{\mu_0\omega\delta}E_0e^{(i-1)x/\delta}\widehat{\mathbf z}.}
$$

The sign of the imaginary part belongs to the stated time convention. Average the [Poynting vector](../../../../../poynting-vector.md) using complex conjugation and the factor one half appropriate to peak [phasors](../../../../../phasor.md):

$$
\langle\mathbf N\rangle=\frac12\operatorname{Re}(\widetilde{\mathbf E}\times\widetilde{\mathbf H}^{\,*})
=N_0e^{-2x/\delta}\widehat{\mathbf x},\qquad
\boxed{N_0=\frac{|E_0|^2}{2\mu_0\omega\delta}=\frac{\sigma\delta|E_0|^2}{4}.}
$$

As an independent [energy](../../../../../energy-split.md) check, $-\partial_x\langle N_x\rangle=\sigma|E_0|^2e^{-2x/\delta}/2$, the mean [Joule heating](../../../../../joule-heating.md) per unit [volume](../../../../../volume.md).

[Ohm's law](../../../../../ohm-s-law.md) gives $\widetilde J_y=\sigma\widetilde E_y$ and $\widetilde B_z=\mu_0\widetilde H_z$. Hence the averaged [Lorentz force](../../../../../lorentz-force.md) per unit [volume](../../../../../volume.md) is

$$
\langle f_x\rangle=\frac12\operatorname{Re}(\widetilde J_y\widetilde B_z^*)
=\sigma\mu_0 N_0 e^{-2x/\delta}.
$$

Integrating through the illuminated half-space gives the positive inward [radiation pressure](../../../../../radiation-pressure.md)

$$
\boxed{p=\int_0^\infty\langle f_x\rangle dx=\frac{\sigma\delta\mu_0}{2}N_0.}
$$

Finally let $Z_0=\sqrt{\mu_0/\epsilon_0}$ be the [vacuum](../../../../../vacuum.md) [wave impedance](../../../../../wave-impedance.md). Tangential-field [boundary conditions](../../../../../boundary-condition.md) at normal incidence give the electric-amplitude [reflection coefficient](../../../../../reflection-coefficient.md) $r=(Z-Z_0)/(Z+Z_0)$. Since $|Z|\ll Z_0$,

$$
R=|r|^2=1-\frac{4Z_0\operatorname{Re}Z}{|Z+Z_0|^2}
\simeq1-\frac{4\operatorname{Re}Z}{Z_0},\qquad
\boxed{R\simeq1-2\sqrt{\frac{2\omega\epsilon_0}{\sigma}}.}
$$

Here $N_0=(1-R)I_{\rm inc}$ by surface [energy](../../../../../energy-split.md) balance. Combining the leading formulas gives $p\simeq2I_{\rm inc}/c$, the nearly perfect-reflector limit. The displayed reflection expansion also assumes a good conductor relative to the incident [vacuum](../../../../../vacuum.md) wave, $\omega\epsilon_0/\sigma\ll1$.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
