<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Ensemble and applications.** A [grand canonical ensemble](../../../../grand-canonical-ensemble.md) describes a system exchanging both [energy](../../../../energy-split.md) and particles with a large reservoir. Its fixed control parameters are $T,V,\mu$, while microstates with different $N$ have [probabilities](../../../../probability.md)

$$
P_r=\Xi^{-1}e^{-\beta(E_r-\mu N_r)},\qquad
\Xi=\sum_r e^{-\beta(E_r-\mu N_r)}.
$$

Weak coupling allows the system's [energy](../../../../energy-split.md) levels to remain meaningful; equilibrium fixes the reservoir [temperature](../../../../temperature-split.md) and [chemical potential](../../../../chemical-potential-split.md). The [grand potential](../../../../grand-potential.md) is $\Phi=-k_BT\ln\Xi=U-TS-\mu N$, with $N$ now the mean population. It generates [entropy](../../../../entropy-split.md), [pressure](../../../../pressure-split.md) and mean [particle number](../../../../particle-number.md) by differentiation. This ensemble is convenient for gases in contact with particle reservoirs, independently occupied quantum levels and surface [adsorption](../../../../adsorption.md); its particle-number fluctuations are part of the description, not an error in counting.

**Classical single-level limit.** For the [single-level grand partition function in the dilute limit](../../../../single-level-grand-partition-function-in-the-dilute-limit.md), put $x_k=e^{-\beta(\epsilon_k-\mu)}$. Empty and singly occupied levels contribute $1$ and $x_k$. In the dilute classical limit $x_k\ll1$, higher occupancies contribute only at order $x_k^2$ or beyond:

$$
\boxed{\Xi_k=1+x_k+O(x_k^2)
\simeq1+\exp[-(\epsilon_k-\mu)/(k_BT)]}.
$$

This truncation does not impose the Pauli principle on a classical gas. A [fermion](../../../../fermion.md) state has exactly $1+x_k$, a [boson](../../../../boson.md) state has $(1-x_k)^{-1}$, and Maxwell-Boltzmann occupancy weights give $e^{x_k}$; they all agree to this order. In particular, $\ln\Xi_k=x_k+O(x_k^2)$, with the classical Maxwell-Boltzmann result exactly $x_k$.

**[grand potential](../../../../grand-potential.md) and [chemical potential](../../../../chemical-potential-split.md).** With $z=e^{\beta\mu}$, summing the single-level [logarithms](../../../../logarithm.md) and using the stated [density of states](../../../../density-of-states.md) gives

$$
\ln\Xi\simeq z\int_0^\infty g(\epsilon)e^{-\beta\epsilon}\,d\epsilon.
$$

Substitute $\epsilon=k_BTx^2$, for which

$$
\int_0^\infty\epsilon^{1/2}e^{-\beta\epsilon}\,d\epsilon
=2(k_BT)^{3/2}\int_0^\infty x^2e^{-x^2}dx
=\frac{\sqrt\pi}{2}(k_BT)^{3/2}.
$$

Combining this with the density-of-states prefactor gives $\ln\Xi=zV/\lambda^3$. Thus

$$
\boxed{\Phi=-k_BT\frac V{\lambda^3}e^{\mu/(k_BT)}}.
$$

Differentiating at fixed $T,V$,

$$
N=-\left(\frac{\partial\Phi}{\partial\mu}\right)_{T,V}
=\frac V{\lambda^3}e^{\mu/(k_BT)},
\qquad
\boxed{\mu=k_BT\ln\frac{N\lambda^3}{V}}.
$$

Similarly $p=-(\partial_V\Phi)_{T,\mu}=k_BTz/\lambda^3$, so $pV=Nk_BT$. This is the [grand-canonical chemical potential of a classical ideal gas](../../../../grand-canonical-chemical-potential-of-a-classical-ideal-gas.md). The condition $N\lambda^3/V\ll1$ states the classical regime. The supplied [density of states](../../../../density-of-states.md) counts one internal state; extra internal degeneracies would have to be included consistently rather than inserted at only one stage.

**One [adsorption](../../../../adsorption.md) site.** Take the free-vapour [energy](../../../../energy-split.md) reference as zero and the [binding energy](../../../../binding-energy.md) as $-\epsilon$. A site is either empty or singly occupied; the latter has vibrational [partition function](../../../../canonical-partition-function.md) $z_s(T)$. Its [adsorption-site grand partition function](../../../../adsorption-site-grand-partition-function.md) and mean occupation are

$$
\Xi_{\rm site}=1+z_s e^{\beta(\mu_s+\epsilon)},\qquad
\theta=\frac{z_s e^{\beta(\mu_s+\epsilon)}}
{1+z_s e^{\beta(\mu_s+\epsilon)}}.
$$

The [chemical potential of an adsorbed species on equivalent sites](../../../../chemical-potential-of-an-adsorbed-species-on-equivalent-sites.md) follows by inverting the occupation ratio

$$
\boxed{\mu_s=-\epsilon+k_BT\ln\frac{\theta}{(1-\theta)z_s}}.
$$

The factor $1-\theta$ is the vacant-site probability. The binding reference and the [energies](../../../../energy-split.md) included in $z_s$ must be chosen consistently, so that vibrational [zero-point energy](../../../../zero-point-energy.md) is not counted twice.

**Isotherm.** The [vibrational factor in a Langmuir equilibrium constant](../../../../vibrational-factor-in-a-langmuir-equilibrium-constant.md) is fixed by [adsorption](../../../../adsorption.md) equilibrium, $\mu_s=\mu_{\rm vap}$. Neglecting vapour internal degrees of freedom and writing its [number density](../../../../number-density.md) as $p/(k_BT)$ gives $e^{\beta\mu_{\rm vap}}=p\lambda^3/(k_BT)$. Therefore

$$
b_s(T)=\frac{z_s(T)\lambda^3}{k_BT}e^{\epsilon/(k_BT)},\qquad
\boxed{\theta(p,T)=\frac{b_s(T)p}{1+b_s(T)p}}.
$$

This is the [Langmuir isotherm](../../../../langmuir-adsorption-model.md): initially linear, increasing monotonically and concave down, approaching unit coverage. Half coverage occurs at $p_{1/2}=1/b_s(T)$. The coefficient has inverse-pressure units. It assumes equivalent independent sites, at most one [molecule](../../../../molecule-split.md) per site and no lateral interaction or multilayer [adsorption](../../../../adsorption.md). The molecular mass appropriate to the vapour determines $\lambda$.

<a id="3/image-original-dimensionless-langmuir-coverage-curve-with-half-coverage-and-limiting-behavior"></a>
![](../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1-adsorption-isotherm.png)

**[Figure 2](#3/image-original-dimensionless-langmuir-coverage-curve-with-half-coverage-and-limiting-behavior). Original dimensionless Langmuir coverage curve with half-coverage and limiting behavior**.

A real uptake measurement must separate adsorbed [molecules](../../../../molecule-split.md) from free gas in the apparatus. Langmuir's original mica experiment compared a mica-containing bulb with a similar blank and inferred uptake from calibrated gas [volumes](../../../../volume.md) and [pressures](../../../../pressure-split.md). His stated blank contribution and bath-temperature drift limited the inferred [adsorption](../../../../adsorption.md); a saturating curve alone does not establish ideal equivalent sites.[pp. 1376–1378: mica apparatus and blank; p. 1385: limitations](../../../../the-adsorption-of-gases-on-plane-surfaces-of-glass-mica-and-platinum-by-irving-langmuir.md)

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
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
