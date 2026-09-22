# Independent permissive gates in an ion channel

↑ **Parent:** [Two-state ion-channel gating](two-state-ion-channel-gating.md)

A permissive gate allows conduction when it is open. Suppose an [ion channel](ion-channel.md) conducts only when all $q$ gates are open, where $q$ is a positive [integer](integer-split.md). If the gate-open [events](event.md) are mutually [independent events](independent-events.md) and each has the same open [probability](probability.md) $p$ at the time considered, then

$$
P_{\mathrm{open}}=\prod_{j=1}^q p=p^q.
$$

This follows from the multiplication rule for [independent events](independent-events.md). Identical transition rates alone do not guarantee independence: the initial gate states must also be independently prepared, and the model must not couple their transitions. Gates sharing a fluctuating [membrane potential](membrane-potential-split.md) can be correlated; the simple product requires an appropriate independence assumption, for example independent gates at an externally fixed voltage.

At $p=0.5$, channels requiring $q=1,2,4$ permissive gates have open [probabilities](probability.md) $0.5$, $0.25$ and $0.0625$. For four independent gates there are $2^4=16$ possible open/closed configurations, equally probable at $p=0.5$; only the all-open configuration conducts. Thus $0.5$ is the gate-open [probability](probability.md), while $0.0625$ is the whole-channel open [probability](probability.md). Neither is a fractional state of one observed channel. Among $160$ independently prepared identical four-gate channels, the [expected value](expected-value-split.md) of the open count is $160/16=10$, although an actual count fluctuates.

<a id="image-independent-permissive-gates-in-an-ion-channel-an-all-open-requirement"></a>
![](independent-ion-channel-gates.png)

**[Figure 5](#image-independent-permissive-gates-in-an-ion-channel-an-all-open-requirement). Independent permissive gates in an ion channel: an all-open requirement**. Left: whole-channel open [probability](probability.md) $p^q$ for one, two and four identical independent permissive gates. Right: all sixteen configurations of four gates at $p=0.5$, each with [probability](probability.md) $1/16$; filled circles are open gates and empty circles closed gates. Only the highlighted all-open configuration permits conduction. This is an illustrative model, not a molecular structure or an ionic [electric current](electric-current.md) measurement.

For unequal independent gate-open [probabilities](probability.md) $p_j$, use $P_{\mathrm{open}}=\prod_j p_j$ rather than $p^q$. This is the distinction behind the [Hodgkin-Huxley model](hodgkin-huxley-model.md)'s $m^3h$: $m$ and $h$ are different activation and inactivation-availability variables, rather than one common $p$. Its $n^4$ uses four identical activation factors. Independence and the all-open requirement are model assumptions; correlated gates or alternative conducting configurations require a different calculation. The simple product is useful because a modest gate-open [probability](probability.md) can produce sharply suppressed whole-channel availability without any additional gate interaction.

## ↑ Ancestors (6)

1. [Two-state ion-channel gating](two-state-ion-channel-gating.md)
2. [Voltage-gated ion channel](voltage-gated-ion-channel.md)
3. [Membrane potential](membrane-potential-split.md)
4. [Biological cell](biological-cell-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Hodgkin-Huxley model](hodgkin-huxley-model.md)
- [Independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md)
- [Two-state ion-channel gating](two-state-ion-channel-gating.md)
