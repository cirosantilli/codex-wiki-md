# Battery internal resistance

↑ **Parent:** [Electric battery](electric-battery.md)

A useful short-interval approximation replaces a [battery](electric-battery.md) by an ideal [electromotive force](electromotive-force.md) $\mathcal E$ in series with a positive internal [electrical resistance](electrical-resistance.md) $r$. This is the [Thévenin terminal response](thevenin-terminal-response.md) with [open-circuit voltage](open-circuit-voltage.md) $\mathcal E$ and [Thévenin resistance](thevenin-resistance.md) $r$. The model describes the terminals without asserting that there is a separate physical [resistor](resistor.md) hidden inside the cell. Both $\mathcal E$ and $r$ can change with composition, [temperature](temperature-split.md), [electric current](electric-current.md) and history.[§10.1, Internal Resistance and Terminal Voltage, current/temperature/history dependence and equation 10.1](university-physics-volume-2-by-samuel-j-ling-and-others.md)

For a resistive [electrical load](electrical-load.md) $R>0$, take $I>0$ to mean discharge: [conventional current](conventional-current.md) leaves the positive terminal. [Kirchhoff's voltage law](kirchhoff-cycle-law.md) and [Ohm's law](ohm-s-law.md) give

$$
\mathcal E-Ir-IR=0,\qquad
I=\frac{\mathcal E}{R+r},\qquad
V_L=IR=\mathcal E-Ir.
$$

For the stipulated $\mathcal E=3\,\mathrm V$, $r=1\,\Omega$, $R=4\,\Omega$,

$$
I=0.6\,\mathrm A,\qquad
Ir=0.6\,\mathrm V,\qquad
V_L=2.4\,\mathrm V.
$$

An [open-circuit voltage](open-circuit-voltage.md) of $3\,\mathrm V$ therefore does not promise $3\,\mathrm V$ at this [electrical load](electrical-load.md). Increasing the load [electrical resistance](electrical-resistance.md) reduces [electric current](electric-current.md) and brings $V_L$ closer to $\mathcal E$, as in [Thévenin load response](thevenin-load-response.md).

The signed relation also explains charging within this model. If an external source drives [electric current](electric-current.md) into the positive terminal, $I<0$ and $V_L=\mathcal E+|I|r$. The terminal [electric potential difference](electric-potential-difference.md) then exceeds $\mathcal E$. This algebra is not evidence that every [battery](electric-battery.md) is rechargeable.[§10.1, paragraph accompanying Figure 10.10: reversed current and charging terminal voltage](university-physics-volume-2-by-samuel-j-ling-and-others.md)

## ↑ Ancestors (6)

1. [Electric battery](electric-battery.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Battery load power and efficiency](battery-load-power-and-efficiency.md)
- [Battery voltage measurement experiment](battery-voltage-measurement-experiment.md)
- [Electric battery](electric-battery.md)
