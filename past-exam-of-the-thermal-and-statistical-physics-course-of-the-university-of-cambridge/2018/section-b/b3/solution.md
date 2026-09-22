<h1 id="section-b/b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

**Classical translational statistics.** Write the [number density](../../../../number-density.md) as $n=N/V$ and the [thermal de Broglie wavelength](../../../../thermal-de-broglie-wavelength.md) as $\lambda=\sqrt{2\pi\hbar^2/(mk_BT)}$. Quantum exchange is negligible when [wave packets](../../../../wave-packet.md) rarely overlap:

$$
\boxed{n\lambda^3\ll1\quad\text{or}\quad n^{-1/3}\gg\lambda.}
$$

The equivalent state-counting statement is that the mean occupation of each thermally relevant one-particle state is much smaller than one. The equations in this question count one internal species; with $g$ equally populated [spin](../../../../spin.md) states the relevant density per species is $n/g$.

Let $z=e^{\beta\mu}$ be the dimensionless [quantum gas fugacity](../../../../fugacity-statistical-mechanics.md), with the lowest one-particle [energy](../../../../energy-split.md) chosen as zero. Both quantum distributions can be written

$$
n_\eta(E)=\frac1{z^{-1}e^{\beta E}-\eta}
=\frac{ze^{-\beta E}}{1-\eta ze^{-\beta E}},
\qquad\eta=\begin{cases}+1&\text{bosons},\\-1&\text{fermions}.\end{cases}
$$

If $z\ll1$, then $n_\eta(E)\simeq ze^{-\beta E}\ll1$ for all $E\geq0$, recovering [Maxwell–Boltzmann statistics](../../../../maxwell-boltzmann-statistics.md). Conversely, low occupation even at the spectrum's bottom requires $z/(1-z)\ll1$ for [bosons](../../../../boson.md) or $z/(1+z)\ll1$ for [fermions](../../../../fermion.md); either condition implies

$$
\boxed{z=e^{\beta\mu}\ll1.}
$$

A single high-energy state can be sparsely occupied even in a degenerate gas, so the condition must hold across the relevant spectrum, not just for one arbitrarily chosen [energy](../../../../energy-split.md). Also, classical translational statistics does not imply that all internal excitation [energies](../../../../energy-split.md) or other quantum effects can be ignored.

**Grand [partition function](../../../../canonical-partition-function.md), density and [pressure](../../../../pressure-split.md).** Noninteracting particles have independent occupations of each one-particle state. Put $x_{\mathbf k}=ze^{-\beta\varepsilon_{\mathbf k}}$. Summing the allowed occupations gives

$$
\Xi_{\mathbf k}=\begin{cases}
\sum_{r=0}^\infty x_{\mathbf k}^r=(1-x_{\mathbf k})^{-1}&\text{bosons},\\
1+x_{\mathbf k}&\text{fermions},
\end{cases}
\qquad
\Xi=\prod_{\mathbf k}(1-\eta x_{\mathbf k})^{-\eta}.
$$

Therefore

$$
\ln\Xi=-\eta\sum_{\mathbf k}\ln(1-\eta ze^{-\beta\varepsilon_{\mathbf k}}).
$$

The [grand potential](../../../../grand-potential.md) is $\Omega_G=-k_BT\ln\Xi=-pV$ for this homogeneous gas. Replacing the sum by $V\int d^3k/(2\pi)^3$ and using $\varepsilon_{\mathbf k}=\hbar^2k^2/(2m)$ gives

$$
\boxed{\beta p=-\eta\int\frac{d^3k}{(2\pi)^3}
\ln\left[1-\eta z e^{-\beta\hbar^2k^2/(2m)}\right].}
$$

The mean number is $N=z\,\partial_z\ln\Xi$, giving

$$
\boxed{\frac NV=\int\frac{d^3k}{(2\pi)^3}
\frac1{z^{-1}e^{\beta\hbar^2k^2/(2m)}-\eta}.}
$$

For [bosons](../../../../boson.md), the grand sum requires $z<1$ when the ground [energy](../../../../energy-split.md) is zero. A macroscopic condensate at the limiting $z\to1$ must be separated from the continuum [integral](../../../../integral-split.md) in the condensed phase. The following small-$z$ calculation is in the normal, nondegenerate regime, so that complication does not enter.

**Density expansion and inversion.** Expand the occupation as a [geometric series](../../../../geometric-series.md):

$$
n_\eta(E)=ze^{-\beta E}+\eta z^2e^{-2\beta E}+z^3e^{-3\beta E}+\cdots.
$$

The Gaussian [wavevector](../../../../wavevector.md) [integral](../../../../integral-split.md) for its $\ell$th term is

$$
\int\frac{d^3k}{(2\pi)^3}e^{-\ell\beta\hbar^2k^2/(2m)}
=\left(\frac{m}{2\pi\ell\beta\hbar^2}\right)^{3/2}
=\frac1{\lambda^3\ell^{3/2}}.
$$

It follows that

$$
\boxed{n\lambda^3=z+\frac{\eta z^2}{2^{3/2}}+O(z^3).}
$$

For the inverse series, put $y=n\lambda^3$ and try $z=y+c y^2+O(y^3)$. Substitution gives $0=(c+\eta/2^{3/2})y^2+O(y^3)$, hence

$$
\boxed{z=n\lambda^3-\frac\eta{2^{3/2}}(n\lambda^3)^2+O((n\lambda^3)^3).}
$$

The leading equality $n\lambda^3\simeq z$ directly connects the density and occupancy criteria for classical behavior.

**[Pressure](../../../../pressure-split.md) and its first quantum correction.** Expanding the [logarithm](../../../../logarithm.md) in the [pressure](../../../../pressure-split.md) expression gives one extra factor $1/\ell$ compared with the density series:

$$
\beta p\lambda^3=z+\frac{\eta z^2}{2^{5/2}}+O(z^3).
$$

Insert the inverse series. To second order in $y=n\lambda^3$,

$$
\beta p\lambda^3=y-\frac{\eta y^2}{2^{3/2}}+
\frac{\eta y^2}{2^{5/2}}+O(y^3)
=y-\frac{\eta y^2}{2^{5/2}}+O(y^3).
$$

Thus

$$
\boxed{pV=Nk_BT\left[1-\frac\eta{2^{5/2}}\frac{N\lambda^3}{V}
+O\left((N\lambda^3/V)^2\right)\right].}
$$

The first quantum correction at fixed density and [temperature](../../../../temperature-split.md) is

$$
\boxed{\Delta p=-\frac{\eta}{2^{5/2}}k_BT\,n^2\lambda^3.}
$$

It is negative for [bosons](../../../../boson.md) and positive for [fermions](../../../../fermion.md), and vanishes in the classical density [limit](../../../../limit-of-a-function.md).

**Virial coefficient.** Define the number-density [virial expansion](../../../../virial-expansion.md) by

$$
\frac p{nk_BT}=1+B_2(T)n+B_3(T)n^2+\cdots
=\sum_{j=1}^\infty B_j(T)n^{j-1},\qquad B_1=1.
$$

The coefficient $B_j$ has units $\mathrm{volume}^{j-1}$ in this convention. Comparing terms gives

$$
\boxed{B_2^{\mathrm{ex}}(T)=-\frac\eta{2^{5/2}}\lambda^3
=-\frac\eta{2^{5/2}}\left(\frac{2\pi\hbar^2}{mk_BT}\right)^{3/2}.}
$$

This is the [exchange contribution to the second virial coefficient](../../../../exchange-contribution-to-the-second-virial-coefficient.md). It arises without a pair-interaction potential; the underlying gas is noninteracting. A molar-density convention would multiply this $B_2$ by the Avogadro constant. For $g$ equally populated internal species, exchange occurs within each species and the coefficient in terms of total density is smaller by a factor $g$.

**Why the two signs differ.** [Bosonic exchange symmetry](../../../../bosonic-exchange-symmetry.md) enhances the [probability](../../../../probability.md) of nearby identical [bosons](../../../../boson.md), whereas [fermionic exchange symmetry](../../../../fermi-dirac-statistics.md) suppresses nearby identical [fermions](../../../../fermion.md) in the same internal state. In the dilute regime, the normalized equal-time [pair detection correlation](../../../../pair-detection-correlation.md) is

$$
g^{(2)}(r)=1+\eta e^{-2\pi r^2/\lambda^2}.
$$

The exchange part follows by squaring the Gaussian one-particle coherence factor $e^{-\pi r^2/\lambda^2}$. At zero separation this gives $g^{(2)}(0)=2$ for [bosons](../../../../boson.md) and $0$ for one-component [fermions](../../../../fermion.md). Integrating the exchange pair weight provides a direct coefficient check:

$$
B_2^{\mathrm{ex}}=-\frac12\int[g^{(2)}(r)-1]d^3r
=-\frac\eta2\left(\frac{\lambda^2}{2}\right)^{3/2}
=-\frac{\eta\lambda^3}{2^{5/2}}.
$$

Bunching therefore acts like an effective statistical attraction in the dilute [equation of state](../../../../equation-of-state.md), lowering the [pressure](../../../../pressure-split.md) needed at fixed density. Exclusion acts like an effective statistical repulsion, raising it. Neither description asserts an actual interparticle force. Different internal [fermion](../../../../fermion.md) species do not exclude each other from a common spatial location in the same way, explaining the importance of the species convention.

## ↑ Ancestors (13)

1. [B3](../b3.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
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
