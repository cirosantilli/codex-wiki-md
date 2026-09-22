# Galvanometer null detection

↑ **Parent:** [Galvanometer](galvanometer.md)

In a [Wheatstone bridge](wheatstone-bridge.md), the [galvanometer](galvanometer.md) connects the two comparison junctions. Its purpose is to locate a [null measurement](null-measurement.md), rather than to measure the branch [electric current](electric-current.md) through the unknown [resistor](resistor.md). Using [Wheatstone bridge detector loading](wheatstone-bridge-detector-loading.md) and [Thévenin's theorem](thevenin-s-theorem.md), a settled [moving-coil galvanometer](moving-coil-galvanometer.md) with winding [electrical resistance](electrical-resistance.md) $R_g$ obeys

$$
I_g=\frac{V_{\mathrm{oc}}}{R_{\mathrm{th}}+R_g},\qquad \theta=S_I\frac{V_{\mathrm{oc}}}{R_{\mathrm{th}}+R_g}.
$$

Here $V_{\mathrm{oc}}$ is the bridge's [open-circuit voltage](open-circuit-voltage.md) and $R_{\mathrm{th}}$ its [Thévenin resistance](thevenin-resistance.md). For a functioning passive detector with finite positive [electrical resistances](electrical-resistance.md), exact $I_g=0$ implies $V_{\mathrm{oc}}=0$, preserving [Wheatstone bridge balance](wheatstone-bridge-balance.md). Away from balance, the detector loads the junctions; its [electrical resistance](electrical-resistance.md) cannot be ignored.

For the illustrative $R_g=100\,\Omega$, $S_I=3000\,\mathrm{rad/A}$ and a chosen $R_{\mathrm{th}}=1900\,\Omega$, a $1.00\,\mathrm{mV}$ bridge [open-circuit voltage](open-circuit-voltage.md) produces $0.500\,\mathrm{\mu A}$ and $0.0859^\circ$. That lies inside the stipulated $0.10^\circ$ zero tolerance. The corresponding resolvable [open-circuit voltage](open-circuit-voltage.md) scale is about $1.16\,\mathrm{mV}$, not arbitrarily small. Actual limits also depend on the zero stability and calibration.

Use the detector checks in the [slide-wire resistance bridge experiment](slide-wire-resistance-bridge-experiment.md): perturb the comparison to either side of the proposed balance and require opposite signs, while confirming the supply is on. A broken connection, a jammed pointer or an inactive supply can also give a zero reading. Conversely, a healthy bridge detector reads zero while the bridge arms still carry [electric current](electric-current.md). A zero deflection alone proves neither a broken conducting path nor infinite sensitivity.

## ↑ Ancestors (7)

1. [Galvanometer](galvanometer.md)
2. [Electric current](electric-current.md)
3. [Electric charge](electric-charge-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
