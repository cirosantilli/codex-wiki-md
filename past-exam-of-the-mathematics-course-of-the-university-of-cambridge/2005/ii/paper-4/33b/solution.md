<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

In the nondegenerate regime, $\mu$ lies well inside the gap, with $\mu\gg kT$ and $E_g-\mu\gg kT$. Then conduction occupations are approximately $e^{(\mu-E)/(kT)}$, while the hole [probability](../../../../../probability.md) in a valence state is approximately $e^{(E-\mu)/(kT)}$. Using the near-edge [density of states](../../../../../density-of-states.md) and the supplied [Gamma integral](../../../../../gamma-integral.md) gives

$$
n=N_ce^{(\mu-E_g)/(kT)},\qquad
p=N_ve^{-\mu/(kT)},\qquad
N_{c,v}=\frac{\sqrt\pi}{2}A_{c,v}(kT)^{3/2}.
$$

Therefore

$$
\boxed{np=N_cN_ve^{-E_g/(kT)}}.
$$

This assumes the edge approximations are valid over the thermally populated ranges. For an intrinsic [semiconductor](../../../../../semiconductor.md) $n=p$, so each carrier density is proportional to $T^{3/2}e^{-E_g/(2kT)}$. Both mobile conduction [Electrons](../../../../../electron.md) and holes contribute to conductivity, $\sigma=|e|(nb_e+pb_h)$ with mobilities $b_e,b_h$. The exponentially varying carrier densities explain strong temperature dependence even when the mobilities vary only algebraically.

Donors supply [Electrons](../../../../../electron.md) and acceptors remove [Electrons](../../../../../electron.md) to create holes. With complete ionization and negligible minority carriers, the majority densities are $n\simeq N_d$ on the n side and $p\simeq N_a$ on the p side. The corresponding isolated [chemical potentials](../../../../../chemical-potential.md) are

$$
\mu_n=E_g+kT\log(N_d/N_c),\qquad
\mu_p=kT\log(N_v/N_a).
$$

Carrier diffusion at contact leaves positively charged donors and negatively charged acceptors in a depletion layer. At equilibrium the electrochemical potential is constant; the [Electron](../../../../../electron.md) [energy](../../../../../energy.md) shift is $-|e|\phi$. Hence the n-minus-p electric potential is

$$
\boxed{V_{np}=\frac{\mu_n-\mu_p}{|e|}
=\frac1{|e|}\left[E_g-kT\log\frac{N_vN_c}{N_dN_a}\right]}.
$$

All $N$ quantities must have a consistent normalization: if $N_c,N_v$ are state densities per volume, $N_d,N_a$ are dopant densities rather than bare atom counts. The formula neglects incomplete ionization, degeneracy and changes in band structure.

At a common temperature the two equilibrium junction/contact effects do not drive a perpetual current. At different junction temperatures, [Electrons](../../../../../electron.md) and holes transport [entropy](../../../../../entropy.md) differently, giving different [Seebeck coefficients](../../../../../seebeck-coefficient.md) on the two sides. The loop has a thermoelectric electromotive force, oriented as $\int_{T_1}^{T_2}(S_n-S_p)\,dT$, and therefore generally carries current when closed. This is the [Seebeck effect](../../../../../seebeck-effect.md): [energy](../../../../../energy.md) is supplied by heat flow from hot to cold. The temperature dependence of the junction barrier is useful intuition, but an exact terminal voltage is not obtained simply by subtracting two equilibrium built-in potentials; it also depends on bulk transport and contact conditions. The given equilibrium density-of-states data do not determine the numerical thermopowers.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
