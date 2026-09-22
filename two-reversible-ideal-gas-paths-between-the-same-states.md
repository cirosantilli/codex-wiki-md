# Two reversible ideal-gas paths between the same states

↑ **Parent:** [State function](state-function.md)

Take a [closed system](closed-system.md) consisting of one [mole](mole-unit.md) of a classical [monatomic gas](monatomic-gas.md), idealized as an [ideal gas](ideal-gas-split.md) with constant [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V=3nR/2$. Stipulate [amount of substance](amount-of-substance.md) $n=1\,\mathrm{mol}$ and [molar gas constant](molar-gas-constant.md) $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$ for this calculation. Set initial [temperature](temperature-split.md) $T_0=300\,\mathrm K$ and [volume](volume-thermodynamics.md) $V_0=0.010\,\mathrm{m^3}$, and define $E_0=nRT_0=2.4942\,\mathrm{kJ}$ and $p_0=E_0/V_0=249.42\,\mathrm{kPa}$. The specified equilibrium endpoints are

$$
A:(V,T,p)=(V_0,T_0,p_0),\qquad
B:(V,T,p)=(3V_0,2T_0,2p_0/3).
$$

Thus $B$ has [volume](volume-thermodynamics.md) $0.030\,\mathrm{m^3}$, [temperature](temperature-split.md) $600\,\mathrm K$ and [pressure](pressure-split.md) $166.28\,\mathrm{kPa}$. The fixed material inventory and [ideal gas law](ideal-gas-law.md) make these complete endpoint specifications for this model. All numbers below are calculated values, rather than measurements of a particular [gas](gas.md).

Use a frictionless piston, ignore bulk mechanical [energy](energy-split.md) changes, and allow only [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) [work](work.md). Each step is the limit of a [reversible thermodynamic process](reversible-thermodynamic-process.md): adjust loads by infinitesimal [pressure](pressure-split.md) differences, and supply [heat](heat-split.md) through infinitesimal [temperature](temperature-split.md) differences. Heating with changing [temperature](temperature-split.md) requires a succession of matching [thermal reservoirs](heat-bath.md); contact with a single hotter [heat bath](heat-bath.md) would give an irreversible finite difference. On a fixed-[volume](volume-thermodynamics.md) leg the piston is locked. These assumptions justify using the actual equilibrium path's [pressure](pressure-split.md) in

$$
W_{\rm by,rev}=\int_{\rm path}p\,dV.
$$

An endpoint chord is not the path; substituting a guessed straight line would compute a different [thermodynamic process](thermodynamic-process.md).[Thermodynamics and Propulsion, §1.3.3, Figures 1.10–1.11: external pressure versus equilibrium gas pressure in boundary work](thermodynamics-and-propulsion.md)

The upper route heats at fixed [volume](volume-thermodynamics.md) from $A$ to $C=(V_0,2T_0,2p_0)$, then undergoes [isothermal expansion](isothermal-expansion.md) at $2T_0$ to $B$. The lower route undergoes [isothermal expansion](isothermal-expansion.md) at $T_0$ from $A$ to $D=(3V_0,T_0,p_0/3)$, then heats at fixed [volume](volume-thermodynamics.md) to $B$. The tuples use the same $(V,T,p)$ ordering as the endpoints. Vertical legs do zero expansion [work](work.md), and the two curved legs have different [pressures](pressure-split.md) at every shared intermediate [volume](volume-thermodynamics.md).

<a id="image-two-reversible-ideal-gas-paths-connect-the-same-equilibrium-endpoints"></a>
![](state-function-two-paths-pv.png)

**[Figure 3](#image-two-reversible-ideal-gas-paths-connect-the-same-equilibrium-endpoints). Two reversible ideal gas paths connect the same equilibrium endpoints**. Original idealized [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) diagram. The upper route is $A\to C\to B$ and the lower route is $A\to D\to B$; the shaded gap is the difference in [work](work.md), not an experimental uncertainty. Both are [reversible thermodynamic processes](reversible-thermodynamic-process.md) under the stated piston and [thermal reservoir](heat-bath.md) assumptions.

The [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md) gives the same endpoint difference for both routes:

$$
\Delta U=\frac32nR(2T_0-T_0)=\frac32E_0=3.7413\,\mathrm{kJ}.
$$

On either fixed-[volume](volume-thermodynamics.md) heating leg, $W_{\rm by}=0$ and $Q=3E_0/2$. On each [isothermal expansion](isothermal-expansion.md), $\Delta U=0$, so the [first law of thermodynamics](first-law-of-thermodynamics-split.md) gives $Q=W_{\rm by}$. The [ideal gas law](ideal-gas-law.md) and the [integral](integral-split.md) of $1/V$ then give

$$
\begin{aligned}
W_{\rm by,upper}&=\int_{V_0}^{3V_0}\frac{2E_0}{V}\,dV=2E_0\ln3, & Q_{\rm upper}&=\frac32E_0+2E_0\ln3,\\
W_{\rm by,lower}&=\int_{V_0}^{3V_0}\frac{E_0}{V}\,dV=E_0\ln3, & Q_{\rm lower}&=\frac32E_0+E_0\ln3.
\end{aligned}
$$

Here $\ln$ is the [natural logarithm](natural-logarithm.md). Rounded to $0.001\,\mathrm{kJ}$, the upper route has $(Q,W_{\rm by},\Delta U)=(9.222,5.480,3.741)\,\mathrm{kJ}$ and the lower route has $(6.481,2.740,3.741)\,\mathrm{kJ}$. Subtracting separately rounded entries can differ by $0.001\,\mathrm{kJ}$; the unrounded balances are exact in the stipulated model.

<a id="image-different-heat-and-work-transfers-leave-the-same-internal-energy-increment"></a>
![](state-function-two-paths-energy-ledger.png)

**[Figure 4](#image-different-heat-and-work-transfers-leave-the-same-internal-energy-increment). Different heat and work transfers leave the same internal energy increment**. Original calculated [energy](energy-split.md) ledger for the two reversible paths. Each incoming [heat](heat-split.md) bar is divided into outgoing [work](work.md) and the common stored increment $\Delta U$. Labels are rounded; bar lengths use unrounded values. These are process totals, not inventories of stored [heat](heat-split.md) or stored [work](work.md).

The shaded [area](surface-area.md) between the curves explains the entire difference:

$$
W_{\rm by,upper}-W_{\rm by,lower}
=Q_{\rm upper}-Q_{\rm lower}
=E_0\ln3\approx2.740159\,\mathrm{kJ}.
$$

Following the upper route forward and the lower route backward makes a [thermodynamic cycle](thermodynamic-cycle.md) with this positive net [work](work.md) and matching net [heat](heat-split.md). Its [internal energy](internal-energy-split.md) change is zero. The two open routes themselves are reversible, so their different [work](work.md) outputs should not be mistaken for a loss caused by [entropy production](entropy-production.md): they receive different [heat](heat-split.md) transfers at different [temperatures](temperature-split.md).

Two other [state functions](state-function.md) provide independent endpoint checks. With [enthalpy](enthalpy-split.md) $H=5nRT/2$ in this model,

$$
\Delta H=\frac52E_0=6.2355\,\mathrm{kJ},\qquad
\Delta S=\frac32nR\ln2+nR\ln3\approx17.7781\,\mathrm{J\,K^{-1}}.
$$

To obtain the [entropy](entropy-split.md) change along either route, integrate $C_V\,dT/T$ on its heating leg, giving $C_V\ln2$, and $nR\,dV/V$ on its [isothermal expansion](isothermal-expansion.md), giving $nR\ln3$. Reordering the legs changes their [heat](heat-split.md) totals but leaves the sum of their [entropy](entropy-split.md) changes unchanged. In particular, neither route's total $Q$ divided by its final [temperature](temperature-split.md) equals $\Delta S$, and neither total $Q$ equals $\Delta H$: both routes include an [isothermal expansion](isothermal-expansion.md), rather than a single fixed-[pressure](pressure-split.md) heating step.

## ↑ Ancestors (6)

1. [State function](state-function.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Mechanical input and thermal storage in a calorimeter](mechanical-input-and-thermal-storage-in-a-calorimeter.md)
- [State function](state-function.md)
