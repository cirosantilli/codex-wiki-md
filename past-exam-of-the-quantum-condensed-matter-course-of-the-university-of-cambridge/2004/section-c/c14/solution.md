<h1 id="section-c/c14/solution">Solution</h1>

↑ **Parent:** [C14](../c14.md)

[Semiconductor doping](../../../../semiconductor-doping.md) introduces electrically active impurities. In [gallium arsenide](../../../../gallium-arsenide.md), [silicon](../../../../silicon.md) has one more valence [electron](../../../../electron.md) than [gallium](../../../../gallium.md) but one fewer than [arsenic](../../../../arsenic.md). [Silicon](../../../../silicon.md) on a [gallium](../../../../gallium.md) site can therefore supply a shallow donor [electron](../../../../electron.md), while [silicon](../../../../silicon.md) on an [arsenic](../../../../arsenic.md) site can accept an [electron](../../../../electron.md) and leave a mobile hole. It is an [amphoteric dopant](../../../../amphoteric-dopant.md), so its net effect depends on site occupation and growth conditions.[1999 abstract: neutral and ionized donors on Ga sites and acceptors on As sites](../../../../thermal-equilibrium-concentrations-of-the-amphoteric-dopant-si-and-the-associated-carrier-concentrations-in-gaas-by-chang-ho-chen-and-others.md)

For isotropic parabolic bands, shift the [energy](../../../../energy-split.md) origin in the given free-electron [density of states](../../../../density-of-states.md) to the appropriate band edge and use its effective [mass](../../../../mass.md):

$$
\boxed{g_c(E)=\frac1{2\pi^2}\left(\frac{2m_e}{\hbar^2}\right)^{3/2}\sqrt{E-\epsilon_c},\quad E\geq\epsilon_c,}
$$

and, for valence [electron](../../../../electron.md) states,

$$
\boxed{g_v(E)=\frac1{2\pi^2}\left(\frac{2m_h}{\hbar^2}\right)^{3/2}\sqrt{\epsilon_v-E},\quad E\leq\epsilon_v.}
$$

The stated normalization includes the two [spin](../../../../spin.md) states and assumes one effective valley. In a nondegenerate semiconductor, the conduction occupation is approximately $e^{-(E-\mu)/(k_BT)}$ and the probability of a valence hole is approximately $e^{(E-\mu)/(k_BT)}$. Substituting $x=(E-\epsilon_c)/(k_BT)$ in the first integral, and the corresponding hole [energy](../../../../energy-split.md) in the second, gives

$$
n=N_ce^{-(\epsilon_c-\mu)/(k_BT)},\qquad p=N_ve^{-(\mu-\epsilon_v)/(k_BT)},
$$

where the [effective density of states](../../../../effective-density-of-states.md) values are $N_c=2[m_ek_BT/(2\pi\hbar^2)]^{3/2}$ and $N_v=2[m_hk_BT/(2\pi\hbar^2)]^{3/2}$. The factor $\sqrt\pi/2$ comes from the supplied Gaussian-weighted integral. Multiplying cancels the shared [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md) [chemical potential](../../../../chemical-potential-split.md) and proves the [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md):

$$
\boxed{np=N_cN_ve^{-E_g/(k_BT)}=4\left(\frac{k_BT}{2\pi\hbar^2}\right)^3(m_em_h)^{3/2}e^{-E_g/(k_BT)}.}
$$

For the given sample $N_D=2\times10^{21}\,\mathrm{m^{-3}}$ and $N_A=10^{21}\,\mathrm{m^{-3}}$. With complete donor ionization and occupied acceptors, [charge neutrality](../../../../charge-neutrality.md) gives $n-p=N_D-N_A=10^{21}\,\mathrm{m^{-3}}$. At $293\,\mathrm K$ the given masses and gap give

$$
N_c\simeq3.92\times10^{23}\,\mathrm{m^{-3}},\quad N_v\simeq8.56\times10^{24}\,\mathrm{m^{-3}},\quad n_i^2\simeq1.26\times10^{24}\,\mathrm{m^{-6}}.
$$

Solving the [compensated semiconductor](../../../../compensated-semiconductor.md) equations, or using $n_i\ll N_D-N_A$, yields

$$
\boxed{n\simeq1.00\times10^{21}\,\mathrm{m^{-3}},\qquad p=\frac{n_i^2}{n}\simeq1.26\times10^3\,\mathrm{m^{-3}}.}
$$

The very small minority density is consistent with the wide gap and the strongly n-type balance. Also $n/N_c\simeq2.6\times10^{-3}\ll1$ and $p/N_v\ll1$, checking the nondegenerate approximation. The acceptor levels are occupied in this n-type regime; complete acceptor ionization in the compensation equation is appropriate to the model.

At low [temperature](../../../../temperature-split.md) [dopant freeze-out](../../../../dopant-freeze-out.md) reduces the conduction-electron population; a quantitative curve would require dopant binding energies and occupation factors. Once donors are ionized while intrinsic excitation is negligible, $n\simeq N_D-N_A$ gives an extrinsic plateau. At higher [temperature](../../../../temperature-split.md) intrinsic pairs eventually dominate, so $n\simeq p\simeq n_i(T)\propto T^{3/2}e^{-E_g/(2k_BT)}$ if the gap and masses are treated as constant. Real gap and [mass](../../../../mass.md) changes modify that last expression.

## ↑ Ancestors (13)

1. [C14](../c14.md)
2. [Section C](../../section-c.md)
3. [2004](../../../2004-split.md)
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
