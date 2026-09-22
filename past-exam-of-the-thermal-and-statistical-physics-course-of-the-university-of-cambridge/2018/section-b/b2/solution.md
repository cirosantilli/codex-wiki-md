<h1 id="section-b/b2/solution">Solution</h1>

↑ **Parent:** [B2](../b2.md)

**[Fermion](../../../../fermion.md) occupation and ordinary metallic [heat capacity](../../../../heat-capacity.md).** The [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) for a single-particle state is

$$
\boxed{\langle n(E)\rangle=\frac1{e^{(E-\mu)/(k_BT)}+1}.}
$$

At low [temperature](../../../../temperature-split.md) it changes appreciably only in an [energy](../../../../energy-split.md) window of width of order $k_BT$ about $\mu\simeq E_F$. If the full [density of states](../../../../density-of-states.md) $D(E)$ is smooth and nonzero there, only about $D(E_F)k_BT$ states change population. Each excited particle or hole carries [energy](../../../../energy-split.md) of order $k_BT$ relative to the [Fermi surface](../../../../fermi-surface.md), so $U(T)-U(0)$ is of order $D(E_F)(k_BT)^2$. Differentiation therefore gives $C_{\mathrm{el}}\propto T$.

More precisely, the fixed-number [Sommerfeld expansion](../../../../sommerfeld-expansion.md) gives

$$
U(T)-U(0)=\frac{\pi^2}{6}D(E_F)(k_BT)^2+O(T^4),
\qquad
\boxed{C_{\mathrm{el}}=\frac{\pi^2}{3}D(E_F)k_B^2T+O(T^3).}
$$

Here $D$ includes all counted internal species. This argument requires $k_BT\ll E_F$ and a [density of states](../../../../density-of-states.md) varying slowly across the thermal window; a band edge or vanishing [density of states](../../../../density-of-states.md) can change the power law.

**Two-dimensional linear dispersion at zero [chemical potential](../../../../chemical-potential-split.md).** Let $g$ count identical positive-energy branches, keeping the state-counting convention explicit. The number of [wavevector](../../../../wavevector.md) states in a ring of radius $k$ is $gA(2\pi k\,dk)/(2\pi)^2$. With $E=\hbar vk$, this gives

$$
D_+(E)=\frac{gAE}{2\pi\hbar^2v^2},\qquad E\geq0.
$$

At $\mu=0$, the thermal [energy](../../../../energy-split.md) of this branch is

$$
U_+(T)=\int_0^\infty D_+(E)\frac{E\,dE}{e^{E/(k_BT)}+1}
=\frac{gA(k_BT)^3}{2\pi\hbar^2v^2}
\int_0^\infty\frac{x^2}{e^x+1}dx.
$$

The dimensionless [integral](../../../../integral-split.md) is $3\zeta(3)/2$. Differentiating gives

$$
\boxed{C_+(T)=\frac{9g\zeta(3)}{4\pi}\frac{Ak_B^3T^2}{\hbar^2v^2}
\sim\frac{Ak_B^3T^2}{\hbar^2v^2}.}
$$

This is the [heat capacity for a two-dimensional linear fermion dispersion](../../../../heat-capacity-for-a-two-dimensional-linear-fermion-dispersion.md). A physical neutral particle–hole-symmetric [Dirac cone](../../../../dirac-cone.md) also has [electron holes](../../../../electron-hole.md) in its filled negative-energy band. Their excitation [energy](../../../../energy-split.md) gives an equal contribution, doubling $C_+$ for the same cone count. The $T^2$ scaling is unchanged. For a positive-energy-only gas, holding $\mu=0$ allows its mean [particle number](../../../../particle-number.md) to vary; a neutral two-band surface instead maintains zero net excess charge as [electron](../../../../electron.md)–hole pairs are thermally excited. These conventions should not be conflated when specifying an exact coefficient.

**Nonzero [chemical potential](../../../../chemical-potential-split.md).** The ordinary metallic regime is

$$
\boxed{k_BT\ll\mu\quad\text{or}\quad T\ll\mu/k_B.}
$$

The thermal window then lies far from the cone tip. Since $D(E)\propto E$, its fractional change across that window is only of order $k_BT/\mu$. Treating it as locally constant restores the Sommerfeld result $C_{\mathrm{el}}\propto D(\mu)T\propto\mu T$. When $k_BT$ is comparable to or larger than $\mu$, the window probes the vanishing [density of states](../../../../density-of-states.md) near the tip and crosses toward the neutral $T^2$ behavior, provided the linear dispersion remains valid.

**Bulk [phonons](../../../../phonon.md) and the surface-to-bulk comparison.** For the [topological insulator](../../../../topological-insulator.md) model, assume bulk electronic excitations are frozen out while the conducting surface remains active. In three dimensions, acoustic [phonons](../../../../phonon.md) have a density of modes proportional to $\omega^2$. Normalize the Debye spectrum to $3N$ modes:

$$
D_{\mathrm{ph}}(\omega)=\frac{9N\omega^2}{\omega_D^3},\qquad
\hbar\omega_D=k_B\Theta_D.
$$

The thermal part of the [energy](../../../../energy-split.md) is

$$
U_{\mathrm{ph}}=\frac{9N\hbar}{\omega_D^3}
\int_0^{\omega_D}\frac{\omega^3}{e^{\hbar\omega/(k_BT)}-1}d\omega.
$$

At $T\ll\Theta_D$, extending the upper integration [limit](../../../../limit-of-a-function.md) to infinity introduces an exponentially small error. With $x=\hbar\omega/(k_BT)$ and $\int_0^\infty x^3/(e^x-1)dx=\pi^4/15$,

$$
U_{\mathrm{ph}}\simeq\frac{3\pi^4}{5}Nk_B\frac{T^4}{\Theta_D^3},
\qquad
\boxed{C_{\mathrm{ph}}\simeq\frac{12\pi^4}{5}Nk_B\left(\frac T{\Theta_D}\right)^3.}
$$

Temperature-independent [zero-point energy](../../../../zero-point-energy.md) makes no contribution to this [heat capacity](../../../../heat-capacity.md). The requested ratio consequently scales as

$$
\boxed{\frac{C_{\mathrm{el}}}{C_{\mathrm{ph}}}
\sim\frac{Ak_B^2\Theta_D^3}{\hbar^2v^2NT}.}
$$

For a fixed shape and composition, $A\propto L^2$ and $N\propto L^3$, so the ratio grows as $1/(LT)$. Smaller samples and lower temperatures favor the surface contribution. It dominates if the dimensionless right-hand side, including its state-counting prefactor, exceeds unity. This is the [surface-electron and bulk-phonon heat-capacity crossover](../../../../surface-electron-and-bulk-phonon-heat-capacity-crossover.md).

The continuum electronic law also requires a thermal [energy](../../../../energy-split.md) larger than the surface finite-size level spacing, of order $\hbar v/L$. The [phonon](../../../../phonon.md) continuum has its own finite-size cutoff. Therefore dominance obtained by formally taking $T\to0$ cannot always be inferred from the two continuum power laws alone.

There is a numerical-normalization qualification in the paper. Combining the explicit one-positive-branch result above with the conventional $3N$-mode Debye normalization gives ratio prefactor $15g\zeta(3)/(16\pi^5)$; including [electron holes](../../../../electron-hole.md) doubles it. For $g=1$, this is approximately $0.00368$ before that doubling, rather than the supplied $5/(12\pi^2)\simeq0.0422$. The problem specifies neither a cone/[spin](../../../../spin.md) multiplicity that equates these nor another mode normalization. Its supplied prefactor is therefore used as the stipulated approximation for the requested numerical estimate, rather than claimed as an exact consequence of the single-branch count.

**Numerical estimate.** A cubic sample of [volume](../../../../volume-thermodynamics.md) $1\,\mathrm{mm^3}$ has side $L=10^{-3}\,\mathrm m$. Counting the conducting surface on all six faces gives

$$
A=6L^2=6\times10^{-6}\,\mathrm{m^2}.
$$

For one atom per cubic cell of side $a=1.5\times10^{-9}\,\mathrm m$,

$$
N\simeq\frac{L^3}{a^3}=2.96\times10^{17}.
$$

Use $k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}$ and $\hbar=1.05457\times10^{-34}\,\mathrm{J\,s}$. Inserting the stated $v=5\times10^5\,\mathrm{m\,s^{-1}}$, $\Theta_D=500\,\mathrm K$ and $T=1\,\mathrm K$ into the paper's supplied prefactor gives

$$
\boxed{\frac{C_{\mathrm{el}}}{C_{\mathrm{ph}}}\simeq7.33\times10^{-6}.}
$$

Thus bulk [phonons](../../../../phonon.md) dominate at this [temperature](../../../../temperature-split.md) in this estimate. If only one face contributes, the ratio is $1.22\times10^{-6}$; if there are $\nu$ [chemical atoms](../../../../atom-physics.md) per [unit cell](../../../../unit-cell.md), divide the corresponding estimate by $\nu$. These geometrical and crystallographic factors are not supplied explicitly.

With the same prefactor and geometry, extrapolating $1/T$ would suggest equality near $7.3\,\mathrm{\mu K}$. However, the surface finite-size scale is already of order $\hbar v/(k_BL)\simeq3.8\,\mathrm{mK}$ for this specimen. That extrapolated crossover lies outside the continuum electronic regime, so it is not a reliable prediction of the sample's ultimate lowest-temperature [heat capacity](../../../../heat-capacity.md).

## ↑ Ancestors (13)

1. [B2](../b2.md)
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
