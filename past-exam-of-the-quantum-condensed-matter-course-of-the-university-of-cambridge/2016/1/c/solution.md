<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For nondegenerate [electrons](../../../../electron.md) in a parabolic [conduction band](../../../../conduction-band.md),

$$
n(T)=N_c(T)\exp\left[-\frac{\Delta(T)}{k_BT}\right],\qquad \Delta(T)=E_c(T)-\mu(T),\qquad N_c(T)\propto T^{3/2}
$$

when the density-of-states [effective mass](../../../../band-effective-mass.md) and valley multiplicity are fixed. The [intrinsic carrier extrapolation across a crossover](../../../../intrinsic-carrier-extrapolation-across-a-crossover.md) must therefore specify how the activation [energy](../../../../energy-split.md) changes with [temperature](../../../../temperature-split.md).

The usual intended estimate treats the quoted $0.9\,\mathrm{eV}$ as a constant intrinsic activation [energy](../../../../energy-split.md) between the two temperatures, and identifies the crossover by $n_i(T_c)\simeq n_{\rm ext}$. Then

$$
\frac{n_i(T_c)}{n_i(T_1)}=\left(\frac{T_c}{T_1}\right)^{3/2}\exp\left[-\frac{0.9\,\mathrm{eV}}{k_B}\left(\frac1{T_c}-\frac1{T_1}\right)\right].
$$

For $T_1=350\,\mathrm K$, $T_c=280\,\mathrm K$ and $k_B=8.6173\times10^{-5}\,\mathrm{eV\,K^{-1}}$, the exponent is $-7.46$ and the prefactor is $0.8^{3/2}=0.7155$. Hence

$$
\boxed{n_{\rm ext}\simeq(2.3\times10^{16})(0.7155)e^{-7.46}\simeq9.5\times10^{12}\,\mathrm{cm^{-3}}\quad\text{under the constant-activation approximation}.}
$$

Equivalently, a fixed-gap intrinsic model with $E_g/2=0.9\,\mathrm{eV}$ gives this result. A crossover is gradual: if $n_{\rm ext}$ denotes the net ionized donor density and $n_i(T_c)=n_{\rm ext}$, [charge neutrality](../../../../charge-neutrality.md) gives the actual [electron](../../../../electron.md) population $n(T_c)=(1+\sqrt5)n_{\rm ext}/2$, rather than exactly $n_{\rm ext}$.

There are two limits to interpreting the numerical estimate literally. First, the printed data specify $E_c-\mu$ only at $350\,\mathrm K$, without specifying $E_g$ or the valence [density of states](../../../../density-of-states.md). They do not mathematically determine $\Delta(280\,\mathrm K)$: without the intended activation assumption the answer remains

$$
n_{\rm ext}\simeq n(350)\left(\frac{280}{350}\right)^{3/2}\exp\left[-\frac{\Delta(280)}{k_B(280)}+\frac{0.9\,\mathrm{eV}}{k_B(350)}\right].
$$

Second, using the original PDF's $0.9\,\mathrm{eV}$ and density implies $N_c(350)\simeq2.1\times10^{29}\,\mathrm{cm^{-3}}$, extraordinarily large for a conventional [semiconductor](../../../../semiconductor-split.md). This confirms that the numerical data should not be treated as a realistic material determination. No unprinted decimal-point correction has been assumed.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
