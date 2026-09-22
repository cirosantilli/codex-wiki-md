# Patch-clamp series resistance

↑ **Parent:** [Whole-cell recording](whole-cell-recording.md)

[Patch-clamp series resistance](patch-clamp-series-resistance.md), also called [patch-clamp access resistance](patch-clamp-series-resistance.md), is the effective [electrical resistance](electrical-resistance.md) between the pipette's sensed voltage and the cell interior. It includes tip access and any remaining obstruction after break-in. For injected [electric current](electric-current.md) $I$ into the [biological cell](biological-cell-split.md), an ideal resistive access path gives

$$
V_p-V=IR_s.
$$

Thus $1\,\mathrm{nA}$ through $20\,\mathrm{M\Omega}$ produces a $20\,\mathrm{mV}$ difference: a substantial possible [voltage clamp](voltage-clamp.md) error. The [electric current](electric-current.md) in this equation is the access-path current, excluding any bypass [seal leak current](seal-leak-current.md). In [current clamp](current-clamp.md), the same access drop contaminates the pipette voltage during injection. Bridge compensation subtracts an estimated $IR_s$; an estimate that changes during recording leaves an error.

An independent passive [voltage clamp](voltage-clamp.md) calculation makes both speed and error visible. Write $v=V-E_L$ and $v_p=V_p-E_L$, with fixed leak [reversal potential](reversal-potential.md) $E_L$, constant membrane [electrical resistance](electrical-resistance.md) $R_m$ and [membrane capacitance](membrane-capacitance.md) $C_m$. Assume an ideal command at the pipette node and omit [seal leak current](seal-leak-current.md) and pipette [capacitance](capacitance.md). [Electric charge conservation](charge-conservation.md) gives

$$
C_m\frac{dv}{dt}=\frac{v_p-v}{R_s}-\frac{v}{R_m}.
$$

For a step $v_p=\Delta V$ from $v(0)=0$, the [ordinary differential equation](ordinary-differential-equation.md) gives

$$
v(t)=\Delta V\frac{R_m}{R_s+R_m}\left(1-e^{-t/\tau_{\mathrm{vc}}}\right),\qquad \tau_{\mathrm{vc}}=C_m\frac{R_sR_m}{R_s+R_m}.
$$

With the figure's parameters and $\Delta V=10\,\mathrm{mV}$, the [time constant](time-constant.md) is $0.909\,\mathrm{ms}$, the final membrane rise is $9.091\,\mathrm{mV}$, and access-path [electric current](electric-current.md) falls from $500$ to $45.45\,\mathrm{pA}$. Only when $R_m\gg R_s$ does the [time constant](time-constant.md) approach $R_sC_m$ and the final voltage approach the command. Actual [voltage clamp](voltage-clamp.md) also depends on amplifier [feedback control](closed-loop-control.md) and the [space clamp](space-clamp.md) problem.

## ↑ Ancestors (5)

1. [Whole-cell recording](whole-cell-recording.md)
2. [Patch clamp](patch-clamp.md)
3. [Neuroscience](neuroscience-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Current clamp](current-clamp.md)
- [Cytosol dialysis](cytosol-dialysis.md)
- [Membrane capacitance](membrane-capacitance.md)
- [Passive membrane response in current clamp](passive-membrane-response-in-current-clamp.md)
- [Patch-clamp series resistance](patch-clamp-series-resistance.md)
- [Patch pipette](patch-pipette.md)
- [Perforated patch recording](perforated-patch-recording.md)
- [Space clamp](space-clamp.md)
- [Whole-cell recording](whole-cell-recording.md)
