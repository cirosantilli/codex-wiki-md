<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [dynamic clamp](../../../../../../dynamic-clamp.md) is a real-time feedback experiment. Measure the [membrane potential](../../../../../../membrane-potential.md) through an electrode, numerically evolve chosen channel or synapse state variables, calculate the modeled current, and inject that current into the real neuron. A virtual synapse might use $I_{\rm syn}=g_{\rm syn}(t)(E_{\rm syn}-V(t))$; a voltage-dependent virtual channel also updates its gate probabilities from the measured voltage. Repeat at a rate fast relative to the dynamics being modeled. Unlike voltage clamp, this procedure does not hold the voltage at a command value.

Two uses are to add a controlled inhibitory conductance and measure its effect on firing or integration, and to couple two real neurons by artificial reciprocal inhibitory [synapses](../../../../../../synapse.md) to test the resulting network dynamics. Both artificial conductances and reciprocal inhibitory connections were demonstrated in the primary [Sharp–O'Neil–Abbott–Marder dynamic-clamp experiments](https://scholarworks.brandeis.edu/esploro/outputs/journalArticle/Dynamic-clamp-computer-generated-conductances-in-real/9923970781201921). Conductance magnitude, time course and reversal voltage can be varied without requiring the cell to express a new channel. Sampling delay, electrode error and the inability of a single injection site to reproduce all dendritic conductance locations are practical limitations.

## ↑ Ancestors (11)

1. [B](../b.md)
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
