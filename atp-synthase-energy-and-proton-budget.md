# ATP synthase energy and proton budget

↑ **Parent:** [ATP synthase](atp-synthase.md)

Define side $P$ as the higher [proton](proton.md) [electrochemical potential](electrochemical-potential.md) reservoir and side $N$ as the synthesis-side reservoir. For transfer $P\to N$ at common [temperature](temperature-split.md) $T$, define the positive downhill [proton-motive force](proton-motive-force.md) magnitude $\Delta p_{\rm drive}$ by

$$
\Delta\widetilde\mu_{P\to N}
=RT\ln\frac{a_N}{a_P}+F(\psi_N-\psi_P)
=-F\Delta p_{\rm drive}.
$$

Here $a$ is [thermodynamic activity](thermodynamic-activity.md), $\psi$ is [electric potential](electric-potential.md), $R$ is the [molar gas constant](molar-gas-constant.md) and $F$ is the [Faraday constant](faraday-constant.md). Thus both a higher [proton](proton.md) [thermodynamic activity](thermodynamic-activity.md) and a more positive [electric potential](electric-potential.md) on side $P$ contribute to the driving magnitude. This definition fixes the sign; conventions for a signed [proton-motive force](proton-motive-force.md) differ. The calculation under [chemiosmosis](chemiosmosis.md) separates these two contributions numerically.

Assume fixed reservoirs, tight mechanical [energy coupling](energy-coupling.md), one transported [proton](proton.md) per $c$ subunit per revolution, and three [ATP](adenosine-triphosphate.md) produced per revolution. Neglect leaks, slipping and [membrane transport](membrane-transport.md) of the chemical reagents. Let $g_{\rm ATP}>0$ be the local molar [Gibbs free energy](gibbs-free-energy.md) cost of [ATP](adenosine-triphosphate.md) formation at the stipulated composition, [pH](ph.md) and [magnesium](magnesium.md)-binding convention. It is not necessarily the [standard state](standard-state.md) value. Adding changes in the [state function](state-function.md) gives, per mole of complete turns,

$$
\Delta G_{\rm turn}=3g_{\rm ATP}-nF\Delta p_{\rm drive}.
$$

For this model net synthesis is thermodynamically favoured when $\Delta G_{\rm turn}<0$. Equality is a reversible balance, not a promise of a useful [reaction rate](reaction-rate.md). A negative value establishes an available driving margin; it does not specify how fast the [enzyme](enzyme-split.md) runs.

Choose $n=10$, $g_{\rm ATP}=50.0\,\mathrm{kJ\,mol^{-1}}$, $F=96485\,\mathrm{C\,mol^{-1}}$ and $\Delta p_{\rm drive}=0.180\,\mathrm V$. These are illustrative inputs, not measurements of the preparation in the experiment below. Then

$$
nF\Delta p_{\rm drive}=173.673\,\mathrm{kJ\,mol^{-1}},\qquad
3g_{\rm ATP}=150.0\,\mathrm{kJ\,mol^{-1}},
$$

and $\Delta G_{\rm turn}=-23.673\,\mathrm{kJ\,mol^{-1}}$. Per [ATP](adenosine-triphosphate.md), the ideal input is $57.891\,\mathrm{kJ\,mol^{-1}}$, leaving a driving margin of $7.891\,\mathrm{kJ\,mol^{-1}}$. The balance point is

$$
\Delta p_* =\frac{3g_{\rm ATP}}{nF}\approx0.15546\,\mathrm V.
$$

At $0.140\,\mathrm V$ the same synthesis cycle instead has $\Delta G_{\rm turn}=+14.921\,\mathrm{kJ\,mol^{-1}}$: the chosen reservoirs favour its reverse.

<a id="image-chosen-ten-subunit-model-the-free-energy-balance-determines-the-favoured-direction"></a>
![](atp-synthase-energy-coupling.png)

**[Figure 8](#image-chosen-ten-subunit-model-the-free-energy-balance-determines-the-favoured-direction). Chosen ten-subunit model: the free energy balance determines the favoured direction**. Original calculation, not experimental data. Fixed $g_{\rm ATP}=50$ kJ/mol, three [ATP](adenosine-triphosphate.md) per turn, no leak or reagent transport. The second panel adds an explicitly hypothetical one-[proton](proton.md)-equivalent transport cost per delivered [ATP](adenosine-triphosphate.md).

The machine is reversible: sufficient [ATP](adenosine-triphosphate.md) [hydrolysis](hydrolysis.md) can drive opposite rotation and pump [protons](proton.md) uphill. Actual direction also depends on inhibition and available [substrates](substrate-biochemistry.md); a weak [proton-motive force](proton-motive-force.md) need not make every intact [enzyme](enzyme-split.md) immediately run backward. [Respiratory uncoupling](respiratory-uncoupling.md) supplies a different failure mode: a parallel [proton](proton.md) leak dissipates the gradient without productive shaft rotation.[Watanabe, 2013, p. 51 and Figure 2: reversal of the coupled motors](rotary-catalysis-of-fof1-atp-synthase-by-rikiya-watanabe.md)

The motor budget $10/3$ is not the whole cost of [ATP](adenosine-triphosphate.md) delivered outside a [mitochondrion](mitochondria.md). Import of [ADP](adenosine-diphosphate.md) and [inorganic phosphate](inorganic-phosphate.md), and export of [ATP](adenosine-triphosphate.md), also draw on the [electrochemical gradient](electrochemical-gradient.md).[Cooper, The Cell: A Molecular Approach, 2nd edition, Transport of Metabolites across the Inner Membrane, Figure 10.12](the-cell-a-molecular-approach-2nd-edition-by-geoffrey-m-cooper/the-mechanism-of-oxidative-phosphorylation.md) For a deliberately simplified system budget, assign these transports together one additional downhill-[proton](proton.md) equivalent per delivered [ATP](adenosine-triphosphate.md), valued at the same $F\Delta p_{\rm drive}$. This is a chosen accounting convention, not a claim of one extra literal [proton](proton.md) through $F_0$, nor a universal transport [stoichiometry](stoichiometry.md). The total becomes $10/3+1=13/3$ equivalents and $75.258\,\mathrm{kJ\,mol^{-1}}$ of gradient expenditure per delivered [ATP](adenosine-triphosphate.md) at $0.180\,\mathrm V$. The ratio of stored chemical [free energy](thermodynamic-free-energy.md) to that expenditure is $50/75.258\approx66.4\%$, compared with $50/57.891\approx86.4\%$ for the motor alone. This system budget changes the resource expenditure, not the motor's balance point $\Delta p_*$. Real transport terms require their own [electrochemical potentials](electrochemical-potential.md), and leaks add further cost.

## ↑ Ancestors (4)

1. [ATP synthase](atp-synthase.md)
2. [Enzyme](enzyme-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)
