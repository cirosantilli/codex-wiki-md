# Free expansion

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)

Free expansion occurs when a [gas](gas.md) spreads into an initially evacuated region without driving an external load. The standard idealization uses a rigid, insulated vessel: initially a partition confines the [gas](gas.md) to [volume](volume-thermodynamics.md) $V_1$, while the remaining compartment contains [vacuum](vacuum.md). Open a passage and wait for [thermodynamic equilibrium](thermodynamic-equilibrium.md); the same fixed [amount of substance](amount-of-substance.md) $n$ now occupies the larger accessible [volume](volume-thermodynamics.md) $V_2$. The outer vessel never changes size. This simple release separates three questions: what [energy](energy.md) is conserved, whether [temperature](temperature.md) changes, and why [entropy](entropy.md) increases. [Free Expansion of Gas](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/free-expansion-of-gas.md)

<a id="image-free-expansion-changes-the-accessible-volume-thermodynamics-the-apparatus-affects-the-observed-temperature"></a>
![](free-expansion-vessel-and-thermometry.png)

**[Figure 9](#image-free-expansion-changes-the-accessible-volume-thermodynamics-the-apparatus-affects-the-observed-temperature). Free expansion changes the accessible volume; the apparatus affects the observed temperature**. Original schematic, with equal compartments chosen for illustration. The top row assumes an insulated [gas](gas.md) with negligible wall [heat capacity](heat-capacity.md). The bottom left sketches the water-bath arrangement of [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md), rather than a reconstruction to scale. The bottom right uses stipulated [heat capacities](heat-capacity.md) and an illustrative [energy](energy.md) demand to show signal suppression; it contains no measured data.

Choose the [gas](gas.md) as the [closed system](closed-system.md), neglect [heat](heat.md) exchange with the walls, and assume negligible changes in bulk [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md) between the equilibrium endpoints. Insulation gives $Q_{\rm in}=0$; no moving outer boundary or external load receives [work](work.md), so $W_{\rm out}=0$. The [first law of thermodynamics](first-law-of-thermodynamics.md) therefore gives

$$
\Delta U=Q_{\rm in}-W_{\rm out}=0.
$$

The gas can develop internal motion during the release; this does not supply external [work](work.md). The intermediate state need not have one equilibrium [pressure](pressure.md) or [temperature](temperature.md), so there is no actual [quasistatic process](quasistatic-process.md) curve $p(V)$ to integrate. In particular, substituting the equilibrium [ideal gas law](ideal-gas-law.md) into $\int p\,dV$ would describe a different process. [OpenStax, section 4.1: free expansion and the absence of equilibrium intermediate states](https://openstax.org/books/university-physics-volume-2/pages/4-1-reversible-and-irreversible-processes)

For an [ideal gas](ideal-gas.md), [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md) depends only on [temperature](temperature.md). With positive [heat capacity at constant volume](heat-capacity-at-constant-volume.md), $U(T_2)=U(T_1)$ implies $T_2=T_1$, and the [ideal gas law](ideal-gas-law.md) gives $p_2/p_1=V_1/V_2$. Doubling the accessible [volume](volume-thermodynamics.md) thus halves the final [pressure](pressure.md) without changing the final [temperature](temperature.md). This is an endpoint statement; it does not assert a spatially uniform, constant [temperature](temperature.md) during the rush. Insulation alone does not imply constant [temperature](temperature.md): a reversible [adiabatic expansion](adiabatic-expansion.md) cools an [ideal gas](ideal-gas.md) because it supplies [work](work.md). [4 Classical Thermodynamics](statistical-physics-by-david-tong/4-classical-thermodynamics.md)

For a [real gas](real-gas.md), $U(T,V)$ can depend on [volume](volume-thermodynamics.md) as well as [temperature](temperature.md), so unchanged [internal energy](internal-energy.md) need not mean unchanged [temperature](temperature.md). For a fixed-composition [simple compressible system](simple-compressible-system.md) in a single [thermodynamic phase](thermodynamic-phase.md), equilibrium identities using a [Maxwell relation](maxwell-relations.md) give

$$
dU=C_V\,dT+\left[T\left(\frac{\partial p}{\partial T}\right)_V-p\right]dV,
\qquad
\left(\frac{\partial T}{\partial V}\right)_U=
\frac{p-T(\partial p/\partial T)_V}{C_V}.
$$

Here $C_V$ is the whole sample's [heat capacity at constant volume](heat-capacity-at-constant-volume.md). The sign depends on the [equation of state](equation-of-state.md); for an [ideal gas](ideal-gas.md) the numerator vanishes. For a finite [free expansion](free-expansion.md), solve $U(T_2,V_2)=U(T_1,V_1)$, or integrate this slope along equilibrium states of equal [internal energy](internal-energy.md); that mathematical curve does not describe the actual release. [Free Expansion of Gas](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/free-expansion-of-gas.md)

Free expansion is useful because it tests how [internal energy](internal-energy.md) depends on [number density](number-density.md) while eliminating external expansion [work](work.md). Its beautiful surprise is that an [ideal gas](ideal-gas.md) can finish with the same [temperature](temperature.md) and [internal energy](internal-energy.md) but greater [entropy](entropy.md): a [thermometer](thermometer.md) alone cannot diagnose reversibility. See [entropy change in free expansion](entropy-change-in-free-expansion.md) for the calculation and [temperature sensitivity of a free-expansion experiment](temperature-sensitivity-of-a-free-expansion-experiment.md) for the experimental qualification. The continuous-flow throttling associated with the [Joule-Thomson coefficient](joule-thomson-coefficient.md) has a different balance: under its usual assumptions it preserves [enthalpy](enthalpy.md), whereas the gas-only idealization here preserves [internal energy](internal-energy.md). [Fitzpatrick, Joule-Thompson Throttling: steady-flow enthalpy balance](https://farside.ph.utexas.edu/teaching/sm1/Thermalhtml/node68.html)

**Table of contents**

- [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)
  - [Temperature sensitivity of a free-expansion experiment](temperature-sensitivity-of-a-free-expansion-experiment.md)
- [Entropy change in free expansion](entropy-change-in-free-expansion.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Adiabatic expansion](adiabatic-expansion.md)
- [Adiabatic process](adiabatic-process.md)
- [Boltzmann entropy when a restriction is removed](boltzmann-entropy-when-a-restriction-is-removed.md)
- [Entropy change in free expansion](entropy-change-in-free-expansion.md)
- [First law of thermodynamics](first-law-of-thermodynamics.md)
- [Free expansion](free-expansion.md)
- [Isothermal expansion](isothermal-expansion.md)
- [Isothermal ideal-gas work](isothermal-ideal-gas-work.md)
- [Isothermal process](isothermal-process.md)
- [Maxwell relations](maxwell-relations.md)
- [Quasistatic process](quasistatic-process.md)
- [Second law of thermodynamics](second-law-of-thermodynamics.md)
