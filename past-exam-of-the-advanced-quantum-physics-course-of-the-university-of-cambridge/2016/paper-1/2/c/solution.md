<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**[Fermi's golden rule](../../../../../fermi-s-golden-rule.md) converts a weak transition [matrix element](../../../../../matrix-element.md) and the available density of final states into a transition rate.** For a static perturbation $W$ and a continuum,

$$
\boxed{\Gamma_{i\to{\rm all}}=\frac{2\pi}{\hbar}
\int |\langle f|W|i\rangle|^2\delta(E_f-E_i)\,\mathrm dN_f.}
$$

When the [matrix element](../../../../../matrix-element.md) is nearly constant on the energy shell, this becomes $(2\pi/\hbar)|W_{fi}|^2\rho(E_i)$. The energy delta function is to be integrated, rather than interpreted as a finite rate to one exactly resonant discrete level. The observation time must resolve a smooth final-state continuum while remaining short enough that first-order depletion is small. A periodically driven perturbation instead gives the corresponding absorption and emission energy shells.

For elastic scattering from a weak localized potential $W(\mathbf r)$, use box-normalized free states $\langle\mathbf r|\mathbf k\rangle=\mathcal V^{-1/2}e^{i\mathbf k\cdot\mathbf r}$. Then

$$
W_{fi}=\frac1{\mathcal V}\widetilde W(\mathbf q),\qquad
\widetilde W(\mathbf q)=\int e^{-i\mathbf q\cdot\mathbf r}
W(\mathbf r)\,\mathrm d^3r,\qquad
\mathbf q=\mathbf k_f-\mathbf k_i.
$$

The number of final states is $\mathcal V k_f^2\,\mathrm dk_f\,\mathrm d\Omega/(2\pi)^3$. With $E_f=\hbar^2k_f^2/(2m)$, the density per energy and [solid angle](../../../../../solid-angle.md) is $\mathcal V m k_f/[(2\pi)^3\hbar^2]$. Dividing the resulting golden-rule rate by the incident single-particle flux $j_i=\hbar k_i/(m\mathcal V)$ gives

$$
\frac{\mathrm d\sigma}{\mathrm d\Omega}
=\frac{m^2}{4\pi^2\hbar^4}\frac{k_f}{k_i}
|\widetilde W(\mathbf q)|^2.
$$

This is the [golden-rule derivation of the Born cross-section](../../../../../golden-rule-derivation-of-the-born-cross-section.md). For the elastic problem $k_f=k_i$, so the first Born [scattering amplitude](../../../../../scattering-amplitude.md) and cross-section are

$$
\boxed{f_B(\mathbf k_f,\mathbf k_i)
=-\frac{m}{2\pi\hbar^2}\widetilde W(\mathbf q),\qquad
\frac{\mathrm d\sigma}{\mathrm d\Omega}=|f_B|^2.}
$$

The box volume cancels, as a physical cross-section must. The minus sign is fixed by the outgoing-wave scattering convention; the golden-rule rate alone determines only the modulus.

For example, $W(r)=g e^{-\kappa r}/r$ has $\widetilde W=4\pi g/(q^2+\kappa^2)$, hence $f_B=-2mg/[\hbar^2(q^2+\kappa^2)]$, with $q=2k\sin(\theta/2)$. Replacing the exact scattering state by the incident [plane wave](../../../../../plane-wave.md) is the essential [Born approximation](../../../../../born-approximation.md). It can fail for strong scattering, low-energy resonances and situations requiring repeated scattering; a small perturbation and a suitable continuum are separate conditions.[§6.3, Born approximation and Yukawa-potential example](../../../../../topics-in-quantum-mechanics-by-david-tong.md)

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
