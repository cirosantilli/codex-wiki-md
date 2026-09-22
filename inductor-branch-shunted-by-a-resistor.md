# Inductor branch shunted by a resistor

↑ **Parent:** [RL circuit](rl-circuit.md)

An ideal source $V$ feeds a series resistance $2R$, followed by parallel branches $R+L$ and $2R$. The [Thévenin equivalent](thevenin-equivalent.md) seen by the [inductor](inductor.md) has voltage $V/2$ and resistance $R+(2R\parallel2R)=2R$. From zero initial current, the inductor current is $V(1-e^{-t/\tau})/(4R)$, the other branch current is $V(1+e^{-t/\tau})/(8R)$, and the source current is $V(3-e^{-t/\tau})/(8R)$. [Kirchhoff's current law](kirchhoff-node-law.md) holds at every time, and the final stored [magnetic energy](magnetic-energy.md) is $LV^2/(32R^2)$.

## ↑ Ancestors (6)

1. [RL circuit](rl-circuit.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
