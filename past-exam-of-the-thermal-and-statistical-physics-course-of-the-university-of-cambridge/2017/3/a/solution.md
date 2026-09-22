<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Component chemical potentials.** Define the per-spin [quantum concentration](../../../../quantum-concentration.md) $n_Q=\lambda_T^{-3}=(mk_BT/(2\pi\hbar^2))^{3/2}$. For a classical component with one-particle [potential energy](../../../../potential-energy.md) $U_\sigma(\mathbf r)$, the local [Helmholtz free energy](../../../../helmholtz-free-energy.md) density is $k_BTn_\sigma[\ln(n_\sigma/n_Q)-1]+n_\sigma U_\sigma$. Its derivative with respect to [number density](../../../../number-density.md) gives the full local [chemical potential](../../../../chemical-potential-split.md), including the magnetic [energy](../../../../energy-split.md). With the up state defined as the lower level,

$$
\boxed{\mu_\uparrow=k_BT\ln\frac{n_\uparrow}{n_Q}-\mu_BB,
\qquad
\mu_\downarrow=k_BT\ln\frac{n_\downarrow}{n_Q}+\mu_BB.}
$$

The [Bohr magneton](../../../../bohr-magneton.md) $\mu_B$ is a [magnetic moment](../../../../magnetic-dipole-moment.md); $\mu_BB$ is an [energy](../../../../energy-split.md). The factor two for the two spin states is not already included in $n_Q$.

**Total equilibrium chemical potential.** If spin conversion is allowed, a particle can be added in either spin state at the same equilibrium free-[energy](../../../../energy-split.md) cost. Thus

$$
\boxed{\mu=\mu_\uparrow=\mu_\downarrow,}
$$

not their sum or zero. The total [particle number](../../../../particle-number.md), or a reservoir, fixes this common value; the supplied information does not specify a numerical [chemical potential](../../../../chemical-potential-split.md). A useful local expression is $\mu=k_BT\ln[n/(2n_Q\cosh x)]$, with $x=\mu_BB/(k_BT)$, whose density dependence is found below.

**Why it is uniform and common.** Moving a small number $dN$ of one species from $\mathbf r_1$ to $\mathbf r_2$ changes the [free energy](../../../../thermodynamic-free-energy.md) by $[\mu_\sigma(\mathbf r_2)-\mu_\sigma(\mathbf r_1)]dN$. If this difference were nonzero, a transfer could lower the [free energy](../../../../thermodynamic-free-energy.md). Equilibrium under diffusion therefore requires each full [chemical potential](../../../../chemical-potential-split.md) to be spatially constant. A spin flip transferring $dN$ from down to up similarly changes [free energy](../../../../thermodynamic-free-energy.md) by $(\mu_\uparrow-\mu_\downarrow)dN$, proving equality when spin relaxation is permitted. This is [chemical equilibrium of a classical spin gas](../../../../chemical-equilibrium-of-a-classical-spin-gas.md). Mere thermal contact at fixed separate spin populations would not enforce the latter equality; full spin equilibrium is the necessary assumption. A spatially varying [magnetic field](../../../../magnetic-field-split.md) is balanced by a spatially varying density, not by a varying full [chemical potential](../../../../chemical-potential-split.md).

**Magnetization.** Invert the component equations at the common $\mu$:

$$
n_\uparrow(\mathbf r)=n_Qe^{\beta\mu}e^{x(\mathbf r)},\qquad
n_\downarrow(\mathbf r)=n_Qe^{\beta\mu}e^{-x(\mathbf r)}.
$$

The two levels have moments $+\mu_B$ and $-\mu_B$ along the field. The [magnetization](../../../../magnetization.md), [magnetic moment](../../../../magnetic-dipole-moment.md) per unit [volume](../../../../volume.md), is therefore

$$
\boxed{M(\mathbf r)=\mu_B(n_\uparrow-n_\downarrow)
=2\mu_Bn_Qe^{\beta\mu}\sinh x(\mathbf r).}
$$

Its SI units are $\mathrm{A\,m^{-1}}$. This expression neglects interactions and magnetic feedback of the gas on the specified external field.

**High-temperature response.** For $|x|\ll1$, $\sinh x\simeq x$ and $\cosh x\simeq1$, yielding

$$
\boxed{M(\mathbf r)\simeq
\frac{2\mu_B^2 n_Qe^{\beta\mu}}{k_BT}B(\mathbf r)
\simeq\frac{n(\mathbf r)\mu_B^2}{k_BT}B(\mathbf r).}
$$

At fixed [number density](../../../../number-density.md), this is the [Curie law](../../../../curie-s-law.md): the susceptibility with respect to $B$ is $n\mu_B^2/(k_BT)$. The conventional dimensionless susceptibility with respect to $H$ is approximately $\chi_v=\mu_0n\mu_B^2/(k_BT)$ when $B\simeq\mu_0H$. At fixed $\mu$, however, $n_Qe^{\beta\mu}$ changes with [temperature](../../../../temperature-split.md), so $M$ itself need not scale simply as $1/T$. The moment per particle has the Curie behaviour; the density constraint must be stated.

**Total density.** Adding the two populations gives

$$
\boxed{n(\mathbf r)=2n_Qe^{\beta\mu}\cosh x(\mathbf r),\qquad
\frac{M(\mathbf r)}{n(\mathbf r)}=\mu_B\tanh x(\mathbf r).}
$$

For a finite container and fixed $N$, normalization gives $e^{\beta\mu}=N/[2n_Q\int\cosh x(\mathbf r)\,d^3r]$. In a weak field the leading density is uniform, with changes only of order $x^2$. Particles preferentially occupy regions where the magnitude of the field lowers one of the spin energies, even though the common [chemical potential](../../../../chemical-potential-split.md) remains uniform.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
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
