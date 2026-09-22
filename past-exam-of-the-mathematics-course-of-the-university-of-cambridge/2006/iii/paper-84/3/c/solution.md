<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [leaky integrate-and-fire model](../../../../../../leaky-integrate-and-fire-model.md) treats the membrane as a [capacitance](../../../../../../capacitance.md) $C_m$. The leak conductance $g_L$ drives voltage towards its resting reversal $V_L$; the excitatory conductance $g_E$ drives it towards its reversal $V_E$; and $I_e$ is injected current, positive inward. A sufficiently high $V_E$ makes increasing $g_E$ depolarizing over the relevant voltage range, while also increasing total conductance and shortening the integration time.

For constant input and conductances, put

$$
\tau_{\rm eff}=\frac{C_m}{g_L+g_E},\qquad V_\infty=\frac{g_LV_L+g_EV_E+I_e}{g_L+g_E}.
$$

Then

$$
\boxed{V(t)=V_\infty+[V(0)-V_\infty]e^{-t/\tau_{\rm eff}}}.
$$

If this trajectory reaches $V_\theta$, register a spike and reset the voltage to $V_0<V_\theta$, optionally enforcing a specified [neuronal refractory period](../../../../../../neuronal-refractory-period.md). The reset makes repeated threshold crossings possible under a constant suprathreshold drive. If $V_\infty\leq V_\theta$ and the initial voltage is below threshold, no finite-time crossing occurs; equality gives asymptotic approach. For time-varying currents or conductances, integrate the subthreshold differential equation until the next crossing.

Use this model when spike timing, spike counts and network integration matter more than the detailed waveform: it is inexpensive for large recurrent networks or comparisons of current-driven and conductance-driven input. It omits ionic spike initiation, channel-specific adaptation and many dendritic effects, for which a [Hodgkin-Huxley model](../../../../../../hodgkin-huxley-model.md) or a spatial model may be needed.

## ↑ Ancestors (11)

1. [C](../c.md)
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
