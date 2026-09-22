# Internal energy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Internal_energy)

Internal energy $U$ is the [energy](energy.md) stored in the microscopic [degrees of freedom](classical-mechanics.md#degree-of-freedom) of a [thermodynamic system](thermodynamics.md#thermodynamic-system): random molecular [kinetic energy](energy.md#kinetic-energy), internal molecular excitations, and interaction [potential energy](energy.md#potential-energy). Its value requires a specified system and an [energy](energy.md) reference. In [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium), [internal energy](internal-energy.md) is a [state function](thermodynamics.md#state-function); it records the present state, without remembering whether a previous change came from stirring, compression or [heat](heat.md) transfer. This makes [internal energy](internal-energy.md) the common accounting quantity connecting mechanical experiments to thermal ones.[§3.2, “Internal Energy”, equation 3.5 and the discussion of molecular motion](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/3-2-work-heat-and-internal-energy)

[Heat](heat.md) and [work](energy.md#work) describe [energy](energy.md) crossing the system boundary during a process. They are not separately stored contents of the system. For a [closed system](thermodynamics.md#closed-system) whose bulk [kinetic energy](energy.md#kinetic-energy) and external [potential energy](energy.md#potential-energy) have unchanged endpoint values, the [first law of thermodynamics](first-law-of-thermodynamics.md) gives

$$
\Delta U=Q_{\rm in}+W_{\rm on}=Q_{\rm in}-W_{\rm out}.
$$

Here $Q_{\rm in}$ is positive for incoming [heat](heat.md), and $W_{\rm on}=-W_{\rm out}$ is positive for net [work](energy.md#work) done on the system. Two routes between the same equilibrium states have the same $\Delta U$, although their [heat](heat.md) and [work](energy.md#work) can differ. The infinitesimal notation $dU=\delta Q_{\rm in}+\delta W_{\rm on}$ distinguishes a [state function](thermodynamics.md#state-function) change from path-dependent transfers.[§4.2, equation 4.156 and “Quasi-Static Processes”: state energy versus heat and work; Tong uses work positive inward](physics-bibliography.md#statistical-physics-by-david-tong/4-classical-thermodynamics)

For a calculated example, take one [mole](physics.md#mole-unit) of a classical [monatomic gas](ideal-gas.md#monatomic-gas) in the [ideal gas](ideal-gas.md) regime, at fixed [volume](thermodynamics.md#volume-thermodynamics), from $300$ to $310\,\mathrm K$. With stipulated [molar gas constant](ideal-gas.md#molar-gas-constant) $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$, its [internal energy](internal-energy.md) change is $3nR\Delta T/2=124.71\,\mathrm J$. A purely thermal route supplies $Q_{\rm in}=124.71\,\mathrm J$ with $W_{\rm on}=0$. An ideal insulated stirring route supplies $W_{\rm on}=124.71\,\mathrm J$ with $Q_{\rm in}=0$, measured between equilibrium endpoints after the motion dies away. The same stored increment has two different transfer histories; neither history defines a separate kind of stored [energy](energy.md).

<a id="internal-energy-storage-and-transfers"></a>
![](internal-energy-storage-and-transfers.png)

**[Figure 1](#internal-energy-storage-and-transfers). Internal energy is stored; heat and work are ways to change it**. Original schematic and calculated [ideal gas](ideal-gas.md) example with the stipulated parameters above; no experimental data. The two routes end at the same [temperature](temperature.md) and [volume](thermodynamics.md#volume-thermodynamics). Microscopic [kinetic energy](energy.md#kinetic-energy) and interaction [potential energy](energy.md#potential-energy) belong inside $U$; whole-body motion and external elevation are accounted for separately under the stated convention.

The familiar [internal energy of an ideal gas](ideal-gas.md#internal-energy-of-an-ideal-gas) is a useful special case. Neglect intermolecular interactions, hold the [amount of substance](physics.md#amount-of-substance) $n$ and composition fixed, and suppose that $f$ independent quadratic terms per particle obey the classical [equipartition theorem](canonical-ensemble.md#equipartition-theorem). Choosing the constant reference contribution as zero gives

$$
U=\frac f2nRT,\qquad C_V=\frac f2nR.
$$

Here $T$ is absolute [temperature](temperature.md), $R$ is the [molar gas constant](ideal-gas.md#molar-gas-constant), and $C_V$ is the whole sample's [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume). A [monatomic gas](ideal-gas.md#monatomic-gas) has $f=3$ translational terms. A rigid diatomic [molecule](molecule.md) has $f=5$ when its two rotational terms are active and vibration is frozen; activating one [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) vibration adds two terms, one [kinetic energy](energy.md#kinetic-energy) and one [potential energy](energy.md#potential-energy), giving $f=7$. The counting is of quadratic contributions, so a vibrational coordinate is not just one contribution.[§§2.2.1 and 2.4, equations 2.57–2.58 and the rotation/vibration energy counting](physics-bibliography.md#statistical-physics-by-david-tong/2-classical-gases)

This constant-$f$ formula applies only over a regime with those same active terms, classical translational statistics, nonrelativistic motion and unchanged composition. Quantum freezing, [quantum degeneracy](quantum-mechanics.md#degenerate-energy-levels), [chemical reactions](chemical-reaction.md) or appreciable intermolecular interactions invalidate that simple counting. More generally, at fixed amount and composition an [ideal gas](ideal-gas.md) can still have $U=U(T)$ with varying [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume), so use $\Delta U=\int_{T_1}^{T_2}C_V(T)\,dT$. A nonzero constant reference adds $U_*$ to $fnRT/2$ without altering $\Delta U$.

**Table of contents**

- [Thermodynamic internal pressure](#thermodynamic-internal-pressure)
- [Internal energy and system boundaries](#internal-energy-and-system-boundaries)
- [Internal energy at constant temperature](#internal-energy-at-constant-temperature)
- [Joule's paddle-wheel experiment](#joule-s-paddle-wheel-experiment)
  - [Paddle-wheel calorimetry energy balance](#paddle-wheel-calorimetry-energy-balance)
- [Specific internal energy](#specific-internal-energy)

## Thermodynamic internal pressure

↑ **Parent:** [Internal energy](internal-energy.md)

For a [simple compressible system](thermodynamics.md#simple-compressible-system) at fixed composition and particle number, the internal pressure is the [partial derivative](multivariable-calculus.md#partial-derivative) of [internal energy](internal-energy.md) with respect to [volume](thermodynamics.md#volume-thermodynamics) at fixed [temperature](temperature.md). From $dU=T\,dS-p\,dV$ and the [Maxwell relation](thermodynamics.md#maxwell-relations) $(\partial S/\partial V)_T=(\partial p/\partial T)_V$, it has the measurable expression in the title. It is distinct from the mechanical [pressure](pressure.md) $p$.

For an [ideal gas](ideal-gas.md), $p=nRT/V$ gives $\pi_T=0$, so its [internal energy](internal-energy.md) depends only on [temperature](temperature.md) at fixed amount of gas. For the [Dieterici equation](thermodynamics.md#dieterici-equation) $p=nRT\exp[-an/(VRT)]/(V-nb)$, direct [differentiation](calculus.md#differentiation) gives

$$
\pi_T=\frac{an^2}{V(V-nb)}\exp\left(-\frac{an}{VRT}\right).
$$

Thus an [equation of state](pressure.md#equation-of-state) determines this volume sensitivity even without determining the full caloric [function](function.md) $U(T,V)$.

## Internal energy and system boundaries

↑ **Parent:** [Internal energy](internal-energy.md)

For an ordinary stationary laboratory sample, a useful convention is

$$
E_{\rm total}=U+K_{\rm bulk}+\Phi_{\rm ext},\qquad
\Delta U+\Delta K_{\rm bulk}+\Delta\Phi_{\rm ext}
=Q_{\rm in}+W_{\rm on}.
$$

The bulk [kinetic energy](energy.md#kinetic-energy) $K_{\rm bulk}$ includes organized whole-body motion; for pure translation it is $Mv_{\rm cm}^2/2$, with total [mass](classical-mechanics.md#mass) $M$ and [center of mass](classical-mechanics.md#center-of-mass) speed $v_{\rm cm}$. The external [potential energy](energy.md#potential-energy) $\Phi_{\rm ext}$ includes elevation in an imposed [gravitational field](physics.md#gravitational-field), approximately $Mgz$ in a uniform field. Accelerating a sealed bottle or lifting it without otherwise changing its state changes these mechanical terms, rather than its [internal energy](internal-energy.md). Molecular [kinetic energy](energy.md#kinetic-energy) is measured relative to the chosen bulk motion.[§3.2, “Internal Energy”: molecular speeds relative to the center of mass; moving-train and roof examples](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/3-2-work-heat-and-internal-energy)

State the convention rather than applying this separation blindly. If an experiment separately tracks a rotating apparatus or an organized flow, its mechanical [kinetic energy](energy.md#kinetic-energy) must not also be counted in $U$. In [Joule's paddle-wheel experiment](#joule-s-paddle-wheel-experiment), waiting for the apparatus and fluid to come to rest removes such an endpoint ambiguity. Including the vessel and paddle changes whose [internal energy](internal-energy.md) is measured; including the falling weights additionally puts their changing [gravitational potential energy](energy.md#gravitational-energy) inside the enlarged system's total [energy](energy.md) balance.

## Internal energy at constant temperature

↑ **Parent:** [Internal energy](internal-energy.md)

Constant [temperature](temperature.md) does not generally mean constant [internal energy](internal-energy.md). At fixed amount and composition, within one smooth [thermodynamic phase](thermodynamics.md#thermodynamic-phase) of a [simple compressible system](thermodynamics.md#simple-compressible-system), an equilibrium identity is

$$
dU=C_V\,dT+\left[T\left(\frac{\partial p}{\partial T}\right)_V-p\right]dV.
$$

The bracket vanishes for the [ideal gas law](ideal-gas.md#ideal-gas-law) $pV=nRT$. It need not vanish for a [real gas](thermodynamics.md#real-gas): changing the [volume](thermodynamics.md#volume-thermodynamics) changes the average interaction [potential energy](energy.md#potential-energy), even when the random-motion contribution stays at the same [temperature](temperature.md). The identity follows by writing $dU=T\,dS-p\,dV$ and using a [Maxwell relation](thermodynamics.md#maxwell-relations); it does not require the actual process to be reversible. [Free Expansion of Gas](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/free-expansion-of-gas)

For a [Van der Waals equation](pressure.md#van-der-waals-equation) model with [volume](thermodynamics.md#volume-thermodynamics) per [mole](physics.md#mole-unit) $v=V/n$, $p=RT/(v-b)-a/v^2$ gives $(\partial U/\partial V)_{T,n}=a/v^2$. Thus an [isothermal expansion](second-law-of-thermodynamics.md#isothermal-expansion) from $v_1$ to $v_2>v_1$, at fixed [amount of substance](physics.md#amount-of-substance) $n$, increases [internal energy](internal-energy.md) by

$$
\Delta U=na\left(\frac1{v_1}-\frac1{v_2}\right)>0.
$$

Separating attractive particles makes their interaction [potential energy](energy.md#potential-energy) less negative. For stipulated $n=1\,\mathrm{mol}$, $a=0.10\,\mathrm{Pa\,m^6\,mol^{-2}}$, $b=10^{-5}\,\mathrm{m^3\,mol^{-1}}$, $T=300\,\mathrm K$, $v_1=0.010$ and $v_2=0.020\,\mathrm{m^3\,mol^{-1}}$, the calculated increase for this one-[mole](physics.md#mole-unit) sample is $5\,\mathrm J$, despite $\Delta T=0$. This dilute stable-branch model example is not a measurement of a named [gas](thermodynamics.md#gas). [Van der Waals Gas](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/van-der-waals-gas)

A [phase transition](critical-phenomenon.md#phase-transition) gives another reason. During equilibrium vaporization of a pure substance at fixed [pressure](pressure.md), the [temperature](temperature.md) can stay at its [phase coexistence](critical-phenomenon.md#phase-coexistence) value while the [phase fraction](thermodynamics.md#phase-fraction) changes. Molecular separation changes interaction [potential energy](energy.md#potential-energy).[§1.5, figure 1.18 and equations 1.7–1.8: molecular attractions and constant-temperature phase conversion](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/1-5-phase-changes) If the [closed system](thermodynamics.md#closed-system) does only [pressure](pressure.md)-[volume](thermodynamics.md#volume-thermodynamics) [work](energy.md#work), its [latent heat](thermodynamic-potential.md#latent-heat) input obeys

$$
Q_{\rm in}=\Delta H,\qquad
\Delta U=\Delta H-p\Delta V.
$$

Here $H=U+pV$ is [enthalpy](enthalpy.md). A vaporization [latent heat](thermodynamic-potential.md#latent-heat) therefore is not automatically the [internal energy](internal-energy.md) increment: some input supplies expansion [work](energy.md#work). A fixed [temperature](temperature.md) reading alone cannot tell how much [internal energy](internal-energy.md) changed.

<h2 id="joule-s-paddle-wheel-experiment">Joule's paddle-wheel experiment</h2>

↑ **Parent:** [Internal energy](internal-energy.md)

Joule's paper [On the Mechanical Equivalent of Heat](physics-bibliography.md#on-the-mechanical-equivalent-of-heat-by-james-prescott-joule) (1850) describes a [copper](chemical-substance.md#copper) vessel holding [water](chemical-substance.md#water) and a brass paddle with stationary vanes. Descending [lead](chemical-substance.md#lead) weights drove its shaft through strings and pulleys; the vanes opposed simple co-rotation. A boxwood shaft segment reduced [thermal conduction](heat.md#thermal-conduction). He measured fall distances and initial/final [temperatures](temperature.md), repeating twenty descents per run and disconnecting the drive for rewinding. Calibrated [thermometers](temperature.md#thermometer) read the [water](chemical-substance.md#water) and room.[pp. 64–66 and Plate VII: thermometer calibration, water apparatus and operating sequence](physics-bibliography.md#on-the-mechanical-equivalent-of-heat-by-james-prescott-joule)

<a id="joule-paddle-wheel-calorimeter"></a>
![](joule-paddle-wheel-calorimeter.png)

**[Figure 2](#joule-paddle-wheel-calorimeter). Joule's paddle-wheel experiment: mechanical input and thermal readout**. Original explanatory schematic, not a scale reconstruction or a plot of measurements. The outlined system includes [water](chemical-substance.md#water), vessel and immersed paddle, but excludes the weights and external drive. The symbolic balance separates mechanical losses outside this boundary from [heat](heat.md) exchange with the room. Rewinding occurs with the drive disconnected.

His matched resting trials retained the [water](chemical-substance.md#water) amount, duration, surroundings and reading procedure, omitting paddle motion to estimate environmental [heat](heat.md) exchange. A screen reduced [thermal radiation](electromagnetic-radiation.md#thermal-radiation) from his body. His calculation included the vessel and paddle [heat capacities](heat.md#heat-capacity), external pulley/string losses, descent [kinetic energy](energy.md#kinetic-energy) and string elasticity; it acknowledged residual vibration and sound.[pp. 66, 69–70 and 82: matched controls, apparatus water-equivalent capacity, mechanical corrections and residual losses](physics-bibliography.md#on-the-mechanical-equivalent-of-heat-by-james-prescott-joule)

The measured observable is a corrected [temperature](temperature.md) rise, interpreted through the participating [heat capacity](heat.md#heat-capacity); it is not a direct view of molecular motion. The experiment tests whether measured mechanical input accounts quantitatively for thermal storage. Frictional warming by itself would establish neither the conversion factor nor the absence of [heat](heat.md) exchange. A modern authored demonstration at UCSB instead measures crank turns and a cylinder's [temperature](temperature.md) with an electrical [thermometer](temperature.md#thermometer): the apparatus differs, but again both mechanical input and thermal response must be measured. [52.33 -- Mechanical equivalent of heat](physics-bibliography.md#ucsb-physics-lecture-demonstrations/52-33-mechanical-equivalent-of-heat)

### Paddle-wheel calorimetry energy balance

↑ **Parent:** [Joule's paddle-wheel experiment](#joule-s-paddle-wheel-experiment)

Choose the [water](chemical-substance.md#water), vessel and immersed paddle as the [closed system](thermodynamics.md#closed-system), with fixed outer [volume](thermodynamics.md#volume-thermodynamics) and negligible endpoint changes in bulk mechanical [energy](energy.md). Between common equilibrium [temperatures](temperature.md) $T_1$ and $T_2$,

$$
\Delta U_{\rm assembly}=\int_{T_1}^{T_2}C_{\rm eff}(T)\,dT
=W_{\rm shaft,on}+Q_{\rm room,in}.
$$

The effective [heat capacity](heat.md#heat-capacity) $C_{\rm eff}$ includes every component that participates in the common [temperature](temperature.md) change. For nearly constant $C_{\rm eff}$, the readout is $C_{\rm eff}\Delta T$. [Heat](heat.md) transferred between [water](chemical-substance.md#water) and paddle stays inside this boundary; it must not be added again as external input. The drive supplies shaft [work](energy.md#work) even though the vessel has no expansion [work](energy.md#work).

For a simplified modern model, let $M$ be the total descending [mass](classical-mechanics.md#mass), let each of $N$ descents cover height $h$, and let $W_{\rm loss,out}$ be [energy](energy.md) diverted by the external drive. With negligible remaining drive [kinetic energy](energy.md#kinetic-energy) and elastic storage,

$$
W_{\rm shaft,on}=NMgh-W_{\rm loss,out},\qquad
NMgh=C_{\rm eff}\Delta T+W_{\rm loss,out}+Q_{\rm room,out}.
$$

The signed $Q_{\rm room,out}=-Q_{\rm room,in}$ may be negative if the room warms the assembly. This model omits the small endpoint and elastic corrections explicitly considered in the historical analysis. It does not equate all of the weights' lost [gravitational potential energy](energy.md#gravitational-energy) with the [water](chemical-substance.md#water)'s gained [internal energy](internal-energy.md).

As a proposed modern protocol, measure the falling [masses](classical-mechanics.md#mass) and distances, calibrate the [thermometer](temperature.md#thermometer) and $C_{\rm eff}$ independently, record room [temperature](temperature.md) and resting drift before and after each run, and wait for fluid motion to decay before the final equilibrium reading. Repeat with different fall budgets and run durations. A stable ratio of corrected input to corrected thermal storage supports the [first law of thermodynamics](first-law-of-thermodynamics.md) over the tested range. Resting controls only estimate leakage if their thermal conditions represent the driven run; sensor lag, nonuniform [temperature](temperature.md), unmeasured drive losses, evaporation or changing [heat capacity](heat.md#heat-capacity) can spoil the inference. Those are limits of the measurement, rather than evidence that [heat](heat.md) was stored as a separate substance.

## Specific internal energy

↑ **Parent:** [Internal energy](internal-energy.md)

Specific [internal energy](internal-energy.md) is [internal energy](internal-energy.md) per unit mass. For a [perfect gas](ideal-gas.md) with constant [specific-heat ratio](ideal-gas.md#heat-capacity-ratio), $e=p/[(\gamma-1)\rho]$. Its material balance is $\rho De/Dt=-p\nabla\cdot\mathbf u+Q$, where $Q$ is [heat](heat.md) supplied per unit volume per unit time.

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics.md)
2. [Statistical physics](statistical-physics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (197)

- [Adiabatic compression](first-law-of-thermodynamics.md#adiabatic-compression)
- [Adiabatic expansion](first-law-of-thermodynamics.md#adiabatic-expansion)
- [Adiabatic process](first-law-of-thermodynamics.md#adiabatic-process)
- [Adiabatic work in a comoving volume](cosmology.md#adiabatic-work-in-a-comoving-volume)
- [Background potential energy](energy.md#background-potential-energy)
- [Calorimetry](calorimetry.md)
- [Canonical partition function](canonical-ensemble.md#canonical-partition-function)
- [Chemical potential](chemical-potential.md)
- [Classical ideal gas in a homogeneous soft trap](canonical-ensemble.md#classical-ideal-gas-in-a-homogeneous-soft-trap)
- [Closed system](thermodynamics.md#closed-system)
- [Constant-entropy magnetic cooling example](temperature.md#constant-entropy-magnetic-cooling-example)
- [Debye T-cubed test](heat.md#debye-t-cubed-test)
- [Dulong-Petit law](heat.md#dulong-petit-law)
- [Einstein solid](heat.md#einstein-solid)
- [Enthalpy](enthalpy.md)
- [Entropic force](force.md#entropic-force)
- [Entropy](entropy.md)
- [Entropy density of a photon gas](statistical-physics.md#entropy-density-of-a-photon-gas)
- [Entropy maximization under thermal contact](thermal-equilibrium.md#entropy-maximization-under-thermal-contact)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Euler relation in thermodynamics](thermodynamics.md#euler-relation-in-thermodynamics)
- [Exergy](thermodynamic-potential.md#exergy)
- [Extensive quantity](thermodynamics.md#extensive-quantity)
- [Finite heat bath](thermal-equilibrium.md#finite-heat-bath)
- [Finite-temperature electron equation of state](quantum-ideal-gas-statistics.md#finite-temperature-electron-equation-of-state)
- [First law of thermodynamics](first-law-of-thermodynamics.md)
- [Fluid total-energy equation](compressible-flow.md#fluid-total-energy-equation)
- [Free expansion](thermodynamics.md#free-expansion)
- [Frictional heating](newtonian-mechanics.md#frictional-heating)
- [Frustrated Ising triangle](spin-model.md#frustrated-ising-triangle)
- [Gibbs-Duhem equation](thermodynamics.md#gibbs-duhem-equation)
- [Gravitational energy generation in a homologously contracting ideal-gas star](stellar-astrophysics.md#gravitational-energy-generation-in-a-homologously-contracting-ideal-gas-star)
- [Heat](heat.md)
- [Heat bath](thermal-equilibrium.md#heat-bath)
- [Heat capacity](heat.md#heat-capacity)
- [Heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume)
- [Heat capacity of a classical magnetic dipole](statistical-physics.md#heat-capacity-of-a-classical-magnetic-dipole)
- [Heat capacity ratio](ideal-gas.md#heat-capacity-ratio)
- [Heat engine](thermodynamics.md#heat-engine)
- [Heat-engine calorimetry](thermodynamics.md#heat-engine-calorimetry)
- [Heat-pump calorimetry](thermodynamics.md#heat-pump-calorimetry)
- [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy)
- [Homogeneous ideal Bose gas condensation](quantum-ideal-gas-statistics.md#homogeneous-ideal-bose-gas-condensation)
- [Homologous adiabatic stellar stability](stellar-structure.md#homologous-adiabatic-stellar-stability)
- [Hydrogen rotational heat capacity](molecule.md#hydrogen-rotational-heat-capacity)
- [Ideal gas](ideal-gas.md)
- [Ideal gas law](ideal-gas.md#ideal-gas-law)
- [Ideal magnetohydrodynamic energy conservation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-energy-conservation)
- [Inelastic collision](classical-mechanics.md#inelastic-collision)
- [Intensive and extensive thermodynamic quantities](thermodynamics.md#intensive-and-extensive-thermodynamic-quantities)
- [Internal energy](internal-energy.md)
- [Internal energy and system boundaries](#internal-energy-and-system-boundaries)
- [Internal energy at constant temperature](#internal-energy-at-constant-temperature)
- [Internal energy of a van der Waals gas](pressure.md#internal-energy-of-a-van-der-waals-gas)
- [Internal energy of an ideal gas](ideal-gas.md#internal-energy-of-an-ideal-gas)
- [Isentropic temperature-volume derivative](thermodynamics.md#isentropic-temperature-volume-derivative)
- [Ising ring bond correlation](spin-model.md#ising-ring-bond-correlation)
- [Isolated system](thermodynamics.md#isolated-system)
- [Isothermal compressibility](thermodynamics.md#isothermal-compressibility)
- [Isothermal expansion](second-law-of-thermodynamics.md#isothermal-expansion)
- [Isothermal process](second-law-of-thermodynamics.md#isothermal-process)
- [James Prescott Joule](physicist.md#james-prescott-joule)
- [Joule heating](electric-charge.md#joule-heating)
- [Joule's free-expansion experiment](thermodynamics.md#joule-s-free-expansion-experiment)
- [Joule-Thomson effect](enthalpy.md#joule-thomson-effect)
- [Kelvin-Planck statement of the second law](second-law-of-thermodynamics.md#kelvin-planck-statement-of-the-second-law)
- [Kinetic friction](newtonian-mechanics.md#kinetic-friction)
- [Latent heat](thermodynamic-potential.md#latent-heat)
- [Lattice energy](ionic-bonding.md#lattice-energy)
- [Linear low-temperature heat capacity of a two-dimensional Fermi gas](quantum-ideal-gas-statistics.md#linear-low-temperature-heat-capacity-of-a-two-dimensional-fermi-gas)
- [Mach-number convention in shock unbinding estimates](compressible-flow.md#mach-number-convention-in-shock-unbinding-estimates)
- [Maxwell relations](thermodynamics.md#maxwell-relations)
- [Mayer's relation](ideal-gas.md#mayer-s-relation)
- [Mechanical input and thermal storage in a calorimeter](thermodynamics.md#mechanical-input-and-thermal-storage-in-a-calorimeter)
- [Normalizing extensive quantities](thermodynamics.md#normalizing-extensive-quantities)
- [Ohm's law](electric-charge.md#ohm-s-law)
- [Paddle-wheel calorimetry energy balance](#paddle-wheel-calorimetry-energy-balance)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018.md#section-b/b2/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019.md#section-b/5/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2.md#a6/b/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2.md#a6/c/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2.md#a6/e/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2.md#a8/b/i/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-2.md#a8/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2.md#a6/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2.md#a6/b/i/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#5/c/v/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/b/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/d/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2012/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2013/paper-1.md#2/solution)
- [Solution](past-exam-of-the-genetics-course-of-the-university-of-cambridge/2024/paper-1.md#7/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-78.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1.md#4b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-54.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#9b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#9b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#9b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#34d/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#34d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#34d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-314.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-314.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#35d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#35a/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#35a/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#39c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#9/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#section-b/5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#17/a/solution)
- [Solution](past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2015/paper-1.md#1/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c11/a-internal-energy/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c11/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2.md#section-c/c11/solution)
- [Solution (film calculations)](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c11/solution-film-calculations)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c10/heat-exchanges-and-efficiency/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c11/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c11/equations-of-state-and-transitions/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c10/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c10/adiabatic-temperature-and-energy-changes/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c10/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c10/free-energy-identity/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c12/diffusion-with-a-heat-source/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-a/a1/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2.md#section-c/c9/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-a/a3/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b2/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b2/d/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2014/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#2/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#3/b/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/5/solution)
- [Photon rocket](momentum.md#photon-rocket)
- [Pressure](pressure.md)
- [Pressure-confined singular isothermal gas sphere](galaxy.md#pressure-confined-singular-isothermal-gas-sphere)
- [Quasistatic process](thermodynamics.md#quasistatic-process)
- [Radiation pressure](pressure.md#radiation-pressure)
- [Radiative cooling](heat.md#radiative-cooling)
- [Relativistic rocket equation](momentum.md#relativistic-rocket-equation)
- [Simple compressible system](thermodynamics.md#simple-compressible-system)
- [Specific heat capacity at constant pressure](heat.md#specific-heat-capacity-at-constant-pressure)
- [Specific internal energy](#specific-internal-energy)
- [State function](thermodynamics.md#state-function)
- [Statistical physics](statistical-physics.md)
- [Steady-flow energy balance](enthalpy.md#steady-flow-energy-balance)
- [Stirling engine](thermodynamics.md#stirling-engine)
- [Stratified mixing energy budget](turbulence.md#stratified-mixing-energy-budget)
- [Surface energy](surface-tension.md#surface-energy)
- [Temperature](temperature.md)
- [Temperature sensitivity of a free-expansion experiment](thermodynamics.md#temperature-sensitivity-of-a-free-expansion-experiment)
- [Thermal boundary resistance](temperature.md#thermal-boundary-resistance)
- [Thermal conduction](heat.md#thermal-conduction)
- [Thermal diffusivity](heat.md#thermal-diffusivity)
- [Thermal equilibration of two finite bodies](thermal-equilibrium.md#thermal-equilibration-of-two-finite-bodies)
- [Thermal equilibrium](thermal-equilibrium.md)
- [Thermodynamic force conjugate to an internal variable](continuum-mechanics.md#thermodynamic-force-conjugate-to-an-internal-variable)
- [Thermodynamic free energy](thermodynamic-potential.md#thermodynamic-free-energy)
- [Thermodynamic internal pressure](#thermodynamic-internal-pressure)
- [Thermodynamic potential](thermodynamic-potential.md)
- [Thermodynamic system](thermodynamics.md#thermodynamic-system)
- [Thermodynamics](thermodynamics.md)
- [Thermodynamics of a liquid film](surface-tension.md#thermodynamics-of-a-liquid-film)
- [Three-dimensional free-electron density of states](quantum-ideal-gas-statistics.md#three-dimensional-free-electron-density-of-states)
- [Two-dimensional ideal gas](ideal-gas.md#two-dimensional-ideal-gas)
- [Two-level paramagnetic cooling model](temperature.md#two-level-paramagnetic-cooling-model)
- [Two-point thermometer calibration example](thermodynamics.md#two-point-thermometer-calibration-example)
- [Two reversible ideal-gas paths between the same states](thermodynamics.md#two-reversible-ideal-gas-paths-between-the-same-states)
- [Van der Waals throttling model](enthalpy.md#van-der-waals-throttling-model)
- [Vibrational partition function](canonical-ensemble.md#vibrational-partition-function)
- [Volume derivative form of the heat-capacity difference](enthalpy.md#volume-derivative-form-of-the-heat-capacity-difference)
- [Zeroth law of thermodynamics](thermodynamics.md#zeroth-law-of-thermodynamics)
