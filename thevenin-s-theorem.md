<h1 id="thevenin-s-theorem">Thévenin's theorem</h1>

↑ **Parent:** [Electrical engineering](electrical-engineering-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thévenin's_theorem)

Thévenin's theorem replaces the terminal behavior of a [linear resistive circuit](linear-resistive-circuit.md) by an ideal [voltage source](voltage-source.md) in series with a [Thévenin resistance](thevenin-resistance.md), whenever its terminal [electric potential difference](electric-potential-difference.md) is a well-defined [affine function](affine-function.md) of the delivered [electric current](electric-current.md). Fix terminals $a,b$, write $V=\phi(a)-\phi(b)$, and take $I$ positive _out of the network at $a$_ into the [electrical load](electrical-load.md), returning through $b$. Then

$$
V=V_{\mathrm{oc}}-IR_{\mathrm{th}}.
$$

The [open-circuit voltage](open-circuit-voltage.md) $V_{\mathrm{oc}}$ is the intercept at $I=0$; $-R_{\mathrm{th}}$ is the slope. Thus two parameters predict what happens when many different [electrical loads](electrical-load.md) are connected. The [Wheatstone bridge detector loading](wheatstone-bridge-detector-loading.md) calculation uses precisely this replacement to find the detector reading even when the bridge's two [voltage dividers](voltage-divider.md) interact through its detector.

For example, a $12\,\mathrm V$ ideal [voltage source](voltage-source.md) with $2\,\mathrm{k\Omega}$ above and $4\,\mathrm{k\Omega}$ below a [voltage divider](voltage-divider.md) junction supplies $V_{\mathrm{oc}}=8\,\mathrm V$ and $R_{\mathrm{th}}=\tfrac43\,\mathrm{k\Omega}$ at that junction relative to the lower terminal. Attaching a $4\,\mathrm{k\Omega}$ [electrical load](electrical-load.md) reduces its voltage to $6\,\mathrm V$ and draws $1.5\,\mathrm{mA}$. The equivalent explains why an unloaded divider ratio alone cannot predict a loaded output.

<a id="thevenin-divider-and-equivalent-circuits"></a>
![](thevenin-divider-and-equivalent-circuits.png)

**[Figure 14](#thevenin-divider-and-equivalent-circuits). A 12 V voltage divider and its 8 V Thévenin equivalent feed the same load**. [Source](thevenin-divider-and-equivalent-circuits.py). Original calculated example: the left circuit has $2\,\mathrm{k\Omega}$ and $4\,\mathrm{k\Omega}$ divider arms; the right circuit has an $8\,\mathrm V$ ideal [voltage source](voltage-source.md) and $\tfrac43\,\mathrm{k\Omega}$ series [Thévenin resistance](thevenin-resistance.md). Both use $V=\phi(a)-\phi(b)$ and delivered [electric current](electric-current.md) $I$ from $a$ into the same [electrical load](electrical-load.md). Dashed boundaries identify what is replaced.

The equivalence concerns the chosen terminals, including the [power](power.md) $VI$ delivered there. It does not identify internal branch [electric currents](electric-current.md) or internal [Joule heating](joule-heating.md). At open circuit the original divider still draws $2\,\mathrm{mA}$ from its $12\,\mathrm V$ supply, while the equivalent's series branch carries no [electric current](electric-current.md). [Thevenin and Norton Equivalents, pp. 1–2, “The Idea” and “Important Notes”: equivalence at the specified terminals](thevenin-and-norton-equivalents-university-of-houston-teaching-notes.md)

**Table of contents**

- [Thévenin terminal response](thevenin-terminal-response.md)
- [Thévenin divider example](thevenin-divider-example.md)
- [Thévenin source suppression](thevenin-source-suppression.md)
- [Thévenin load response](thevenin-load-response.md)
- [Thévenin measurement experiment](thevenin-measurement-experiment.md)
- [Thévenin resistance](thevenin-resistance.md)
- [Thévenin equivalent](thevenin-equivalent.md)

## ↑ Ancestors (2)

1. [Electrical engineering](electrical-engineering-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Galvanometer null detection](galvanometer-null-detection.md)
- [RC low-pass output loading](rc-low-pass-output-loading.md)
- [Thévenin equivalent](thevenin-equivalent.md)
- [Voltage divider](voltage-divider.md)
- [Wheatstone bridge](wheatstone-bridge.md)
- [Wheatstone bridge detector loading](wheatstone-bridge-detector-loading.md)
