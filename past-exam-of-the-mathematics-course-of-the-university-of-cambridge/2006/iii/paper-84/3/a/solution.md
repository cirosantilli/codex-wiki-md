<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At rest, the cell has relatively high intracellular potassium and high extracellular sodium. The [membrane potential](../../../../../../membrane-potential.md) is negative inside, largely because selective resting permeability, particularly potassium leak, combines with these electrochemical gradients. The sodium-potassium pump maintains the gradients over time; it is not the immediate regenerative current of an [action potential](../../../../../../action-potential.md).

Depolarization rapidly activates sodium [voltage-gated ion channels](../../../../../../voltage-gated-ion-channel.md), causing inward sodium current and further depolarization. Slower sodium inactivation and delayed potassium activation then reduce inward current and increase outward potassium current, repolarizing the membrane. Persisting potassium conductance can produce an after-hyperpolarization; recovery of sodium availability contributes to the [neuronal refractory period](../../../../../../neuronal-refractory-period.md). A spike transfers only a small fraction of the bulk ions, so it changes charge separation much more than it changes the overall concentration gradients.

For [two-state ion-channel gating](../../../../../../two-state-ion-channel-gating.md), let $X$ be the fraction of permissive gates. Opening transfers probability from $1-X$ at rate $\alpha_X(V)$, and closing transfers it back at rate $\beta_X(V)$:

$$
\boxed{\dot X=\alpha_X(V)(1-X)-\beta_X(V)X=\frac{X_\infty(V)-X}{\tau_X(V)}},\quad X_\infty=\frac{\alpha_X}{\alpha_X+\beta_X},\quad\tau_X=\frac1{\alpha_X+\beta_X}.
$$

Independent subunits that must all be permissive multiply their probabilities. The [Hodgkin-Huxley model](../../../../../../hodgkin-huxley-model.md) therefore uses $g_{\rm Na}=\bar g_{\rm Na}m^3h$ and $g_{\rm K}=\bar g_{\rm K}n^4$: $m$ describes sodium activation, $h$ sodium availability, and $n$ potassium activation. Their voltage-dependent time scales produce the sequence of inward and outward current. This channel-level construction is the mechanism in the primary [Hodgkin–Huxley membrane-current model](https://onlinelibrary.wiley.com/doi/10.1113/jphysiol.1952.sp004764).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
