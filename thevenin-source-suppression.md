<h1 id="thevenin-source-suppression">Thévenin source suppression</h1>

↑ **Parent:** [Thévenin's theorem](thevenin-s-theorem.md)

To determine the [Thévenin resistance](thevenin-resistance.md), remove the external [electrical load](electrical-load.md) and set each [independent electrical source](independent-electrical-source.md) to zero in the circuit model. A zero ideal [voltage source](voltage-source.md) enforces zero [electric potential difference](electric-potential-difference.md), so replace it by a short connection. A zero ideal [current source](current-source.md) enforces zero [electric current](electric-current.md), so replace it by an open connection. Retain every [resistor](resistor.md), including any explicitly modeled supply [electrical resistance](electrical-resistance.md). Turning an actual power supply's front-panel control to zero is not evidence that it physically becomes an ideal wire.

Retain every [dependent electrical source](dependent-electrical-source.md) and its controlling variable: its response to an [electrical test source](electrical-test-source.md) is part of the network's [electrical resistance](electrical-resistance.md). Impose terminal voltage $v_t$ with an [electrical test source](electrical-test-source.md) and calculate $j_t$ _entering_ the suppressed network at $a$. For a nonzero test yielding a finite ratio,

$$
R_{\mathrm{th}}=\frac{v_t}{j_t}.
$$

Alternatively inject a known entering [electric current](electric-current.md) and solve for $v_t$. The test [electric current](electric-current.md) is opposite to the delivered-current convention of the original [Thévenin terminal response](thevenin-terminal-response.md). [Thevenin and Norton Equivalents, pp. 5–7, “Test Source Method for RTH” and Notes: suppress independent sources, retain dependent sources](thevenin-and-norton-equivalents-university-of-houston-teaching-notes.md)

For an original illustration, put a positive [resistor](resistor.md) $R$ across $a,b$ and a [dependent electrical source](dependent-electrical-source.md) in parallel that injects [electric current](electric-current.md) $gv_t$ from $b$ toward $a$, where $g$ has units of [electrical conductance](electrical-conductance.md). Its control is the same terminal voltage $v_t$. [Kirchhoff's current law](kirchhoff-node-law.md) gives

$$
j_t=\frac{v_t}{R}-gv_t,\qquad
R_{\mathrm{th}}=\frac{1}{R^{-1}-g}.
$$

With $R=1\,\mathrm{k\Omega}$ and $g=0.5\,\mathrm{mS}$, a $1\,\mathrm V$ test draws $0.5\,\mathrm{mA}$, giving $R_{\mathrm{th}}=2\,\mathrm{k\Omega}$. Removing the [dependent electrical source](dependent-electrical-source.md) would falsely give $1\,\mathrm{k\Omega}$. With $g=2\,\mathrm{mS}$, the model instead has $R_{\mathrm{th}}=-1\,\mathrm{k\Omega}$; with $g=1\,\mathrm{mS}$ it draws zero test [electric current](electric-current.md) for any imposed voltage and has no finite ratio. An active physical realization requires a supply and has a limited operating range.

For a finite nonzero $R_{\mathrm{th}}$ and a well-defined short-circuit response, $I_{\mathrm{sc}}=V_{\mathrm{oc}}/R_{\mathrm{th}}$. Thus $R_{\mathrm{th}}=V_{\mathrm{oc}}/I_{\mathrm{sc}}$ is usable when $I_{\mathrm{sc}}\ne0$. A source-free positive [resistor](resistor.md) has both $V_{\mathrm{oc}}=0$ and $I_{\mathrm{sc}}=0$, so this quotient cannot reveal its [electrical resistance](electrical-resistance.md); an [electrical test source](electrical-test-source.md) can.

## ↑ Ancestors (3)

1. [Thévenin's theorem](thevenin-s-theorem.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Dependent electrical source](dependent-electrical-source.md)
- [Output impedance](output-impedance.md)
- [Thévenin divider example](thevenin-divider-example.md)
- [Thévenin resistance](thevenin-resistance.md)
