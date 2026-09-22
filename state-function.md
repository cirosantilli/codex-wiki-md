# State function

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/State_function)

A [state function](state-function.md) assigns a value to each equilibrium [thermodynamic state](thermodynamic-state.md) of a specified [thermodynamic system](thermodynamic-system.md). Its change depends only on the initial and final states. [Internal energy](internal-energy-split.md) $U$, [entropy](entropy-split.md) $S$ and [enthalpy](enthalpy-split.md) $H=U+pV$ are [state functions](state-function.md); here $p$ is [pressure](pressure-split.md) and $V$ is [volume](volume-thermodynamics.md). Transferred [heat](heat-split.md) $Q$ and [work](work.md) $W$ belong to a [thermodynamic process](thermodynamic-process.md), rather than to a state. A system stores [internal energy](internal-energy-split.md); it does not store separate inventories of “heat received” and “work received”.[Thermodynamics and Propulsion, §2.1, points 3–5 and equation 2.2: internal energy, transfer notation and signs](thermodynamics-and-propulsion.md)

Use the explicit convention $Q>0$ for [heat](heat-split.md) entering and $W_{\rm by}>0$ for [work](work.md) done by the [thermodynamic system](thermodynamic-system.md) on its surroundings. For a [closed system](closed-system.md) with unchanged endpoint bulk [kinetic energy](kinetic-energy.md) and external [potential energy](potential-energy.md), the [first law of thermodynamics](first-law-of-thermodynamics-split.md) reads

$$
\Delta U=Q-W_{\rm by},\qquad dU=\delta Q-\delta W_{\rm by}.
$$

The notation $dU$ denotes an [exact differential](exact-differential.md) of a [state function](state-function.md); $\delta Q$ and $\delta W_{\rm by}$ denote incremental transfers. Along a [reversible thermodynamic process](reversible-thermodynamic-process.md) of a [simple compressible system](simple-compressible-system.md),

$$
\delta W_{\rm by,rev}=p\,dV,\qquad \delta Q_{\rm rev}=T\,dS,
$$

where $T$ is absolute [temperature](temperature-split.md). These are rules for particular [thermodynamic processes](thermodynamic-process.md), not definitions of stored [heat](heat-split.md) or stored [work](work.md). In particular, a [quasistatic process](quasistatic-process.md) with [friction](friction.md) can remain near [thermodynamic equilibrium](thermodynamic-equilibrium.md) while producing [entropy](entropy-split.md).[Thermodynamics and Propulsion, §5.3: reversible transfer formulas distinguished from relations between state properties](thermodynamics-and-propulsion.md)

For any [state function](state-function.md) $F$ and two equilibrium states $A,B$, an [integral](integral-split.md) of its [exact differential](exact-differential.md) gives

$$
\int_{A}^{B}dF=F(B)-F(A),\qquad \oint dF=0.
$$

The proof is telescoping: add the changes $F(x_{i+1})-F(x_i)$ along a subdivided path, and all intermediate values cancel. The smooth limit gives the [integral](integral-split.md). Conversely, if an integrable [differential form](differential-form-split.md) has zero [integral](integral-split.md) around every accessible closed path in a connected region, define $F(B)$ by integrating from a reference state. Two routes differ by a closed path, so the definition is unambiguous. This argument needs every accessible loop, rather than a local test that might miss a hole in the domain; see [path independence](path-independence.md).

The same cancellation does not hold separately for [heat](heat-split.md) and [work](work.md). A [thermodynamic cycle](thermodynamic-cycle.md) has $\Delta U=0$ but can have nonzero net transfers, with $\oint\delta Q=\oint\delta W_{\rm by}$. Nor does the fact that [entropy](entropy-split.md) is a [state function](state-function.md) make $Q/T$ its general change: the formula $dS=\delta Q_{\rm rev}/T$ uses a [reversible thermodynamic process](reversible-thermodynamic-process.md) and its varying [temperature](temperature-split.md).

This distinction makes endpoint calculations powerful. We can compute an [internal energy](internal-energy-split.md), [entropy](entropy-split.md) or [enthalpy](enthalpy-split.md) difference along a convenient reversible reference path even when the actual [thermodynamic process](thermodynamic-process.md) is irreversible. Its actual [heat](heat-split.md) and [work](work.md) must still be obtained from its own boundary interactions. The appealing cancellation is visible in [two reversible ideal-gas paths between the same states](two-reversible-ideal-gas-paths-between-the-same-states.md): a different mechanical output requires a matching difference in thermal input, while stored [internal energy](internal-energy-split.md) arrives at the same value.

**Table of contents**

- [Two reversible ideal-gas paths between the same states](two-reversible-ideal-gas-paths-between-the-same-states.md)
- [Mechanical input and thermal storage in a calorimeter](mechanical-input-and-thermal-storage-in-a-calorimeter.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (29)

- [ATP-driven sugar phosphorylation](atp-driven-sugar-phosphorylation.md)
- [ATP synthase energy and proton budget](atp-synthase-energy-and-proton-budget.md)
- [Born-Haber cycle](born-haber-cycle.md)
- [Chemiosmosis](chemiosmosis.md)
- [Energy coupling](energy-coupling.md)
- [Enthalpy](enthalpy-split.md)
- [Entropy](entropy-split.md)
- [Entropy change in free expansion](entropy-change-in-free-expansion.md)
- [First law of thermodynamics](first-law-of-thermodynamics-split.md)
- [Gibbs-Duhem equation](gibbs-duhem-equation.md)
- [Heat](heat-split.md)
- [Heat capacity](heat-capacity.md)
- [Hess's law](hess-s-law.md)
- [Hess's law calorimetry experiment](hess-s-law-calorimetry-experiment.md)
- [Internal energy](internal-energy-split.md)
- [Isothermal expansion](isothermal-expansion.md)
- [Joule-Thomson coefficient](joule-thomson-coefficient.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Maxwell relations](maxwell-relations.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-a/a3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b8/solution.md)
- [Quasistatic process](quasistatic-process.md)
- [State function](state-function.md)
- [Thermodynamic free energy](thermodynamic-free-energy.md)
- [Thermodynamic potential](thermodynamic-potential-split.md)
- [Thermodynamic process](thermodynamic-process.md)
- [Thermodynamics](thermodynamics-split.md)
- [Two reversible ideal-gas paths between the same states](two-reversible-ideal-gas-paths-between-the-same-states.md)
