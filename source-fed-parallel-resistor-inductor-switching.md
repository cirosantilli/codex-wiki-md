# Source-fed parallel resistor-inductor switching

↑ **Parent:** [Inductor](inductor.md)

An ideal [voltage source](voltage-source.md) $V_0$ and series [resistor](resistor.md) $R_1$ feed parallel branches $L$ and $R_2$. [Thévenin's theorem](thevenin-s-theorem.md) gives $R_{\rm th}=R_1R_2/(R_1+R_2)$ and $V_{\rm th}=V_0R_2/(R_1+R_2)$. Starting with zero [inductor](inductor.md) current, $i_L=(V_0/R_1)(1-e^{-t/\tau})$ and $i_2=V_0e^{-t/\tau}/(R_1+R_2)$. Switch-on heat in $R_2$ is $LV_0^2/[2R_1(R_1+R_2)]$. Disconnecting the source leaves the stored [magnetic energy](magnetic-energy.md) $Li_L^2/2$ to dissipate through $R_2$, with [time constant](time-constant.md) $L/R_2$.

## ↑ Ancestors (7)

1. [Inductor](inductor.md)
2. [Self-inductance](self-inductance.md)
3. [Inductance](inductance.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
