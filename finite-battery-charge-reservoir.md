# Finite battery charge reservoir

↑ **Parent:** [Electric battery](electric-battery.md)

A [battery](electric-battery.md)'s charge reservoir means a finite amount of [electric charge](electric-charge-split.md) can pass through the external [electrical circuit](electrical-circuit-split.md) before its usable chemical state is depleted. It does not mean a large net [electric charge](electric-charge-split.md) is sitting inside the casing. For one net cell [chemical reaction](chemical-reaction-split.md) transferring $n$ [electrons](electron.md) per reaction event, an ideal reaction inventory obeys

$$
Q_{\rm delivered}=\int_0^t I(t')\,dt'=nF\xi,\qquad
W_L=\int_0^t V_L(t')I(t')\,dt',
$$

where $F$ is the [Faraday constant](faraday-constant.md) and $\xi$ the [extent of reaction](extent-of-reaction.md) in [moles](mole-unit.md), assuming all the [electric current](electric-current.md) serves that reaction. At fixed [temperature](temperature-split.md) and [pressure](pressure-split.md), its reversible [electromotive force](electromotive-force.md) obeys $\Delta_rG=-nF\mathcal E$: a decrease in [Gibbs free energy](gibbs-free-energy.md) provides the maximum reversible electrical [work](work.md) per [mole](mole-unit.md). The [electromotive force](electromotive-force.md) also depends on composition; the [Daniell cell](daniell-cell.md) illustrates this with [thermodynamic activity](thermodynamic-activity.md).[§17.4, E° and ΔG°, and Potentials at Nonstandard Conditions: free energy, cell potential and composition](chemistry-2e-by-paul-flowers-and-others/17-4-potential-free-energy-and-equilibrium.md)

As an original finite-reservoir exercise, stipulate usable $Q_{\max}=360\,\mathrm C$ and hold the preceding $3\,\mathrm V$, $1\,\Omega$, $4\,\Omega$ parameters constant until an abrupt cutoff. Then $t=Q_{\max}/I=600\,\mathrm s$, available electrical [work](work.md) is $\mathcal E Q_{\max}=1080\,\mathrm J$, load [work](work.md) is $V_LQ_{\max}=864\,\mathrm J$, and internal dissipation is $216\,\mathrm J$. This explicitly finite idealization predicts ten minutes, not an experimentally measured runtime. Real accessible charge depends on discharge conditions and the chosen terminal-voltage cutoff. Charge alone is also not an [energy](energy-split.md): converting it to delivered [work](work.md) requires the terminal [electric potential difference](electric-potential-difference.md) throughout discharge.

## ↑ Ancestors (6)

1. [Electric battery](electric-battery.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
