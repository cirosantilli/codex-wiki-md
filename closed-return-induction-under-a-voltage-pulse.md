# Closed-return induction under a voltage pulse

↑ **Parent:** [Coupled RL induction model](coupled-rl-induction-model.md)

Apply $V_0$ for $0\leq t<T$ and then set the drive to zero while retaining the closed primary return. By [superposition](superposition-principle.md), each pulse-response [electric current](electric-current.md) is its [equal-loop RL induction step](equal-loop-rl-induction-step.md) response at $t$ minus that response at $t-T$, with the step response defined as zero before its onset. All currents remain continuous at $T$; the drive changes their [derivatives](derivative.md).

<a id="image-calculated-induction-transients-and-magnetic-energy-in-a-closed-return-rl-model"></a>
![](coupled-rl-voltage-pulse-and-energy.png)

**[Figure 5](#image-calculated-induction-transients-and-magnetic-energy-in-a-closed-return-rl-model). Calculated induction transients and magnetic energy in a closed-return RL model**. [Source](coupled-rl-voltage-pulse-and-energy.py). The applied voltage lasts $120\,\mathrm{ms}$. Currents are exact linear-model calculations. The lower-right panel compares the magnetic energy computed from the currents with source work minus Joule heat, obtained by separate analytic integrations. No curves are historical measurements or galvanometer needle traces.

For the displayed pulse, the secondary responds negatively as the primary builds and positively as it decays. Between these transients, the primary is almost steady and the secondary is almost quiet. The [energy balance of coupled RL circuits](energy-balance-of-coupled-rl-circuits.md) accounts for the entire process, including the [energy](energy-split.md) remaining in the [magnetic field](magnetic-field-split.md) when the drive changes.

## ↑ Ancestors (8)

1. [Coupled RL induction model](coupled-rl-induction-model.md)
2. [Faraday induction-ring experiment](faraday-induction-ring-experiment.md)
3. [Faraday's law of induction](faraday-s-law-of-induction.md)
4. [Maxwell equations](maxwell-equations-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
