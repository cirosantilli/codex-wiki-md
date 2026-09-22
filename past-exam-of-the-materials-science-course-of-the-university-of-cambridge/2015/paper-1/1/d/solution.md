<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For [indexing a diamond-cubic powder pattern](../../../../../indexing-a-diamond-cubic-powder-pattern.md), $d_{hkl}=a/\sqrt{h^2+k^2+l^2}$ and [Bragg's law](../../../../../bragg-s-law.md) gives $\sin^2\theta=\lambda^2(h^2+k^2+l^2)/(4a^2)$. Using half of each printed scattering angle, the ratios to the first peak are approximately

$$
1,\ 2.66658,\ 3.66665,\ 5.33319,\ 6.33322.
$$

Multiplying by3 gives the allowed sequence $3,8,11,16,19$. Thus

$$
\boxed{111,\quad220,\quad311,\quad400,\quad331.}
$$

The numerical calculation, expressed without assuming a historical Data Book wavelength, is

$$
\begin{array}{c|c|c|c}
2\theta\ (\mathrm{deg})&hkl&h^2+k^2+l^2&a/\lambda\\\hline
28.524&111&3&3.51534\\
47.443&220&8&3.51540\\
56.294&311&11&3.51535\\
69.351&400&16&3.51538\\
76.629&331&19&3.51537
\end{array}
$$

Therefore **$a\simeq3.51537\lambda$**. As a separately identified reference convention, choosing Cu K$\alpha_1$ with $\lambda\simeq0.15406\ {\rm nm}$ gives

$$
\boxed{a\simeq0.54158\ {\rm nm}.}
$$

That wavelength follows from the copper $KL_3$ transition near $8047.8227\ {\rm eV}$ in the NIST transition database, using $\lambda=hc/E$.[Copper, experimental KL3 transition energy](../../../../../x-ray-transition-energies-database-by-national-institute-of-standards-and-technology.md)

The paper says Cu K$\alpha$ but does not give the line-selection convention or an explicit wavelength. A rounded unresolved-doublet wavelength, for example $0.15418\ {\rm nm}$, would instead give about $0.54200\ {\rm nm}$. These are conditional wavelength evaluations, not claims about the unavailable historical Data Book. The angles are internally consistent with one cubic parameter; they should not be replaced by literature peak positions simply to obtain a familiar [silicon](../../../../../silicon.md) value.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the materials science course of the University of Cambridge](../../../../split.md)
6. [Materials science course of the University of Cambridge](../../../../../materials-science-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
