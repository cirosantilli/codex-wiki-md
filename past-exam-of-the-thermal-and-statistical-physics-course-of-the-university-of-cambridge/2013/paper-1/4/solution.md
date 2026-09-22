<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At zero applied field, [time-reversal symmetry](../../../../t-symmetry.md) interchanges $M$ and $-M$ without changing the [free energy](../../../../thermodynamic-free-energy.md), so the analytic expansion contains only even [powers](../../../../power.md). The term $-\mu_0HM$ breaks this symmetry at fixed nonzero H. Stationarity and local stability require

$$
\boxed{\mu_0H=a(T)M+bM^3,\qquad a(T)+3bM^2>0.}
$$

For $T>T_c$ at small field, the cubic term is higher order and $M\simeq\mu_0H/a(T)$. Thus the susceptibility as defined in the question is

$$
\boxed{\chi=\left(\frac{\partial M}{\partial H}\right)_T\xrightarrow[H\to0]{}\frac{\mu_0}{a(T)}.}
$$

The three requested free-energy sketches and their minima are given separately above.

For the plotted isotherms, divide the [equation of state](../../../../equation-of-state.md) by nonzero M and rearrange:

$$
\boxed{M^2=\frac{\mu_0}{b}\frac HM-\frac{a(T)}b.}
$$

This is an [Arrott plot](../../../../arrott-plot.md): its slope determines b, and the isotherm through the origin identifies the mean-field [Curie temperature](../../../../curie-temperature.md).[1957, abstract: molecular-field criterion from cubic magnetisation versus internal field at the Curie temperature](../../../../criterion-for-ferromagnetism-from-observations-of-magnetic-isotherms-by-anthony-arrott.md) Under the paper's stated uniform-field Landau model, use H as supplied on its axis.

The ordinate unit is $(10^4\,\mathrm{A\,m^{-1}})^2=10^8\,\mathrm{A^2\,m^{-2}}$. Reading the original graph gives slopes about $0.076$–$0.080$ ordinate units per unit H/M, so the physical slope is approximately $7.8\times10^6\,\mathrm{A^2\,m^{-2}}$. Consequently

$$
\boxed{b\simeq1.6\times10^{-13}\,\mathrm{J\,m\,A^{-4}}.}
$$

Approximate horizontal intercepts and the corresponding $a=\mu_0(H/M)_{M^2=0}$ are:

- $4.2\,\mathrm K$: intercept $-62$, giving $a\simeq-7.8\times10^{-5}\,\mathrm{H\,m^{-1}}$.
- $13\,\mathrm K$: intercept $-40$, giving $a\simeq-5.1\times10^{-5}\,\mathrm{H\,m^{-1}}$.
- $19\,\mathrm K$: intercept $-15$, giving $a\simeq-1.9\times10^{-5}\,\mathrm{H\,m^{-1}}$.
- $25\,\mathrm K$: intercept $+17$, giving $a\simeq+2.2\times10^{-5}\,\mathrm{H\,m^{-1}}$.

The sign change brackets the transition between 19 and 25 K. A linear fit of $a(T)=\alpha(T-T_c)$ across the four read-offs gives approximately $\alpha=4.8\times10^{-6}\,\mathrm{H\,m^{-1}\,K^{-1}}$ and

$$
\boxed{T_c\simeq22\,\mathrm K.}
$$

Interpolating only the two nearest isotherms also gives about 22 K. These are graph estimates, not exact recovered measurements.

Below $T_c$ at zero field, the stable branches have $M_0^2=-a/b$. Substitution gives the [free-energy density](../../../../free-energy-density.md) relative to the omitted smooth background:

$$
F_{\min}=-\frac{a(T)^2}{4b}=-\frac{\alpha^2(T-T_c)^2}{4b}.
$$

The equilibrium excess heat-capacity [density](../../../../density.md) is $c_H=-T\partial_T^2F_{\min}=T\alpha^2/(2b)$ below $T_c$ and zero above it. Therefore

$$
\boxed{\Delta c_H=\frac{T_c\alpha^2}{2b}>0.}
$$

The all-isotherm linear fit gives **about $1.5\times10^3\,\mathrm{J\,m^{-3}\,K^{-1}}$**. Estimating the slope only between the 19 K and 25 K curves instead gives $\alpha\simeq6.9\times10^{-6}\,\mathrm{H\,m^{-1}\,K^{-1}}$ and a jump near $3\times10^3\,\mathrm{J\,m^{-3}\,K^{-1}}$. The lines are not exactly parallel and the intercepts are not perfectly linear in T, so **a jump of order a few $10^3\,\mathrm{J\,m^{-3}\,K^{-1}}$ is supported; finer precision is not**. This is per [volume](../../../../volume.md) because F is a [density](../../../../density.md); no sample [volume](../../../../volume.md) is given to convert it to a total [heat capacity](../../../../heat-capacity.md).

If $b<0$, the quartic truncation is unbounded below. Add a positive sixth-order term $cM^6/6$ with $c>0$. At zero field the coexistence conditions give

$$
M_{\rm jump}^2=-\frac{3b}{4c},\qquad
 a_{\rm transition}=\frac{3b^2}{16c}>0.
$$

Thus the zero-field transition is generically first order, with a discontinuous spontaneous magnetisation and possible [metastability](../../../../metastability.md). It occurs before the quadratic coefficient reaches zero. The case $b=0$ is the tricritical boundary of this mean-field model; no value of c is invented.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
