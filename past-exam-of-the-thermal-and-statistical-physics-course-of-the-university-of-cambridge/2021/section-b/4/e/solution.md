<h1 id="section-b/4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Substituting the [chemical potentials](../../../../../chemical-potential-split.md) into the equilibrium relation gives

$$
2\ln(n_c\lambda_c^3)-\beta\epsilon
=2\ln(n_{\rm CO}\lambda_{\rm CO}^3)+\ln(n_{\rm O_2}\lambda_{\rm O_2}^3).
$$

Exponentiation and the positive square root give the [law of mass action](../../../../../law-of-mass-action.md) in number-density form:

$$
\boxed{n_c=n_{\rm CO}\sqrt{n_{\rm O_2}}\,\frac{\lambda_{\rm CO}^3\lambda_{\rm O_2}^{3/2}}{\lambda_c^3}\,e^{\epsilon/(2k_BT)}.}
$$

All three [thermal de Broglie wavelengths](../../../../../thermal-de-broglie-wavelength.md) have the same $T^{-1/2}$ dependence. Define the temperature-independent mass factor

$$
B=\left(\frac{m_c}{m_{\rm CO}}\right)^{3/2}\left(\frac{m_c}{m_{\rm O_2}}\right)^{3/4},\qquad
\frac{\lambda_{\rm CO}^3\lambda_{\rm O_2}^{3/2}}{\lambda_c^3}=B\lambda_c^{3/2}.
$$

If $f_\alpha=n_\alpha/n$, this exact equilibrium relation can be written

$$
n_c=Bf_{\rm CO}\sqrt{f_{\rm O_2}}\,n^{3/2}\lambda_c^{3/2}e^{\epsilon/(2k_BT)}.
$$

It already has the requested dimensional structure: $n^{3/2}\lambda_c^{3/2}$ has units $\mathrm{m^{-3}}$. Its coefficient, however, depends on the conserved elemental composition through the species fractions.

For the intended case of a gas obtained by dissociating initially pure [carbon dioxide](../../../../../carbon-dioxide.md), conservation of the elemental ratio gives $n_{\rm CO}=2n_{\rm O_2}$ throughout. Hence

$$
n_{\rm CO}=\frac23(n-n_c),\qquad n_{\rm O_2}=\frac13(n-n_c),
$$

and the exact relation within this ideal-mixture model is

$$
n_c=A_0(n-n_c)^{3/2}\lambda_c^{3/2}e^{\epsilon/(2k_BT)},\qquad A_0=\frac{2B}{3\sqrt3}.
$$

At high [temperature](../../../../../temperature-split.md) with $k_BT\gg\epsilon$ and in the dilute [ideal gas](../../../../../ideal-gas-split.md) regime, $n\lambda_c^3\ll1$, this equation is self-consistently dissociation dominated:

$$
\frac{n_c}{n}\simeq A_0\sqrt{n\lambda_c^3}\,e^{\epsilon/(2k_BT)}\ll1.
$$

Thus $n-n_c\simeq n$, and to leading order

$$
\boxed{n_{\rm CO_2}\simeq A\,n^{3/2}\lambda_{\rm CO_2}^{3/2}e^{\epsilon/(2k_BT)},\quad
A=\frac{2}{3\sqrt3}\left(\frac{m_{\rm CO_2}}{m_{\rm CO}}\right)^{3/2}\left(\frac{m_{\rm CO_2}}{m_{\rm O_2}}\right)^{3/4}.}
$$

Using nominal molecular masses $28,32,44$ in common mass units gives $A\simeq0.963$, confirming that it is of order unity. The exponential has been retained as the leading binding correction, although it tends to one as $T\to\infty$.

The printed question does not explicitly fix the elemental composition. Without the initially-pure-$\mathrm{CO_2}$ assumption, the universal result is the boxed mass-action relation, and $A=Bf_{\rm CO}\sqrt{f_{\rm O_2}}$ approaches a composition-dependent constant when both dissociation products have nonzero high-temperature fractions. It need not be of order unity for an arbitrarily unbalanced mixture. Also, $k_BT\gg\epsilon$ alone does not justify replacing $n-n_c$ by $n$ at arbitrarily high density; the dilute classical regime is part of the model.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
