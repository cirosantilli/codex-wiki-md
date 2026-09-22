# Chemical potential

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_potential)

The [chemical potential](chemical-potential.md) measures how a [thermodynamic potential](thermodynamic-potential.md) changes when matter is added under specified constraints. It plays for matter exchange the role that [temperature](temperature.md) plays for [heat](heat.md) exchange: a difference supplies a direction, and equality characterizes [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium) when the corresponding exchange is allowed. This connects [diffusion](thermodynamics.md#diffusion), [phase coexistence](critical-phenomenon.md#phase-coexistence) and [chemical equilibrium](#chemical-equilibrium) through one quantity.

For a single component, the particle convention is

$$
\mu_{\rm particle}=\left(\frac{\partial U}{\partial N}\right)_{S,V},
$$

where $U$ is [internal energy](internal-energy.md), $N$ counts particles, $S$ is [entropy](entropy.md) and $V$ is [volume](thermodynamics.md#volume-thermodynamics). This [partial derivative](multivariable-calculus.md#partial-derivative) holds [entropy](entropy.md) and [volume](thermodynamics.md#volume-thermodynamics) fixed; it measures an incremental change rather than the average [energy](energy.md) per particle. See [David Tong, Statistical Physics, section 1.4](https://davidtong.org/pdfs/teaching/statistical-physics/statphys1.pdf).

In [chemistry](chemistry.md) the molar convention instead uses [amount of substance](physics.md#amount-of-substance) $n$, measured in [moles](physics.md#mole-unit):

$$
\mu_{\rm m}=\left(\frac{\partial G}{\partial n}\right)_{T,p},
\qquad n=\frac{N}{N_{\rm A}},
\qquad \mu_{\rm m}=N_{\rm A}\mu_{\rm particle}.
$$

Here $G$ is [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy), $T$ is [temperature](temperature.md), $p$ is [pressure](pressure.md) and $N_{\rm A}$ is the [Avogadro constant](physics.md#avogadro-constant). The units are $\mathrm J$ per particle versus $\mathrm{J\,mol^{-1}}$. For several [chemical species](mathematical-biology.md#chemical-species), define each [chemical potential](chemical-potential.md) by varying only its own particle count or [amount of substance](physics.md#amount-of-substance), with all other components' counts or amounts fixed. Many texts use $\mu$ for either convention, so the units and the variable being differentiated must identify it.

For a [simple compressible system](thermodynamics.md#simple-compressible-system) with variable component inventories, the fundamental differentials are

$$
dU=T\,dS-p\,dV+\sum_i\mu_{{\rm particle},i}\,dN_i,
\qquad
dG=-S\,dT+V\,dp+\sum_i\mu_{{\rm m},i}\,dn_i.
$$

They describe changes between states in [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium) with only [pressure](pressure.md)-[volume](thermodynamics.md#volume-thermodynamics) [work](energy.md#work). If every component inventory is fixed, the sums vanish. The [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) form follows by differentiating $G=U-TS+pV$ and using $dN_i=N_{\rm A}\,dn_i$; this is why the two definitions describe the same [chemical potential](chemical-potential.md) in different units.

A [chemical potential](chemical-potential.md) can be negative. Holding [entropy](entropy.md) fixed while adding matter need not increase [internal energy](internal-energy.md); Tong explains this explicitly for a classical [ideal gas](ideal-gas.md) in [Statistical Physics, section 2.2.4](https://davidtong.org/pdfs/teaching/statistical-physics/statphys2.pdf). Its absolute sign also depends on the reference [energy](energy.md): replacing $U$ by $U+\epsilon_0N$ shifts $\mu_{\rm particle}$ by $\epsilon_0$. A common reference shift cancels from differences for the same [chemical species](mathematical-biology.md#chemical-species), which are what determine exchange. Thus “energy cost” means a signed increment, not an always positive amount that must be supplied.

**Table of contents**

- [Water activity](#water-activity)
- [Standard chemical potential](#standard-chemical-potential)
- [Grand-canonical chemical potential of a classical ideal gas](#grand-canonical-chemical-potential-of-a-classical-ideal-gas)
- [Quasi-Fermi level](#quasi-fermi-level)
  - [Quasi-Fermi-level splitting](#quasi-fermi-level-splitting)
- [Chemical potential equality for particle exchange](#chemical-potential-equality-for-particle-exchange)
  - [Open-system equilibrium contacts](#open-system-equilibrium-contacts)
  - [Chemical potential and Helmholtz free energy](#chemical-potential-and-helmholtz-free-energy)
- [Chemical potential of an ideal gas](#chemical-potential-of-an-ideal-gas)
- [Electrochemical potential](#electrochemical-potential)
  - [Electrochemical gradient](#electrochemical-gradient)
    - [Proton-motive force](#proton-motive-force)
- [Chemical potential of a composition field](#chemical-potential-of-a-composition-field)
- [Chemical equilibrium](#chemical-equilibrium)
  - [Number-based dissociation equilibrium ratio](#number-based-dissociation-equilibrium-ratio)
  - [Reaction formula-unit conservation](#reaction-formula-unit-conservation)
    - [Dissociation fraction versus conserved density](#dissociation-fraction-versus-conserved-density)
  - [Ionic product of water](#ionic-product-of-water)
  - [Dimerization](#dimerization)
  - [Ocean carbonate chemistry](#ocean-carbonate-chemistry)
    - [Carbonate compensation](#carbonate-compensation)
  - [Van't Hoff equation](#van-t-hoff-equation)
  - [Standard entropy of reaction](#standard-entropy-of-reaction)
  - [Gibbs energy of reaction](#gibbs-energy-of-reaction)
    - [Standard Gibbs energy of reaction](#standard-gibbs-energy-of-reaction)
  - [Chemical equilibrium of a classical spin gas](#chemical-equilibrium-of-a-classical-spin-gas)
  - [Chemical disequilibrium](#chemical-disequilibrium)
  - [Zero chemical potential from number-changing reactions](#zero-chemical-potential-from-number-changing-reactions)
  - [Chemical relaxation time](#chemical-relaxation-time)
  - [Equilibrium constant](#equilibrium-constant)
    - [Dimensionless concentration equilibrium constant](#dimensionless-concentration-equilibrium-constant)
    - [Association constant](#association-constant)
    - [Dissociation constant](#dissociation-constant)
  - [Standard state](#standard-state)
    - [Standard pressure](#standard-pressure)
    - [Standard concentration](#standard-concentration)
    - [Thermodynamic activity](#thermodynamic-activity)
      - [Chemical fugacity](#chemical-fugacity)
      - [Activity coefficient](#activity-coefficient)
  - [Reaction quotient](#reaction-quotient)
  - [Photon chemical potential](#photon-chemical-potential)

## Water activity

↑ **Parent:** [Chemical potential](chemical-potential.md)

Water activity measures the chemical potential of water relative to a chosen pure-water standard state. Under ideal-vapour conditions above a flat solution, it is the equilibrium vapour pressure divided by that above pure liquid water at the same temperature. Dissolved solute usually lowers activity. [Raoult's law](mixture.md#raoult-s-law) gives the ideal dilute-solution limit; nonideal interactions require an activity model.

## Standard chemical potential

↑ **Parent:** [Chemical potential](chemical-potential.md)

The [chemical potential](chemical-potential.md) assigned to a specified [standard state](#standard-state). With dimensionless [thermodynamic activity](#thermodynamic-activity) $a$, the per-particle convention is $\mu=\mu^\circ+k_BT\ln a$; a molar convention uses $RT$. The [standard state](#standard-state) changes both $\mu^\circ$ and the activity definition without changing observable [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system).

## Grand-canonical chemical potential of a classical ideal gas

↑ **Parent:** [Chemical potential](chemical-potential.md)

For one internal species, the [grand canonical partition function](statistical-physics.md#grand-canonical-partition-function) of a classical [ideal gas](ideal-gas.md) satisfies $\ln\Xi=zV/\lambda^3$, with [quantum gas fugacity](statistical-physics.md#fugacity-statistical-mechanics) $z=e^{\beta\mu}$ and [thermal de Broglie wavelength](canonical-ensemble.md#thermal-de-broglie-wavelength) $\lambda=\sqrt{2\pi\hbar^2/(mk_BT)}$. Differentiating the [grand potential](statistical-physics.md#grand-potential) gives $N=zV/\lambda^3$, hence $\mu=k_BT\ln(n\lambda^3)$. An internal partition factor must be included consistently if internal states are available.

## Quasi-Fermi level

↑ **Parent:** [Chemical potential](chemical-potential.md)

A [quasi-Fermi level](#quasi-fermi-level) is a local electron or hole population parameter in a semiconductor driven out of equilibrium, assuming each population is internally close enough to thermal equilibrium to use a [Fermi-Dirac distribution](quantum-ideal-gas-statistics.md#fermi-dirac-distribution). Separate electron and hole parameters replace one common equilibrium [chemical potential](chemical-potential.md). Their spatial profiles depend on transport, generation and recombination as well as electrostatics. For ideal ohmic contacts with the p voltage $V$ relative to n, the contact electron [electrochemical potentials](#electrochemical-potential) obey $\mu_p-\mu_n=-eV$.

### Quasi-Fermi-level splitting

↑ **Parent:** [Quasi-Fermi level](#quasi-fermi-level)

The difference between electron and hole quasi-Fermi levels under nonequilibrium conditions. For ideal selective contacts their terminal separation sets $qV$; poor contacts can lose part of the internal splitting.

## Chemical potential equality for particle exchange

↑ **Parent:** [Chemical potential](chemical-potential.md)

Consider two internally equilibrated reservoirs A and B at the same imposed [temperature](temperature.md) and [pressure](pressure.md). They may have different compositions or represent different phases. Transfer a small positive [amount of substance](physics.md#amount-of-substance) $\delta n$ of the same [chemical species](mathematical-biology.md#chemical-species) from A to B, holding the other inventories fixed. To first order, their total [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) changes by

$$
\delta G_{\rm total}
=-\mu_{{\rm m},A}\delta n+\mu_{{\rm m},B}\delta n
=(\mu_{{\rm m},B}-\mu_{{\rm m},A})\delta n.
$$

Hence exchange toward lower [chemical potential](chemical-potential.md) lowers [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy). If transfer is allowed in both directions and the two reservoirs contain the exchangeable component, [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium) requires equal [chemical potentials](chemical-potential.md) for that component. See [MIT 5.60, Lecture 14, pages 1–2](https://ocw.mit.edu/courses/5-60-thermodynamics-kinetics-spring-2008/e763a06aa3b5de09cd6bfea6280f219c_5_60_lecture14.pdf).

An impermeable partition can maintain unequal [chemical potentials](chemical-potential.md); equality is a condition on an allowed exchange. Two pure samples of the same [ideal gas](ideal-gas.md) already have equal [chemical potentials](chemical-potential.md) at the same [temperature](temperature.md) and [pressure](pressure.md). Different compositions at a common [pressure](pressure.md) can instead give different [chemical potentials](chemical-potential.md) for one component through its [thermodynamic activity](#thermodynamic-activity).

Equality concerns the same exchangeable component in different places, not all different [chemical species](mathematical-biology.md#chemical-species). For a permitted [chemical reaction](chemical-reaction.md), the corresponding interior [chemical equilibrium](#chemical-equilibrium) criterion is $\sum_i\nu_i\mu_{{\rm m},i}=0$, with signed [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) entries $\nu_i$. The existing [chemical equilibrium](#chemical-equilibrium) and [constrained Gibbs minimization for chemical equilibrium](thermodynamic-potential.md#constrained-gibbs-minimization-for-chemical-equilibrium) sections develop those composition constraints.

### Open-system equilibrium contacts

↑ **Parent:** [Chemical potential equality for particle exchange](#chemical-potential-equality-for-particle-exchange)

Unconstrained thermal, mechanical and particle-exchange contacts require equality of [temperature](temperature.md), [pressure](pressure.md) and the [chemical potential](chemical-potential.md) of each exchangeable species. Walls, external fields, interfaces and chemical reactions change which variations are allowed.

### Chemical potential and Helmholtz free energy

↑ **Parent:** [Chemical potential equality for particle exchange](#chemical-potential-equality-for-particle-exchange)

Rigid compartments impose a different constraint: fixed [volume](thermodynamics.md#volume-thermodynamics) rather than fixed [pressure](pressure.md). With [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) $F=U-TS$,

$$
dF=-S\,dT-p\,dV+\sum_i\mu_{{\rm m},i}\,dn_i,
\qquad
\mu_{{\rm m},i}=\left(\frac{\partial F}{\partial n_i}\right)_{T,V,n_{j\ne i}}.
$$

This follows immediately by differentiating $F=U-TS$ in the [chemical potential](chemical-potential.md) differential above. It expresses the same [chemical potential](chemical-potential.md) through the [thermodynamic potential](thermodynamic-potential.md) appropriate to fixed [temperature](temperature.md) and [volume](thermodynamics.md#volume-thermodynamics).

Consider a [closed system](thermodynamics.md#closed-system) consisting of two rigid compartments of equal [volume](thermodynamics.md#volume-thermodynamics) $V$, maintained at a common fixed [temperature](temperature.md) $T$. A valve permits exchange of the same [ideal gas](ideal-gas.md); the partition stays in place. Initially $n_A=9\,\mathrm{mol}$ and $n_B=3\,\mathrm{mol}$, with conserved total [amount of substance](physics.md#amount-of-substance) $n_{\rm tot}=12\,\mathrm{mol}$. These are macroscopic [moles](physics.md#mole-unit), modeled continuously, not twelve individual particles. By the [ideal gas law](ideal-gas.md#ideal-gas-law), $p_B/p_A=n_B/n_A=1/3$, so initially

$$
\mu_{{\rm m},B}-\mu_{{\rm m},A}=-RT\ln3.
$$

At $300\,\mathrm K$ with the stipulated $R$, this is approximately $-2740.311\,\mathrm{J\,mol^{-1}}$, favoring transfer from A to B.

At fixed $T$ and equal $V$, integrating the ideal-gas [chemical potential](chemical-potential.md) gives the total [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy), up to a term independent of the allocation,

$$
F_{\rm total}
=RT\left[n_A\ln\frac{n_A}{n_{\rm ref}}+n_B\ln\frac{n_B}{n_{\rm ref}}-n_{\rm tot}\right]+C.
$$

Here $n_{\rm ref}$ is a positive reference [amount of substance](physics.md#amount-of-substance); any omitted common term linear in $n_A+n_B$ is constant along this exchange. Let $x=n_A/n_{\rm tot}$ be the [dimensionless](physics.md#dimensionless-quantity) fraction in A. The relative [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) then takes the particularly simple form

$$
\frac{F_{\rm total}(x)-F_{\rm total}(1/2)}{n_{\rm tot}RT}
=x\ln x+(1-x)\ln(1-x)+\ln2.
$$

Its [derivative](calculus.md#derivative) along the allowed transfer and its second [derivative](calculus.md#derivative) are

$$
\frac{dF_{\rm total}}{dn_A}
=\mu_{{\rm m},A}-\mu_{{\rm m},B}
=RT\ln\frac{x}{1-x},
\qquad
\frac{d^2F_{\rm total}}{dn_A^2}
=RT\left(\frac{1}{n_A}+\frac{1}{n_B}\right)>0.
$$

Thus the [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) is a strictly [convex function](real-analysis.md#convex-function) of the allocation for positive amounts. Its unique minimum has $x=1/2$, or $n_A=n_B=6\,\mathrm{mol}$, and equal [chemical potentials](chemical-potential.md). Initially its excess above this minimum is $n_{\rm tot}RT[\tfrac34\ln(3/2)+\tfrac14\ln(1/2)]\simeq3915.474\,\mathrm J$ at $300\,\mathrm K$. Relaxation decreases the total [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) by this amount in the model; the final [pressures](pressure.md) are also equal because both compartments have the same [volume](thermodynamics.md#volume-thermodynamics).

<a id="image-chemical-potential-differences-are-slopes-of-the-total-helmholtz-free-energy"></a>
![](chemical-potential-particle-transfer.png)

**[Figure 1](#image-chemical-potential-differences-are-slopes-of-the-total-helmholtz-free-energy). Chemical potential differences are slopes of the total Helmholtz free energy**. Two equal rigid compartments at fixed [temperature](temperature.md) start with $9\,\mathrm{mol}$ and $3\,\mathrm{mol}$ of the same [ideal gas](ideal-gas.md), and reach $6\,\mathrm{mol}$ each after exchange. Lower left: the [dimensionless](physics.md#dimensionless-quantity) excess [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy). Lower right: its [derivative](calculus.md#derivative) with respect to the allocation, divided by $RT$, equals the [chemical potential](chemical-potential.md) difference divided by $RT$. The horizontal variable is $x=n_A/n_{\rm tot}$.

The beautiful connection is that the direction of matter exchange and the slope of a [free energy](thermodynamic-potential.md#thermodynamic-free-energy) curve are the same calculation. The [entropy](entropy.md) gained by redistributing the [ideal gas](ideal-gas.md) makes equal allocation favorable here. As with [chemical equilibrium](#chemical-equilibrium), a [free energy](thermodynamic-potential.md#thermodynamic-free-energy) minimum identifies the favored state, while transport properties determine how quickly it is reached. The fixed-[temperature](temperature.md), fixed-[pressure](pressure.md) [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) criterion is summarized in [16.4 Free Energy](chemistry-bibliography.md#chemistry-2e-by-paul-flowers-and-others/16-4-free-energy); the rigid experiment instead uses [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy).

## Chemical potential of an ideal gas

↑ **Parent:** [Chemical potential](chemical-potential.md)

For a pure [ideal gas](ideal-gas.md) at [temperature](temperature.md) $T$ and [pressure](pressure.md) $p$,

$$
\mu_{\rm m}(T,p)=\mu_{\rm m}^\circ(T)+RT\ln\frac{p}{p^\circ},
$$

where $R$ is the [molar gas constant](ideal-gas.md#molar-gas-constant) and $p^\circ$ specifies the reference [pressure](pressure.md) of the [standard state](#standard-state). The ratio inside the [natural logarithm](calculus.md#natural-logarithm) is [dimensionless](physics.md#dimensionless-quantity). The [chemical potential](chemical-potential.md) difference therefore depends on a ratio of [pressures](pressure.md), not an absolute difference. See [MIT 5.60, Lecture 14, page 4](https://ocw.mit.edu/courses/5-60-thermodynamics-kinetics-spring-2008/e763a06aa3b5de09cd6bfea6280f219c_5_60_lecture14.pdf).

For a [chemical species](mathematical-biology.md#chemical-species) in an ideal [gas](thermodynamics.md#gas) [mixture](mixture.md), replace $p$ by its [partial pressure](ideal-gas.md#partial-pressure). More generally write $\mu_{{\rm m},i}=\mu_{{\rm m},i}^\circ+RT\ln a_i$ using its [thermodynamic activity](#thermodynamic-activity) $a_i$ and a consistent [standard state](#standard-state). For an ideal dilute [chemical solution](mixture.md#solution-chemistry), $a_i=c_i/c^\circ$ with reference [concentration](mathematical-physics.md#concentration) $c^\circ$; the [thermodynamic activity](#thermodynamic-activity) section describes departures from this idealization.

As a computed comparison, take identical [chemical species](mathematical-biology.md#chemical-species) at $T=300\,\mathrm K$, with $p_A=2p^\circ$ and $p_B=p^\circ$. Stipulate $R=8.314462618\,\mathrm{J\,mol^{-1}\,K^{-1}}$. Then

$$
\mu_{{\rm m},B}-\mu_{{\rm m},A}
=RT\ln\frac{p_B}{p_A}
=-RT\ln2
\simeq-1728.944\,\mathrm{J\,mol^{-1}}.
$$

Halving the [pressure](pressure.md) gives the same decrement whether starting from $2p^\circ$ or $20p^\circ$, provided the [ideal gas](ideal-gas.md) approximation remains valid. This comparison uses different [pressures](pressure.md); it is not the common-[pressure](pressure.md) reservoir setup of [chemical potential equality for particle exchange](#chemical-potential-equality-for-particle-exchange). The fixed-[volume](thermodynamics.md#volume-thermodynamics) example in [chemical potential and Helmholtz free energy](#chemical-potential-and-helmholtz-free-energy) supplies an exchange experiment with unequal initial [pressures](pressure.md).

<a id="image-ideal-gas-chemical-potential-difference-versus-pressure-ratio"></a>
![](chemical-potential-and-pressure.png)

**[Figure 2](#image-ideal-gas-chemical-potential-difference-versus-pressure-ratio). Ideal gas chemical potential difference versus pressure ratio**. At a common [temperature](temperature.md), the [chemical potential](chemical-potential.md) difference is $RT\ln(p_B/p_A)$. The arrows give the initial transfer direction through an open route between rigid compartments; the decreasing [thermodynamic potential](thermodynamic-potential.md) there is [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy). The marked comparison uses $300\,\mathrm K$ and the stipulated [molar gas constant](ideal-gas.md#molar-gas-constant).

## Electrochemical potential

↑ **Parent:** [Chemical potential](chemical-potential.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electrochemical_potential)

The molar [electrochemical potential](#electrochemical-potential) combines the molar [chemical potential](chemical-potential.md) $\mu_{\rm m}$ with the electrical contribution $zF_{\rm Far}\psi$, where $z$ is the signed charge number of an [ion](chemistry.md#ion), $F_{\rm Far}=N_{\rm A}e$ is the [Faraday constant](physics.md#faraday-constant) and $\psi$ is [electric potential](electric-field.md#electric-potential). Both terms have units $\mathrm{J\,mol^{-1}}$. In the particle convention the corresponding expression is $\widetilde\mu_{\rm particle}=\mu_{\rm particle}+ze\psi$, with [elementary charge](electric-charge.md#elementary-charge) $e$; multiplying it by the [Avogadro constant](physics.md#avogadro-constant) gives the molar form. Transfer between locations at the same [temperature](temperature.md) and [pressure](pressure.md) is driven by differences in [electrochemical potential](#electrochemical-potential). The [membrane transport](cell-membrane.md#membrane-transport) examples use it to distinguish neutral [solute](mixture.md#solute) transfer from [ion](chemistry.md#ion) transfer.

### Electrochemical gradient

↑ **Parent:** [Electrochemical potential](#electrochemical-potential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electrochemical_gradient)

An [electrochemical gradient](#electrochemical-gradient) combines spatial changes in [chemical potential](chemical-potential.md) and [electric potential](electric-field.md#electric-potential) for a charged species. [Passive transport](cell-membrane.md#passive-transport) proceeds downhill in [electrochemical potential](#electrochemical-potential) when an appropriate route is available; a [concentration](mathematical-physics.md#concentration) difference alone does not determine the direction for an [ion](chemistry.md#ion).

#### Proton-motive force

↑ **Parent:** [Electrochemical gradient](#electrochemical-gradient)

A [proton-motive force](#proton-motive-force) is a [proton](physics.md#proton) [electrochemical potential](#electrochemical-potential) difference per unit [electric charge](electric-charge.md). It combines the [electric potential difference](electric-field.md#electric-potential-difference) and the [chemical potential](chemical-potential.md) difference across a [cell membrane](cell-membrane.md); the direction and sign convention must be specified.

## Chemical potential of a composition field

↑ **Parent:** [Chemical potential](chemical-potential.md)

For a composition [free energy](thermodynamic-potential.md#thermodynamic-free-energy) $F=\int[f(\phi)+\kappa|\nabla\phi|^2/2]$, the local chemical potential is the [functional derivative](calculus-of-variations.md#functional-derivative)

$$
\mu=f'(\phi)-\kappa\nabla^2\phi.
$$

At [phase coexistence](critical-phenomenon.md#phase-coexistence), exchanges between the bulk phases require equal [chemical potentials](chemical-potential.md). Mechanical equilibrium additionally requires equal [pressure](pressure.md) for a flat interface, or a [Young–Laplace equation](surface-tension.md#young-laplace-equation) pressure jump for a curved interface.

## Chemical equilibrium

↑ **Parent:** [Chemical potential](chemical-potential.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_equilibrium)

At [chemical equilibrium](#chemical-equilibrium), a reversible [chemical reaction](chemical-reaction.md) has equal forward and reverse [reaction rates](chemical-kinetics.md#reaction-rate), so its macroscopic composition stays constant. Individual [molecules](molecule.md) can keep changing identity: the reaction has not stopped. This dynamic balance is the definition described by the [IUPAC Gold Book, chemical equilibrium](https://goldbook.iupac.org/terms/view/C01023). Equal [reaction rates](chemical-kinetics.md#reaction-rate) also need not mean equal [concentrations](mathematical-physics.md#concentration). A small population converting rapidly can balance a large population converting slowly.

This distinction gives two useful questions. Which composition is favored at the specified [temperature](temperature.md) and other constraints? [Thermodynamics](thermodynamics.md) answers through [chemical potentials](chemical-potential.md) and an [equilibrium constant](#equilibrium-constant). How quickly does a prepared mixture approach that composition? [Chemical kinetics](chemical-kinetics.md) answers through [reaction rates](chemical-kinetics.md#reaction-rate). Knowing the destination does not determine the journey's duration. A composition that barely changes during observation may reflect extremely slow [chemical kinetics](chemical-kinetics.md), so constancy alone does not establish [chemical equilibrium](#chemical-equilibrium).

Consider the idealized elementary [chemical reaction](chemical-reaction.md)

$$
\mathrm A\rightleftharpoons\mathrm B,
\qquad k_f=0.3\,\mathrm{s}^{-1},\qquad k_r=0.1\,\mathrm{s}^{-1}.
$$

Assume a well-mixed [closed system](thermodynamics.md#closed-system) at fixed [temperature](temperature.md) and [volume](geometry-and-topology.md#volume), with first-order [law of mass action](mathematical-biology.md#law-of-mass-action) rates in both directions and no competing [chemical reactions](chemical-reaction.md). Write $a=[\mathrm A]$ and $b=[\mathrm B]$ for [concentrations](mathematical-physics.md#concentration) in $\mathrm M=\mathrm{mol}/\mathrm L$. The total $a+b=C=1\,\mathrm M$ is conserved because each conversion replaces one [molecule](molecule.md) by one [molecule](molecule.md). This conservation is special to the chosen [stoichiometry](chemical-reaction.md#stoichiometry).

The forward and reverse [reaction rates](chemical-kinetics.md#reaction-rate), measured as conversions per unit [volume](geometry-and-topology.md#volume) per unit time, are $J_f=k_fa$ and $J_r=k_rb$. Hence

$$
\frac{da}{dt}=-k_fa+k_rb=-(k_f+k_r)a+k_rC.
$$

Setting this [derivative](calculus.md#derivative) to zero gives

$$
a_{\rm eq}=\frac{k_rC}{k_f+k_r}=0.25\,\mathrm M,
\qquad b_{\rm eq}=0.75\,\mathrm M.
$$

With $a(0)=1\,\mathrm M$ and $b(0)=0$, solving the [ordinary differential equation](differential-equation.md#ordinary-differential-equation) yields

$$
a(t)=\bigl(0.25+0.75e^{-0.4t/\mathrm s}\bigr)\,\mathrm M,
\qquad b(t)=\bigl(0.75-0.75e^{-0.4t/\mathrm s}\bigr)\,\mathrm M.
$$

At $t=5\,\mathrm s$, these are approximately $0.3515\,\mathrm M$ and $0.6485\,\mathrm M$. Initially $J_f=0.3\,\mathrm{M/s}$ and $J_r=0$. At [chemical equilibrium](#chemical-equilibrium), both are $0.075\,\mathrm{M/s}$, while the net [reaction rate](chemical-kinetics.md#reaction-rate) $J_f-J_r$ is zero. The persistent exchange is visible in the lower panel even after the upper panel has nearly flattened.

<a id="image-constant-equilibrium-composition-with-continuing-molecular-conversion"></a>
![](reversible-reaction-equilibrium.png)

**[Figure 3](#image-constant-equilibrium-composition-with-continuing-molecular-conversion). Constant equilibrium composition with continuing molecular conversion**. The idealized [chemical reaction](chemical-reaction.md) starts entirely in A. Upper panel: [concentrations](mathematical-physics.md#concentration). Lower panel: forward, reverse and net [reaction rates](chemical-kinetics.md#reaction-rate). The equilibrium rates coincide at a positive value.

Why does [chemical equilibrium](#chemical-equilibrium) also involve a [free energy](thermodynamic-potential.md#thermodynamic-free-energy) minimum? For a [closed system](thermodynamics.md#closed-system) at fixed [temperature](temperature.md) and [pressure](pressure.md), without imposed non-expansion [work](energy.md#work), stable equilibrium minimizes [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) over compositions allowed by conserved elemental inventories. See [W. C. Carter, MIT thermodynamics notes, sections 2-1.14 and 2-1.19](https://ocw.mit.edu/courses/3-00-thermodynamics-of-materials-fall-2002/14c95abd6fac023d84bd33c5d74d787d_lecture_02_oneside.PDF). This is [constrained Gibbs minimization for chemical equilibrium](thermodynamic-potential.md#constrained-gibbs-minimization-for-chemical-equilibrium): freely minimizing over unrelated species amounts would change the inventory. At fixed [temperature](temperature.md) and [volume](geometry-and-topology.md#volume), the appropriate potential is [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy). In either setting, varying an allowed [extent of reaction](chemical-reaction.md#extent-of-reaction) gives the corresponding [free energy](thermodynamic-potential.md#thermodynamic-free-energy) slope $\sum_i\nu_i\mu_i$, with molar [chemical potentials](chemical-potential.md) and signed [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) entries. An interior equilibrium has zero slope; stability requires a minimum. For A converting to B, this says $\mu_{\mathrm B}=\mu_{\mathrm A}$.

The beauty of this connection is that molecular exchange, a macroscopic composition, and a geometric minimum describe the same balance. In the ideal concentration model, let $x=b/C$ and choose the standard molar [chemical potential](chemical-potential.md) difference consistent with $K=3$. Up to a composition-independent constant, the fixed-volume [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) then obeys

$$
\frac{F}{nRT}=(1-x)\ln(1-x)+x\ln x-x\ln3,
$$

where $n$ is the conserved total [amount of substance](physics.md#amount-of-substance) and $R$ the [molar gas constant](ideal-gas.md#molar-gas-constant). Its [derivative](calculus.md#derivative) is $\ln[x/(1-x)]-\ln3$, vanishing at $x=3/4$. Its second [derivative](calculus.md#derivative) is $1/x+1/(1-x)>0$ inside $0<x<1$, so this balance is the unique minimum. The mixing [entropy](entropy.md) terms explain why the favored composition still contains A.

### Number-based dissociation equilibrium ratio

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For ideal-gas single-particle functions $Z_1^{(i)}=C_iVT^{3/2}$ and reaction $A\rightleftharpoons2B$, equilibrium gives $K_N=N_B^2/N_A=(C_B^2/C_A)VT^{3/2}$. This particle-number ratio contains a [volume](geometry-and-topology.md#volume) factor; the concentration ratio $n_B^2/n_A=K_N/V$ does not.

### Reaction formula-unit conservation

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For $A\rightleftharpoons2B$, the conserved amount is $M=N_A+N_B/2$. The total particle count $N_A+N_B$ changes during reaction. Defining a dissociated fraction by $\alpha=N_B/(2M)$ gives $N_A=M(1-\alpha)$.

#### Dissociation fraction versus conserved density

↑ **Parent:** [Reaction formula-unit conservation](#reaction-formula-unit-conservation)

For $A\rightleftharpoons2B$, $\alpha^2/(1-\alpha)=K_N/(4M)$. The left side increases monotonically on $0<\alpha<1$, so increasing the conserved formula-unit [density](fluid-mechanics.md#density) at fixed [temperature](temperature.md) reduces dissociation in the ideal model.

### Ionic product of water

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The product of hydrogen-ion and hydroxide-ion activities at a specified temperature. In dilute aqueous solution at 25 degrees Celsius, its usual [concentration](mathematical-physics.md#concentration) approximation is ten to the minus fourteen.

### Dimerization

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

Reversible association of two molecular units to form a [dimer](molecule.md#dimer).

### Ocean carbonate chemistry

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The linked equilibria among dissolved [carbon dioxide](chemical-substance.md#carbon-dioxide), bicarbonate, carbonate and hydrogen ions in seawater. At a fixed alkalinity, added carbon changes speciation and acidity, limiting how much extra carbon can be held at a given atmospheric [partial pressure](ideal-gas.md#partial-pressure). Exchange and chemical partitioning therefore do not behave like irreversible destruction by a single first-order sink.

#### Carbonate compensation

↑ **Parent:** [Ocean carbonate chemistry](#ocean-carbonate-chemistry)

Adjustment of ocean and sediment carbonate chemistry through dissolution or burial of carbonate minerals. Following a carbon-dioxide perturbation, additional carbonate dissolution can increase alkalinity and permit further ocean uptake. The adjustment is much slower than surface gas exchange, operating over millennial timescales.

<h3 id="van-t-hoff-equation">Van't Hoff equation</h3>

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The temperature relation $\mathrm d\ln K/\mathrm dT=\Delta_rH^\circ/(RT^2)$ for a dimensionless thermodynamic equilibrium constant. With constant reaction enthalpy, integration gives the difference of reciprocal temperatures.

### Standard entropy of reaction

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The stoichiometric sum of standard molar entropies of products minus those of reactants: $\Delta_rS^\circ=\sum_i\nu_iS_i^\circ$.

### Gibbs energy of reaction

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The derivative of [Gibbs energy](thermodynamic-potential.md#gibbs-free-energy) with respect to reaction extent at fixed [temperature](temperature.md) and [pressure](pressure.md): $\Delta_rG=\sum_i\nu_i\mu_i$. For a reversible electrochemical cell reaction, $\Delta_rG=-nFE$.

#### Standard Gibbs energy of reaction

↑ **Parent:** [Gibbs energy of reaction](#gibbs-energy-of-reaction)

The [Gibbs energy of reaction](#gibbs-energy-of-reaction) for specified [standard states](#standard-state). It determines the dimensionless [equilibrium constant](#equilibrium-constant) through $\Delta_rG^\circ=-RT\ln K$.

### Chemical equilibrium of a classical spin gas

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For a nondegenerate spin-one-half ideal gas with energies $\mp\mu_BB(\mathbf r)$, the two component [chemical potentials](chemical-potential.md) are $k_BT\ln(n_\pm/n_Q)\mp\mu_BB$. Diffusive and spin-conversion equilibrium require one spatially constant common chemical potential, provided spin conversion is allowed. Hence the displayed densities give total [number density](statistical-physics.md#number-density) $n=2n_Qe^{\beta\mu}\cosh(\beta\mu_BB)$ and [magnetization](electromagnetism.md#magnetization) $M=2\mu_Bn_Qe^{\beta\mu}\sinh(\beta\mu_BB)=n\mu_B\tanh(\beta\mu_BB)$. The high-temperature fixed-density limit is $M\simeq n\mu_B^2B/(k_BT)$, a [Curie law](statistical-physics.md#curie-s-law). At fixed chemical potential the density itself varies with temperature, so the unnormalized magnetization need not have a pure $1/T$ dependence.

### Chemical disequilibrium

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

A chemical system is out of local [chemical equilibrium](#chemical-equilibrium) when reaction adjustment cannot keep pace with transport, imposed changes or external driving. Comparing the [chemical relaxation time](#chemical-relaxation-time) with transport and irradiation times identifies plausible departures. [Disequilibrium chemistry in an exoplanet atmosphere](exoplanet.md#disequilibrium-chemistry-in-an-exoplanet-atmosphere) combines this principle with mixing, horizontal advection and [atmospheric photochemistry](exoplanet.md#atmospheric-photochemistry).

### Zero chemical potential from number-changing reactions

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For one particle species in [chemical equilibrium](#chemical-equilibrium) under $2\phi\leftrightarrow3\phi$, chemical balance gives $2\mu_\phi=3\mu_\phi$, hence $\mu_\phi=0$. Elastic $2\phi\leftrightarrow2\phi$ imposes no such constraint. In an expanding universe the number-changing reaction must remain fast compared with the [Hubble parameter](cosmology.md#hubble-parameter); after chemical freeze-out a nonzero [chemical potential](chemical-potential.md) can develop even if elastic collisions maintain [kinetic equilibrium](thermal-equilibrium.md#kinetic-equilibrium).

### Chemical relaxation time

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The chemical relaxation time estimates how rapidly a perturbed abundance returns toward [chemical equilibrium](#chemical-equilibrium). Comparing it with the [eddy mixing time](exoplanet.md#eddy-mixing-time) identifies a [chemical quench level](exoplanet.md#chemical-quench-level).

For the A-to-B model in [chemical equilibrium](#chemical-equilibrium), deviations decay by [exponential decay](analysis.md#exponential-decay) with $\tau_{\rm chem}=1/(k_f+k_r)=2.5\,\mathrm s$. After one such interval, $1/e$ of the initial deviation remains; reaching one percent takes $\ln(100)\tau_{\rm chem}\simeq11.51\,\mathrm s$. Multiplying both [rate constants](chemical-kinetics.md#rate-constant) by two preserves their ratio and the equilibrium composition, but halves $\tau_{\rm chem}$ to $1.25\,\mathrm s$. The equilibrium exchange rates double to $0.15\,\mathrm{M/s}$. Faster exchange therefore coexists with the same final composition and the same [free energy](thermodynamic-potential.md#thermodynamic-free-energy) minimum.

<a id="image-doubling-both-rates-changes-the-approach-time-but-preserves-equilibrium"></a>
![](equilibrium-vs-rate.png)

**[Figure 4](#image-doubling-both-rates-changes-the-approach-time-but-preserves-equilibrium). Doubling both rates changes the approach time but preserves equilibrium**. Left: B [concentration](mathematical-physics.md#concentration) for two pairs of [rate constants](chemical-kinetics.md#rate-constant) with the same ratio. Right: the shared ideal-mixture [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy), shifted to zero at its constrained minimum.

### Equilibrium constant

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equilibrium_constant)

For a specified [chemical reaction](chemical-reaction.md) and [standard state](#standard-state) convention, the dimensionless [equilibrium constant](#equilibrium-constant) is the equilibrium value of the [reaction quotient](#reaction-quotient) $Q=\prod_i a_i^{\nu_i}$, where $a_i$ denotes [thermodynamic activity](#thermodynamic-activity) and $\nu_i$ a signed [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) entry. [Thermodynamic activities](#thermodynamic-activity) incorporate the reference state and departures from ideal behavior. See [IUPAC Gold Book, equilibrium constant](https://goldbook.iupac.org/terms/view/E02177).

In the ideal concentration model for A converting to B, use $a_{\mathrm A}=[\mathrm A]/c^\circ$ and $a_{\mathrm B}=[\mathrm B]/c^\circ$ with the same reference $c^\circ=1\,\mathrm M$. Their ratio gives $Q=[\mathrm B]/[\mathrm A]$ and $K=0.75/0.25=3$. Equality $K=k_f/k_r$ applies to this elementary first-order pair; it is not a universal ratio of two measured [rate constants](chemical-kinetics.md#rate-constant) for an arbitrary multistep [chemical reaction](chemical-reaction.md).

At a specified constant [temperature](temperature.md), with consistent [standard states](#standard-state), the standard molar reaction [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) is

$$
\Delta_rG^\circ=\sum_i\nu_i\mu_i^\circ=-RT\ln K,
\qquad \Delta_rG=\Delta_rG^\circ+RT\ln Q=RT\ln(Q/K).
$$

Here $\Delta_rG$ is the local slope per [mole](physics.md#mole-unit) of [extent of reaction](chemical-reaction.md#extent-of-reaction) at fixed [temperature](temperature.md) and [pressure](pressure.md), rather than the finite total [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy) change between two mixtures. At equilibrium $\Delta_rG=0$, while $\Delta_rG^\circ$ generally remains nonzero. For $K=3$ at $298\,\mathrm K$, it is about $-2.72\,\mathrm{kJ/mol}$. For positive activities, $Q<K$ favors forward conversion and $Q>K$ favors reverse conversion; neither sign supplies a [reaction rate](chemical-kinetics.md#reaction-rate). See [MIT 5.111, Lecture 18, reaction free energy and equilibrium](https://ocw.mit.edu/courses/5-111sc-principles-of-chemical-science-fall-2014/ec12f084d867a5e5532b12ee99bdc767_MIT5_111F14_Lec18.pdf).

#### Dimensionless concentration equilibrium constant

↑ **Parent:** [Equilibrium constant](#equilibrium-constant)

For ideal [concentration](mathematical-physics.md#concentration) activities and signed stoichiometric coefficients $\nu_i$, $K_c=\prod_i(c_i/c^\circ)^{\nu_i}$ at equilibrium. Its numerical value depends on the stated [standard concentration](#standard-concentration) when $\sum_i\nu_i\ne0$. Number concentrations require a number-concentration reference; molar concentrations require the corresponding molar reference.

#### Association constant

↑ **Parent:** [Equilibrium constant](#equilibrium-constant)

For $A+B\rightleftharpoons AB$, a concentration [association constant](#association-constant) is $K_a=[AB]/([A][B])$. Comparisons require matched solvent, temperature and standard-state conventions.

#### Dissociation constant

↑ **Parent:** [Equilibrium constant](#equilibrium-constant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dissociation_constant)

### Standard state

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

A standard state is a specified reference state used to define a species' standard [chemical potential](chemical-potential.md) $\mu_i^\circ$. The reference convention, including [temperature](temperature.md), must be consistent when calculating [thermodynamic activities](#thermodynamic-activity), [reaction quotients](#reaction-quotient), and [equilibrium constants](#equilibrium-constant).

#### Standard pressure

↑ **Parent:** [Standard state](#standard-state)

The reference [pressure](pressure.md) used to define a standard gas activity; a common convention is one bar. Normalizing [pressure](pressure.md) by this reference keeps a thermodynamic [equilibrium constant](#equilibrium-constant) dimensionless.

#### Standard concentration

↑ **Parent:** [Standard state](#standard-state)

The reference concentration $c^\circ$ used to make concentration activities dimensionless. Changing this reference changes the numerical dimensionless [equilibrium constant](#equilibrium-constant) when the reaction changes the total number of solute or gas molecules.

#### Thermodynamic activity

↑ **Parent:** [Standard state](#standard-state)

The thermodynamic activity is the dimensionless quantity defined by $\mu_i=\mu_i^\circ+RT\ln a_i$, where $R$ is the [molar gas constant](ideal-gas.md#molar-gas-constant). For an ideal dilute solution with a specified [concentration](mathematical-physics.md#concentration) reference, $a_i=c_i/c^\circ$; departures from ideality are represented by an [activity coefficient](#activity-coefficient) multiplying this ratio.

##### Chemical fugacity

↑ **Parent:** [Thermodynamic activity](#thermodynamic-activity)

An effective gas [pressure](pressure.md) defined by $\mu=\mu^\circ+RT\ln(f/p^\circ)$ in a specified standard-state convention. It approaches the gas [pressure](pressure.md) at low density and differs from the dimensionless [fugacity](statistical-physics.md#fugacity-statistical-mechanics).

##### Activity coefficient

↑ **Parent:** [Thermodynamic activity](#thermodynamic-activity)

### Reaction quotient

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For a [chemical reaction](chemical-reaction.md) with signed [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) entries $\nu_i$, positive for products and negative for reactants, the reaction quotient is the product of the species' [thermodynamic activities](#thermodynamic-activity) raised to these powers. It equals the [equilibrium constant](#equilibrium-constant) at [chemical equilibrium](#chemical-equilibrium), with all quantities using the same [standard state](#standard-state) convention.

### Photon chemical potential

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The chemical potential of photons in thermal equilibrium is zero because their number is not conserved.

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics.md)
2. [Statistical physics](statistical-physics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (347)

- [Adsorption chemical potential](physical-chemistry.md#adsorption-chemical-potential)
- [Aggregate molecular fraction versus aggregate number fraction](physical-chemistry.md#aggregate-molecular-fraction-versus-aggregate-number-fraction)
- [Asymmetric-cutoff BCS transition temperature](fermi-liquid.md#asymmetric-cutoff-bcs-transition-temperature)
- [BCS-BEC crossover](fermi-liquid.md#bcs-bec-crossover)
- [BCS quasiparticle spectrum](fermi-liquid.md#bcs-quasiparticle-spectrum)
- [Binary activity-coefficient consistency](thermodynamics.md#binary-activity-coefficient-consistency)
- [Boltzmann distribution](thermodynamics.md#boltzmann-distribution)
- [Boltzmann suppression](thermal-equilibrium.md#boltzmann-suppression)
- [Boltzmann suppression of a nonrelativistic relic](thermal-equilibrium.md#boltzmann-suppression-of-a-nonrelativistic-relic)
- [Bose condensation in a three-dimensional harmonic trap](quantum-ideal-gas-statistics.md#bose-condensation-in-a-three-dimensional-harmonic-trap)
- [Bosonic coherent-state path integral](quantum-field-theory.md#bosonic-coherent-state-path-integral)
- [Carrier densities with chemical potential pinned to a band edge](tensor-product-of-quantum-systems.md#carrier-densities-with-chemical-potential-pinned-to-a-band-edge)
- [Chemical equilibrium](#chemical-equilibrium)
- [Chemical equilibrium of a classical spin gas](#chemical-equilibrium-of-a-classical-spin-gas)
- [Chemical potential](chemical-potential.md)
- [Chemical potential and Helmholtz free energy](#chemical-potential-and-helmholtz-free-energy)
- [Chemical potential equality for particle exchange](#chemical-potential-equality-for-particle-exchange)
- [Chemical potential of a composition field](#chemical-potential-of-a-composition-field)
- [Chemical potential of a two-dimensional ideal Fermi gas](quantum-ideal-gas-statistics.md#chemical-potential-of-a-two-dimensional-ideal-fermi-gas)
- [Chemical potential of an adsorbed species on equivalent sites](physical-chemistry.md#chemical-potential-of-an-adsorbed-species-on-equivalent-sites)
- [Chemical potential of an ideal gas](#chemical-potential-of-an-ideal-gas)
- [Clapeyron pressure relation for equal-density phases](geophysics.md#clapeyron-pressure-relation-for-equal-density-phases)
- [Clausius-Clapeyron relation](thermodynamic-potential.md#clausius-clapeyron-relation)
- [Common-pressure melting-point slope](thermodynamic-potential.md#common-pressure-melting-point-slope)
- [Common-tangent construction for phase coexistence](critical-phenomenon.md#common-tangent-construction-for-phase-coexistence)
- [Compensated semiconductor](semiconductor.md#compensated-semiconductor)
- [Condensate compressibility in an optical lattice](optics.md#condensate-compressibility-in-an-optical-lattice)
- [Constrained Gibbs minimization for chemical equilibrium](thermodynamic-potential.md#constrained-gibbs-minimization-for-chemical-equilibrium)
- [Contact potential difference](quantum-mechanics.md#contact-potential-difference)
- [Critical micelle concentration](physical-chemistry.md#critical-micelle-concentration)
- [Critical micelle concentration from standard chemical potentials](physical-chemistry.md#critical-micelle-concentration-from-standard-chemical-potentials)
- [Cubic-quintic Gross–Pitaevskii equation](quantum-ideal-gas-statistics.md#cubic-quintic-gross-pitaevskii-equation)
- [Degenerate neutrino and antineutrino energy density](cosmology.md#degenerate-neutrino-and-antineutrino-energy-density)
- [Density crossover of a fixed-coupling BCS cutoff model](fermi-liquid.md#density-crossover-of-a-fixed-coupling-bcs-cutoff-model)
- [Diffusion-capacitance analogy](critical-phenomenon.md#diffusion-capacitance-analogy)
- [Diffusion-controlled droplet growth](critical-phenomenon.md#diffusion-controlled-droplet-growth)
- [Diffusion creep](engineering.md#diffusion-creep)
- [Dilute-polymer free-energy expansion](mixture.md#dilute-polymer-free-energy-expansion)
- [Electrochemical gradient](#electrochemical-gradient)
- [Electrochemical potential](#electrochemical-potential)
- [Electron-positron thermal pair abundance](quantum-ideal-gas-statistics.md#electron-positron-thermal-pair-abundance)
- [Electron removal spectral function](quantum-field-theory.md#electron-removal-spectral-function)
- [Energy reference in molecular partition functions](canonical-ensemble.md#energy-reference-in-molecular-partition-functions)
- [Entropy density](entropy.md#entropy-density)
- [Entropy density at zero chemical potential](entropy.md#entropy-density-at-zero-chemical-potential)
- [Entropy density of a photon gas](statistical-physics.md#entropy-density-of-a-photon-gas)
- [Equilibrating voltage probe](quantum-mechanics.md#equilibrating-voltage-probe)
- [Extent of reaction](chemical-reaction.md#extent-of-reaction)
- [Fermi-Dirac half-order integral at zero argument](tensor-product-of-quantum-systems.md#fermi-dirac-half-order-integral-at-zero-argument)
- [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy)
- [Fermi-energy oscillations in a two-dimensional electron gas](quantum-theory.md#fermi-energy-oscillations-in-a-two-dimensional-electron-gas)
- [Fermi level](quantum-ideal-gas-statistics.md#fermi-level)
- [Fermi-volume conservation in two hybridized electron bands](bloch-s-theorem.md#fermi-volume-conservation-in-two-hybridized-electron-bands)
- [Fermi window](quantum-ideal-gas-statistics.md#fermi-window)
- [Field-induced triplon condensation](quantum-ideal-gas-statistics.md#field-induced-triplon-condensation)
- [Finite-box ground-energy convention in Bose condensation](quantum-ideal-gas-statistics.md#finite-box-ground-energy-convention-in-bose-condensation)
- [Finite-micelle aggregation-number distribution](physical-chemistry.md#finite-micelle-aggregation-number-distribution)
- [Finite-size condensate chemical potential](quantum-ideal-gas-statistics.md#finite-size-condensate-chemical-potential)
- [Finite-temperature electron equation of state](quantum-ideal-gas-statistics.md#finite-temperature-electron-equation-of-state)
- [Fixed-chemical-potential Sommerfeld density increase](quantum-ideal-gas-statistics.md#fixed-chemical-potential-sommerfeld-density-increase)
- [Fixed-number low-temperature Pauli susceptibility](quantum-ideal-gas-statistics.md#fixed-number-low-temperature-pauli-susceptibility)
- [Fixed-particle-number Gibbs minimum](thermodynamic-potential.md#fixed-particle-number-gibbs-minimum)
- [Fugacity (statistical mechanics)](statistical-physics.md#fugacity-statistical-mechanics)
- [Gauge-invariant Josephson phase](superconductivity.md#gauge-invariant-josephson-phase)
- [Gibbs-Duhem equation](thermodynamics.md#gibbs-duhem-equation)
- [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy)
- [Gibbs free energy of mixing](mixture.md#gibbs-free-energy-of-mixing)
- [Grand-canonical Hamiltonian of a Bose field](quantum-ideal-gas-statistics.md#grand-canonical-hamiltonian-of-a-bose-field)
- [Grand-canonical spin susceptibility of a half-filled single level](statistical-physics.md#grand-canonical-spin-susceptibility-of-a-half-filled-single-level)
- [Grand-potential particle-number variance](statistical-physics.md#grand-potential-particle-number-variance)
- [Gross–Pitaevskii equation](quantum-ideal-gas-statistics.md#gross-pitaevskii-equation)
- [Harmonic-trap chemical-potential pinning](quantum-ideal-gas-statistics.md#harmonic-trap-chemical-potential-pinning)
- [Heat capacity for a two-dimensional linear fermion dispersion](quantum-ideal-gas-statistics.md#heat-capacity-for-a-two-dimensional-linear-fermion-dispersion)
- [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy)
- [Ideal binary Gibbs-Duhem cancellation](thermodynamics.md#ideal-binary-gibbs-duhem-cancellation)
- [Ideal solution](mixture.md#ideal-solution)
- [Ideal-solution vapor-liquid equilibrium test](mixture.md#ideal-solution-vapor-liquid-equilibrium-test)
- [Impurity level](semiconductor.md#impurity-level)
- [Intensive and extensive thermodynamic quantities](thermodynamics.md#intensive-and-extensive-thermodynamic-quantities)
- [Intensive quantity](thermodynamics.md#intensive-quantity)
- [Intrinsic-semiconductor chemical potential](semiconductor.md#intrinsic-semiconductor-chemical-potential)
- [Kelvin equation](thermodynamic-potential.md#kelvin-equation)
- [Kinetic equilibrium](thermal-equilibrium.md#kinetic-equilibrium)
- [Landau quasiparticle](fermi-liquid.md#landau-quasiparticle)
- [Lens bound on a reconstructed Fermi pocket](bloch-s-theorem.md#lens-bound-on-a-reconstructed-fermi-pocket)
- [Linear composition bias leaves coexistence compositions unchanged](critical-phenomenon.md#linear-composition-bias-leaves-coexistence-compositions-unchanged)
- [Low-temperature energy of gapless bosonic excitations](quantum-ideal-gas-statistics.md#low-temperature-energy-of-gapless-bosonic-excitations)
- [Low-temperature liquid volume of a van der Waals gas](pressure.md#low-temperature-liquid-volume-of-a-van-der-waals-gas)
- [Mass-action model of micellization](physical-chemistry.md#mass-action-model-of-micellization)
- [Maxwell-Boltzmann distribution](quantum-ideal-gas-statistics.md#maxwell-boltzmann-distribution)
- [Maxwell construction](thermodynamic-potential.md#maxwell-construction)
- [Maxwell relations](thermodynamics.md#maxwell-relations)
- [Membrane transport](cell-membrane.md#membrane-transport)
- [Mixture measurements and the Gibbs-Duhem constraint](thermodynamics.md#mixture-measurements-and-the-gibbs-duhem-constraint)
- [Nernst equilibrium potential](membrane-potential.md#nernst-equilibrium-potential)
- [Nonrelativistic entropy at zero chemical potential](entropy.md#nonrelativistic-entropy-at-zero-chemical-potential)
- [Number density of a relativistic neutrino relative to photons](cosmology.md#number-density-of-a-relativistic-neutrino-relative-to-photons)
- [Occupation of an interacting localized electron level](bloch-s-theorem.md#occupation-of-an-interacting-localized-electron-level)
- [One-dimensional photon-gas thermodynamics](statistical-physics.md#one-dimensional-photon-gas-thermodynamics)
- [One-electron defect plateau](statistical-physics.md#one-electron-defect-plateau)
- [Open-system equilibrium contacts](#open-system-equilibrium-contacts)
- [Order-parameter mobility](critical-phenomenon.md#order-parameter-mobility)
- [Oscillatory thermal-change amplitude ratio](quantum-ideal-gas-statistics.md#oscillatory-thermal-change-amplitude-ratio)
- [Osmosis](cell-membrane.md#osmosis)
- [Osmotic pressure](cell-membrane.md#osmotic-pressure)
- [Osmotic pressure in Flory-Huggins solution theory](mixture.md#osmotic-pressure-in-flory-huggins-solution-theory)
- [Ostwald ripening](critical-phenomenon.md#ostwald-ripening)
- [Oxygen concentration cell](electrochemistry.md#oxygen-concentration-cell)
- [Pairing gap](fermi-liquid.md#pairing-gap)
- [Particle saturation in a homogeneous Bose gas](quantum-ideal-gas-statistics.md#particle-saturation-in-a-homogeneous-bose-gas)
- [Passive transport](cell-membrane.md#passive-transport)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#1/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#2/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2.md#a7/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2.md#a10/a/ii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2.md#a10/a/iv/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2.md#a10/b/ii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2.md#a6/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2.md#a8/a/i/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/b/ii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#6/e/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#5/c/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#48/f/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#5/a/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#section-e/26/e/solution)
- [B](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2019/paper-1.md#4/b)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-67.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-55.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4.md#15d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4.md#33b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-61.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-61.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83.md#2/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-62.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#10a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#33e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#15d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-72.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#34d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#34d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-42.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-81.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#33c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#33c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#33c/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-53.md#2/2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#34d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#34d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-305.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-310.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#35a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#36a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#9b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#35d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-310.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-344.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#35a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#36a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#35a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#35a/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-344.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#37b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#9d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#35b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#35b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2.md#9e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-344.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-344.md#1/d/ii/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/10/iii/c/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/10/iv/c/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-2.md#section-a-i/14/i/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-2.md#section-b/19/i/solution)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2021/paper-ne3.md#4/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c11/b-internal-energy/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2.md#section-d/d13/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c10/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2.md#section-d/d9/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2.md#section-a/4/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/f/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c11/equations-of-state-and-transitions/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c11/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-a/a2/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2.md#section-c/c8/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#b3/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-b/b2/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1.md#1/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2013/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2013/paper-1.md#2/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2013/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#1/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b7/b/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b8/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-c/c11/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-c/c14/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2009.md#section-b/b4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012.md#1/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012.md#2/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012.md#3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2013.md#3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2013.md#4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014.md#4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1.md#4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017.md#1/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017.md#3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017.md#4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021.md#section-b/6/b/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022.md#section-b/5/f/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022.md#section-b/6/b/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1.md#4/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-b/b5/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2013/paper-1.md#2/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2014/paper-1.md#2/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#2/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#3/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018.md#section-b/b2/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-a/1/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/6/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/d/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/e/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/d/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/e/solution)
- [Pauli reduction of the pinned-edge mass-action product](semiconductor.md#pauli-reduction-of-the-pinned-edge-mass-action-product)
- [Phase diagram](thermodynamic-potential.md#phase-diagram)
- [Phase equilibrium](thermodynamics.md#phase-equilibrium)
- [Phase rule](thermodynamic-potential.md#phase-rule)
- [Phonon](quantum-ideal-gas-statistics.md#phonon)
- [Photon gas](statistical-physics.md#photon-gas)
- [Polymorphism (materials science)](thermodynamics.md#polymorphism-materials-science)
- [Pomeranchuk cooling](statistical-physics.md#pomeranchuk-cooling)
- [Primordial helium response to electron-neutrino degeneracy](cosmology.md#primordial-helium-response-to-electron-neutrino-degeneracy)
- [Proton-motive force](#proton-motive-force)
- [Quadratic-boson heat-capacity coefficient](quantum-ideal-gas-statistics.md#quadratic-boson-heat-capacity-coefficient)
- [Quantum capacitance](electromagnetism.md#quantum-capacitance)
- [Quantum concentration](canonical-ensemble.md#quantum-concentration)
- [Quasi-Fermi level](#quasi-fermi-level)
- [Raoult's law](mixture.md#raoult-s-law)
- [Sakharov conditions](cosmology.md#sakharov-conditions)
- [Saturation of harmonic-trap excited states](quantum-ideal-gas-statistics.md#saturation-of-harmonic-trap-excited-states)
- [Saturation particle number for Bose-Einstein condensation](quantum-ideal-gas-statistics.md#saturation-particle-number-for-bose-einstein-condensation)
- [Screened quantum Hall edge strips](relativistic-electromagnetism.md#screened-quantum-hall-edge-strips)
- [Selective potassium equilibrium](membrane-potential.md#selective-potassium-equilibrium)
- [Semiconductor mass-action law](semiconductor.md#semiconductor-mass-action-law)
- [Single-electron superconducting tunneling](superconductivity.md#single-electron-superconducting-tunneling)
- [Solvation free energy](ionic-bonding.md#solvation-free-energy)
- [Solvation thermodynamic balance](ionic-bonding.md#solvation-thermodynamic-balance)
- [Standard chemical potential](#standard-chemical-potential)
- [Standard state](#standard-state)
- [Substitutional semiconductor doping](semiconductor.md#substitutional-semiconductor-doping)
- [Thermal damping of a sinusoidal density of states](quantum-ideal-gas-statistics.md#thermal-damping-of-a-sinusoidal-density-of-states)
- [Thermionic tail-flux derivation](thermionic-emission.md#thermionic-tail-flux-derivation)
- [Thermodynamic limit](statistical-physics.md#thermodynamic-limit)
- [Thermomechanical effect](statistical-physics.md#thermomechanical-effect)
- [Tonicity](cell-membrane.md#tonicity)
- [Triple point](thermodynamic-potential.md#triple-point)
- [Triple-point cell](thermodynamic-potential.md#triple-point-cell)
- [Tunnel-rate-selective spin readout](semiconductor.md#tunnel-rate-selective-spin-readout)
- [Two-component Bose-Einstein condensate](quantum-ideal-gas-statistics.md#two-component-bose-einstein-condensate)
- [Two-wave estimate of a Bragg-gap coupling from a pocket area](bloch-s-theorem.md#two-wave-estimate-of-a-bragg-gap-coupling-from-a-pocket-area)
- [Uniform-current pumped polariton condensate](quantum-ideal-gas-statistics.md#uniform-current-pumped-polariton-condensate)
- [Uniform ring condensate](quantum-ideal-gas-statistics.md#uniform-ring-condensate)
- [Van der Waals liquid-gas coexistence](pressure.md#van-der-waals-liquid-gas-coexistence)
- [Vaporization](critical-phenomenon.md#vaporization)
- [Vibrational factor in a Langmuir equilibrium constant](physical-chemistry.md#vibrational-factor-in-a-langmuir-equilibrium-constant)
- [Voltage partition in a ballistic constriction](quantum-ideal-gas-statistics.md#voltage-partition-in-a-ballistic-constriction)
- [Water potential](cell-membrane.md#water-potential)
- [Zero chemical potential from number-changing reactions](#zero-chemical-potential-from-number-changing-reactions)
