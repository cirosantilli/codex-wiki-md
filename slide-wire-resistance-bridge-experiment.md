# Slide-wire resistance bridge experiment

↑ **Parent:** [Wheatstone bridge](wheatstone-bridge.md)

PHYWE's documented experiment uses a one-metre slide wire, a connection box, an unknown [resistor](resistor.md), a known comparison [resistor](resistor.md), a supply, and a digital multimeter in steady-current mA mode as the null detector. Its two yellow detector leads join the fixed-resistor junction and the slider. Move the slider until the indicated [electric current](electric-current.md) vanishes; read the two wire [lengths](length.md) on the ruler and infer the unknown [electrical resistance](electrical-resistance.md) from their ratio. The guide advises changing the comparison [resistor](resistor.md) if no null is reachable or the slider lies near an end.[PHYWE, P2410200, pp. 6–8: equipment, Figure 4 wiring, and Procedure (1/6)](wheatstone-bridge-by-phywe-p2410200.md)

The inference requires uniform [electrical resistivity](electrical-resistivity.md) and [wire cross-sectional area](wire-cross-sectional-area.md), so the two wire [electrical resistances](electrical-resistance.md) have the ratio of their [lengths](length.md), by $R=\rho_{\mathrm{el}}L/A$. Retaining PHYWE's labeling, its equation (6) is $R_x=R_C\ell_1/\ell_2$, where $R_C$ is the comparison [electrical resistance](electrical-resistance.md). This is a different arm placement from our schematic. The guide's example table reports larger discrepancies near wire ends.[PHYWE, P2410200, p. 5, equation (6), and p. 12, Table 1 and end-position discussion](wheatstone-bridge-by-phywe-p2410200.md)

Useful additional controls distinguish a true [null measurement](null-measurement.md) from an insensitive or disconnected detector. Check the detector zero with the supply off, then move the adjustable arm slightly to either side of the candidate balance and verify opposite detector signs. Reconnect the unknown with short, secure leads and repeat the balance. Any lead or contact [electrical resistance](electrical-resistance.md) included in that arm contributes to the inferred value, even though a detector lead carries no [electric current](electric-current.md) at exact balance. For very small unknown [electrical resistances](electrical-resistance.md), [four-terminal sensing](four-terminal-sensing.md) addresses this separate connection problem; a detector null alone does not remove it.

Check for [Joule heating](joule-heating.md) by repeating at lower supply [electric potential difference](electric-potential-difference.md) and with shorter powered intervals, holding ambient [temperature](temperature.md) fixed. At balance the unknown still dissipates [power](power.md)

$$
P_x=\left(\frac{V_s}{R_3+R_x}\right)^2R_x.
$$

Halving $V_s$ quarters this [power](power.md) while halving ideal detector sensitivity. A balance that moves with excitation or elapsed [time](time-in-physics.md) suggests changing [electrical resistance](electrical-resistance.md), including self-heating; it is not explained by passive detector loading alone. These are proposed controls, not claimed outcomes of PHYWE's experiment. Standard-[resistor](resistor.md) accuracy, wire uniformity, contact reproducibility and finite detector resolution still limit the [electrical measurement](electrical-measurement.md). Large [electrical resistances](electrical-resistance.md) also make unwanted leakage paths consequential.

## ↑ Ancestors (5)

1. [Wheatstone bridge](wheatstone-bridge.md)
2. [Resistance bridge](resistance-bridge.md)
3. [Electrical measurement](electrical-measurement.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)
