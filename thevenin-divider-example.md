<h1 id="thevenin-divider-example">Thévenin divider example</h1>

↑ **Parent:** [Thévenin's theorem](thevenin-s-theorem.md)

In the pictured original [linear resistive circuit](linear-resistive-circuit.md), the ideal [voltage source](voltage-source.md) keeps its upper node at $12\,\mathrm V$ relative to $b$. Let $R_1=2\,\mathrm{k\Omega}$ connect that node to $a$, and $R_2=4\,\mathrm{k\Omega}$ connect $a$ to $b$. With the external [electrical load](electrical-load.md) removed, the [voltage divider](voltage-divider.md) gives

$$
V_{\mathrm{oc}}=12\,\mathrm V\,\frac{4\,\mathrm{k\Omega}}{2\,\mathrm{k\Omega}+4\,\mathrm{k\Omega}}=8\,\mathrm V.
$$

To find the [Thévenin resistance](thevenin-resistance.md), [Thévenin source suppression](thevenin-source-suppression.md) replaces the ideal $12\,\mathrm V$ [voltage source](voltage-source.md) by a wire. Both [resistors](resistor.md) now join $a$ to $b$ in parallel, giving

$$
R_{\mathrm{th}}=\frac{R_1R_2}{R_1+R_2}=\frac43\,\mathrm{k\Omega}.
$$

This is the [electrical resistance](electrical-resistance.md) looking into the original network with its [independent electrical source](independent-electrical-source.md) suppressed; the external [electrical load](electrical-load.md) is excluded.

An independent check uses [Kirchhoff's current law](kirchhoff-node-law.md) at $a$, without suppressing anything:

$$
\frac{12\,\mathrm V-V}{2\,\mathrm{k\Omega}}=\frac{V}{4\,\mathrm{k\Omega}}+I,
\qquad V=8\,\mathrm V-\left(\frac43\,\mathrm{k\Omega}\right)I.
$$

The [Thévenin terminal response](thevenin-terminal-response.md) thus follows directly from the original topology. Shorting $a$ to $b$ in this ideal calculation gives $I_{\mathrm{sc}}=6\,\mathrm{mA}$: the lower [resistor](resistor.md) has zero voltage and the upper [resistor](resistor.md) limits the [electric current](electric-current.md). All numerical values here and in the figures are stipulated model values, not laboratory data.

## ↑ Ancestors (3)

1. [Thévenin's theorem](thevenin-s-theorem.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thévenin load response](thevenin-load-response.md)
