<h1 id="thevenin-load-response">Thévenin load response</h1>

↑ **Parent:** [Thévenin's theorem](thevenin-s-theorem.md)

A positive resistive [electrical load](electrical-load.md) obeys [Ohm's law](ohm-s-law.md), $V_L=IR_L$. Its [resistive load line](resistive-load-line.md) intersects the [Thévenin terminal response](thevenin-terminal-response.md) at

$$
I=\frac{V_{\mathrm{oc}}}{R_{\mathrm{th}}+R_L},\qquad
V_L=\frac{V_{\mathrm{oc}}R_L}{R_{\mathrm{th}}+R_L},
$$

provided $R_{\mathrm{th}}+R_L\ne0$. For the [Thévenin divider example](thevenin-divider-example.md), $R_L=1\,\mathrm{k\Omega}$ gives $I=24/7\,\mathrm{mA}$ and $V_L=24/7\,\mathrm V$; $R_L=4\,\mathrm{k\Omega}$ gives $I=1.5\,\mathrm{mA}$ and $V_L=6\,\mathrm V$. At $R_L=R_{\mathrm{th}}=\tfrac43\,\mathrm{k\Omega}$, the voltage is $4\,\mathrm V$, half the [open-circuit voltage](open-circuit-voltage.md).

<a id="thevenin-terminal-load-lines-and-voltage"></a>
![](thevenin-terminal-load-lines-and-voltage.png)

**[Figure 15](#thevenin-terminal-load-lines-and-voltage). Load-line intersections and load voltage for the 12 V divider**. [Source](thevenin-terminal-load-lines-and-voltage.py). Left: the [Thévenin terminal response](thevenin-terminal-response.md) falls from $8\,\mathrm V$ at zero delivered [electric current](electric-current.md) to zero voltage at $6\,\mathrm{mA}$; three positive [resistive load lines](resistive-load-line.md) select operating points. Right: both the original loaded [voltage divider](voltage-divider.md) calculation and its equivalent give the same voltage curve, approaching $8\,\mathrm V$ as $R_L$ increases. Calculated values only.

For this positive $R_{\mathrm{th}}$, increasing $R_L$ reduces the drawn [electric current](electric-current.md) and raises $V_L$ toward $V_{\mathrm{oc}}$. This explains [voltmeter loading](voltmeter-loading.md): a [voltmeter](voltmeter.md) itself is an [electrical load](electrical-load.md). The equivalence also applies to a nonlinear [electrical load](electrical-load.md) through intersection with its terminal relation, but an arbitrary load need not give a unique operating point. If negative $R_{\mathrm{th}}$ cancels positive $R_L$, the displayed formula is singular; a real active circuit's limits and dynamics must then be considered.

## ↑ Ancestors (3)

1. [Thévenin's theorem](thevenin-s-theorem.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Battery internal resistance](battery-internal-resistance.md)
