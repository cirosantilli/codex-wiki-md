<h1 id="a6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the supplied separable molecular model,

$$
f_i=\left(\frac{2\pi m_i k_{\mathrm B}T}{h^2}\right)^{3/2}
q_{\mathrm{rot},i}\bar q_{\mathrm{vib},i},
$$

with electronic factors unity. The integer masses are $2u$, $28u$ and $30u$. The [rotational symmetry numbers](../../../../../../rotational-symmetry-number.md) are respectively $2,1,2$: rotating either hydrogen or methanal by $180^\circ$ about its appropriate symmetry axis exchanges identical hydrogens, whereas CO has distinct ends.

With the given conversion $k_{\mathrm B}/hc=0.6950\ \mathrm{cm^{-1}\,K^{-1}}$, a spectroscopic constant $\widetilde b$ corresponds to a temperature $\theta=\widetilde b/0.6950$. At $500$ K the partition-function factors are

$$
\begin{array}{c|rrr}
 &\mathrm H_2&\mathrm{CO}&\mathrm{H_2CO}\\\hline
f_{\mathrm{trans}}/\mathrm{m^{-3}}&5.9429\times10^{30}&3.1131\times10^{32}&3.4525\times10^{32}\\
q_{\mathrm{rot}}&2.8484&182.895&1565.83\\
\bar q_{\mathrm{vib}}&1.7804\times10^{-3}&4.4141\times10^{-2}&9.6\times10^{-8}\\
f/\mathrm{m^{-3}}&3.0137\times10^{28}&2.5133\times10^{33}&5.1898\times10^{28}
\end{array}
$$

For instance,

$$
q_{\mathrm{rot},\mathrm{H_2CO}}=\frac{\sqrt\pi}{2}
\left[\frac{(0.6950\times500)^3}{9.4\times1.3\times1.1}\right]^{1/2}
=1565.83.
$$

The [vibrational partition functions](../../../../../../vibrational-partition-function.md) here include their zero-point Boltzmann factors. The given reference-energy change must therefore be used consistently with that convention; adding a second vibrational [zero-point energy](../../../../../../zero-point-energy.md) correction would double count it. Because the numerical energy change is per mole, its exponential uses $RT$, not $k_{\mathrm B}T$:

$$
\exp\left(\frac{18000}{R\times500}\right)=75.9295.
$$

Consequently,

$$
\boxed{K_c=\frac{(5.1898\times10^{28})(1\ \mathrm{m^{-3}})}
{(3.0137\times10^{28})(2.5133\times10^{33})}\,75.9295
\simeq5.20\times10^{-32}.}
$$

This tiny dimensionless value refers to the extremely dilute one-molecule-per-cubic-metre standard state. It is not a concentration-independent statement about the fraction of carbon monoxide converted in a particular cloud. The calculation follows the supplied classical rotational and harmonic vibrational formulas, without adding separate nuclear-spin factors.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [A6](../../../a6.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
