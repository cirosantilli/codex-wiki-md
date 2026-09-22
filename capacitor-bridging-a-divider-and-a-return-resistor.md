# Capacitor bridging a divider and a return resistor

↑ **Parent:** [Capacitor](capacitor.md)

Feed a node through resistance $R$ from an ideal voltage $V$, connect that node to ground through $2R$, and connect a capacitor from it to a second node grounded through $R$. The capacitor sees a [Thévenin equivalent](thevenin-equivalent.md) with open-circuit voltage $2V/3$ and resistance $(R\parallel2R)+R=5R/3$. For zero initial capacitor voltage, $I_C=2V e^{-t/\tau}/(5R)$ and $\tau=5RC/3$. The $2R$ branch current is $V/(3R)-I_C/3$, so the two branch currents coincide at $t=\tau\log(8/5)$. This illustrates why the source-side resistor alone does not determine a charging time constant.

## ↑ Ancestors (5)

1. [Capacitor](capacitor.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
