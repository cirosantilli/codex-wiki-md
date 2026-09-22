<h1 id="section-b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**Occupation and the two-dimensional [Fermi energy](../../../../fermi-energy.md).** For an independent single-particle state, the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) is

$$
\boxed{n(\varepsilon)=\frac1{e^{\beta(\varepsilon-\mu)}+1},\qquad\beta=\frac1{k_BT}.}
$$

The [chemical potential](../../../../chemical-potential-split.md) enforces the chosen mean [particle number](../../../../particle-number.md) through $N=\sum_j n(\varepsilon_j)$, including [spin](../../../../spin.md) states in the sum. It is common to all states in particle-exchange equilibrium and must generally change with [temperature](../../../../temperature-split.md) or field when the total mean number is held fixed. At zero [temperature](../../../../temperature-split.md), the distribution becomes a [Heaviside step function](../../../../heaviside-step-function.md) at the [Fermi energy](../../../../fermi-energy.md).

Let the sample [area](../../../../surface-area.md) be $\mathcal S$ and let $g_s$ be its internal [spin](../../../../spin.md) [spin degeneracy](../../../../spin-degeneracy.md). In the continuum limit, filling the disk $k<k_F$ gives

$$
N=g_s\frac{\mathcal S}{(2\pi)^2}\pi k_F^2,
\qquad k_F^2=\frac{4\pi N}{g_s\mathcal S}.
$$

Therefore

$$
\boxed{\mu(T=0)=\varepsilon_F=\frac{\hbar^2k_F^2}{2m}
=\frac{2\pi\hbar^2}{g_s m}\frac N{\mathcal S}.}
$$

For spin-half [fermions](../../../../fermion.md) with both [spin](../../../../spin.md) states available, $g_s=2$ and $\varepsilon_F=\pi\hbar^2N/(m\mathcal S)$; for a spin-polarized gas $g_s=1$. The question does not specify the [area](../../../../surface-area.md) or [spin degeneracy](../../../../spin-degeneracy.md), so these conventions must be stated rather than extracting an [energy](../../../../energy-split.md) from $N$ alone. Although the original text calls $\mathbf k$ [momentum](../../../../momentum-split.md), the supplied $\hbar^2k^2/(2m)$ dispersion makes it a [wave vector](../../../../wavevector.md); physical [momentum](../../../../momentum-split.md) is $\mathbf p=\hbar\mathbf k$. The result agrees with the constant [two-dimensional free-electron density of states](../../../../two-dimensional-free-electron-density-of-states.md). Discrete level spacings in a finite sample would require a specified boundary spectrum.

**One level occupied on average.** Write $\delta=\mu_BB$ and $z=e^{\beta(\varepsilon-\mu)}>0$. The two mean [spin](../../../../spin.md) occupations are

$$
N_+=\frac1{1+ze^{\beta\delta}},\qquad
N_-=\frac1{1+ze^{-\beta\delta}}.
$$

Imposing $N_++N_-=1$ gives $2+z(e^{\beta\delta}+e^{-\beta\delta})=1+z(e^{\beta\delta}+e^{-\beta\delta})+z^2$, hence $z^2=1$. Thus, for every positive [temperature](../../../../temperature-split.md),

$$
\boxed{\mu=\varepsilon,\qquad
N_+-N_-=-\tanh\left(\frac{\beta\mu_BB}{2}\right).}
$$

The total [magnetic moment](../../../../magnetic-dipole-moment.md) is $\mathcal M=-\mu_B(N_+-N_-)$. Consequently

$$
\boxed{\chi=\left(\frac{\partial\mathcal M}{\partial B}\right)_{B=0}
=\frac{\mu_B^2}{2k_BT}.}
$$

This is the [grand-canonical spin susceptibility of a half-filled single level](../../../../grand-canonical-spin-susceptibility-of-a-half-filled-single-level.md). Empty, singly occupied and doubly occupied orbital states are allowed in the [grand canonical ensemble](../../../../grand-canonical-ensemble.md). At zero field, the singly occupied configurations together have [probability](../../../../probability.md) $1/2$, explaining the factor of two relative to one permanent spin-half moment. If exactly one [electron](../../../../electron.md) were required at all times, a canonical two-state [partition function](../../../../canonical-partition-function.md) would instead give $\mathcal M=\mu_B\tanh(\beta\mu_BB)$ and $\chi=\mu_B^2/(k_BT)$. That different answer does not implement the stated average-number [constraint](../../../../constraint-mechanics.md).

**Density-of-states formula for the susceptibility.** Here $g$ is the zero-field [single-spin density of states](../../../../single-spin-density-of-states.md). Regard its argument $E$ as the full spin-shifted [energy](../../../../energy-split.md). The shifted functions are $g_\pm(E)=g(E\mp\mu_BB)$, so

$$
N_\pm(B)=\int_{-\infty}^{\infty}g(E\mp\mu_BB)n(E;\mu(B),T)\,dE.
$$

The total number is even in $B$; thus $\mu(B)=\mu(0)+O(B^2)$ at fixed total number on a smooth branch. More directly, terms from $\mu'(0)$ cancel in the [spin](../../../../spin.md) difference because the two densities coincide at zero field. To first order,

$$
N_+-N_-=-2\mu_BB\int_{-\infty}^{\infty}g'(E)n(E;\mu(0),T)\,dE+O(B^3).
$$

It follows that

$$
\boxed{\chi=2\mu_B^2\int_{-\infty}^{\infty}g'(E)n(E)_{B=0}\,dE.}
$$

For a physical [energy band](../../../../energy-band.md), take $g$ to vanish below its lower edge. Provided the endpoint term vanishes, [integration by parts](../../../../integration-by-parts.md) also gives

$$
\boxed{\frac\chi{2\mu_B^2}=\int_{-\infty}^{\infty}g(E)[-n'(E)]\,dE.}
$$

This form displays the positive response and the narrow thermal window around $\mu$. A sharp band edge is included by the corresponding distributional [derivative](../../../../derivative.md) in the first expression. The susceptibility defined here is the [derivative](../../../../derivative.md) of total [magnetic moment](../../../../magnetic-dipole-moment.md) with respect to $B$, with units $\mathrm{J\,T^{-2}}$; it is not automatically a dimensionless SI [volume](../../../../volume-thermodynamics.md) susceptibility. A density-of-states convention per unit [volume](../../../../volume-thermodynamics.md) likewise gives a response per unit [volume](../../../../volume-thermodynamics.md). These are the [field conventions for magnetic susceptibility](../../../../field-conventions-for-magnetic-susceptibility.md).

**[Chemical potential](../../../../chemical-potential-split.md) at fixed number.** Define the integrated single-spin state count

$$
G(E)=\int_{-\infty}^E g(u)\,du,
\qquad K_T(E)=-n'(E).
$$

The [probability](../../../../probability.md) kernel $K_T$ has unit [integral](../../../../integral-split.md), mean $\mu$, and [variance](../../../../variance-split.md) $a(k_BT)^2$. Using [integration by parts](../../../../integration-by-parts.md),

$$
\frac N2=\int g(E)n(E)\,dE=\int G(E)K_T(E)\,dE.
$$

Expand $G$ about $\mu$. The linear term integrates to zero, while $G''=g'$ gives

$$
\frac N2=G(\mu)+\frac a2(k_BT)^2g'(\mu)+O(T^4).
$$

This is the number form of the [Sommerfeld expansion](../../../../sommerfeld-expansion.md). Since $N/2=G(\varepsilon_F)$ at zero [temperature](../../../../temperature-split.md), set $\mu=\varepsilon_F+\delta\mu$ with $\delta\mu=O(T^2)$:

$$
0=g(\varepsilon_F)\delta\mu+\frac a2(k_BT)^2g'(\varepsilon_F)+O(T^4).
$$

Therefore

$$
\boxed{\mu=\varepsilon_F-\frac a2\frac{g'(\varepsilon_F)}{g(\varepsilon_F)}(k_BT)^2+O(T^4).}
$$

The coefficient can be obtained directly. With $y=(E-\mu)/(k_BT)$,

$$
a=\int_{-\infty}^{\infty}\frac{y^2e^y}{(1+e^y)^2}dy
=4\sum_{\ell=1}^{\infty}\frac{(-1)^{\ell+1}}{\ell^2}
=\boxed{\frac{\pi^2}{3}}.
$$

For example, the sum follows by expanding $e^{-y}/(1+e^{-y})^2$ on $y>0$, using the evenness of the kernel and integrating each exponential. Thus $a/2=\pi^2/6$. A [density of states](../../../../density-of-states.md) increasing with [energy](../../../../energy-split.md) gives a downward quadratic chemical-potential shift. For the constant two-dimensional [density of states](../../../../density-of-states.md) that shift vanishes to this order; a finite lower band edge still allows exponentially small corrections.

**Low-temperature susceptibility at fixed number.** Apply the same kernel expansion to $g$ itself:

$$
\frac\chi{2\mu_B^2}
=g(\mu)+\frac a2(k_BT)^2g''(\mu)+O(T^4).
$$

The shift of $\mu$ must be retained in the first term. Writing $g_F=g(\varepsilon_F)$ and similarly for its [derivatives](../../../../derivative.md),

$$
g(\mu)=g_F+g_F'\delta\mu+O(T^4)
=g_F-\frac a2\frac{g_F'^2}{g_F}(k_BT)^2+O(T^4).
$$

Consequently

$$
\boxed{\frac\chi{2\mu_B^2}
=g_F-\frac a2\left(\frac{g_F'^2}{g_F}-g_F''\right)(k_BT)^2+O(T^4),
\qquad a=\frac{\pi^2}{3}.}
$$

This is the [fixed-number low-temperature Pauli susceptibility](../../../../fixed-number-low-temperature-pauli-susceptibility.md). The $g_F''$ contribution is thermal broadening at fixed [chemical potential](../../../../chemical-potential-split.md); the $-g_F'^2/g_F$ contribution enforces fixed total number. Both are needed. If the [density of states](../../../../density-of-states.md) were instead defined with both [spin](../../../../spin.md) directions included, the prefactor $2$ would be absorbed into that definition. Only the [spin](../../../../spin.md) response has been calculated; no orbital magnetic response is included.

The expansion assumes $g_F>0$, sufficient smoothness near the [Fermi energy](../../../../fermi-energy.md), and a [temperature](../../../../temperature-split.md) small compared with the [energy](../../../../energy-split.md) scale over which $g$ changes or encounters a band edge. It does not apply unmodified at a singular [density of states](../../../../density-of-states.md). For the ideal two-dimensional parabolic band, $g_F'=g_F''=0$, so the leading Pauli response is [temperature](../../../../temperature-split.md) independent, consistently with the earlier state count.

## ↑ Ancestors (13)

1. [6](../6.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
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
