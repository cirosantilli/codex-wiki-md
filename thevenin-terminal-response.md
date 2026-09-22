<h1 id="thevenin-terminal-response">Thévenin terminal response</h1>

↑ **Parent:** [Thévenin's theorem](thevenin-s-theorem.md)

With the [passive sign convention](passive-sign-convention.md) applied to the network, its entering [electric current](electric-current.md) is $J=-I$, and the same relation becomes $V=V_{\mathrm{oc}}+JR_{\mathrm{th}}$. The [electrical load](electrical-load.md) uses the [passive sign convention](passive-sign-convention.md) with entering [electric current](electric-current.md) $I$, so it absorbs [power](power.md) $VI$. A positive delivered [electric current](electric-current.md) therefore produces a voltage drop for positive $R_{\mathrm{th}}$; changing the reference direction without changing the equation would give the wrong sign.

The reason is [linearity](linearity.md) of [Ohm's law](ohm-s-law.md), [Kirchhoff's current law](kirchhoff-node-law.md), [Kirchhoff's voltage law](kirchhoff-cycle-law.md), and the constitutive relations of any linear [dependent electrical sources](dependent-electrical-source.md). Solve once at $I=0$ with the [independent electrical sources](independent-electrical-source.md) present. Subtract this solution from a solution with prescribed delivered [electric current](electric-current.md) $I$: the fixed [independent electrical sources](independent-electrical-source.md) cancel, leaving a homogeneous [linear](linearity.md) network whose terminal voltage change is proportional to $I$. This is a short [superposition principle](superposition-principle.md) argument for an [affine function](affine-function.md); the fixed offset need not vanish.

The qualification about a well-defined response matters. An ideal [voltage source](voltage-source.md) alone has $R_{\mathrm{th}}=0$. An ideal nonzero [current source](current-source.md) alone constrains $I$ and does not have a finite open-circuit voltage or a representation $V=V_{\mathrm{oc}}-IR_{\mathrm{th}}$ with finite coefficients. Linear [dependent electrical sources](dependent-electrical-source.md) can give [negative resistance](negative-resistance.md), and singular ideal networks may fail to have a unique finite response. Neither a finite nor a strictly positive passive $R_{\mathrm{th}}$ follows merely from calling an [electrical circuit](electrical-circuit-split.md) linear. [Thevenin and Norton Equivalents, p. 11, “On a Negative Thevenin Equivalent Resistance”: dependent-source models can have negative equivalent resistance](thevenin-and-norton-equivalents-university-of-houston-teaching-notes.md)

## ↑ Ancestors (3)

1. [Thévenin's theorem](thevenin-s-theorem.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Battery internal resistance](battery-internal-resistance.md)
- [Electrical load](electrical-load.md)
- [Resistive load line](resistive-load-line.md)
- [Thévenin divider example](thevenin-divider-example.md)
- [Thévenin load response](thevenin-load-response.md)
- [Thévenin measurement experiment](thevenin-measurement-experiment.md)
- [Thévenin resistance](thevenin-resistance.md)
- [Thévenin source suppression](thevenin-source-suppression.md)
