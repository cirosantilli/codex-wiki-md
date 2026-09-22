# Phenomenological paired-pulse recovery

↑ **Parent:** [Neuronal paired-pulse recovery](neuronal-paired-pulse-recovery.md)

Choose the following original phenomenological [mathematical model](mathematical-model.md) solely to calculate a paired-pulse readout. It is not experimental data, a fit to the teaching experiment, or a simulation of the [Hodgkin-Huxley model](hodgkin-huxley-model.md). The conditioning [action potential](action-potential.md) defines time zero. Test pulses have fixed width $0.2\,\mathrm{ms}$; $I$ denotes their inward [electric current](electric-current.md) amplitude. Impose an [absolute neuronal refractory period](absolute-neuronal-refractory-period.md) $t_{\mathrm{abs}}=2\,\mathrm{ms}$. No finite test amplitude generates an event for $0<\Delta<t_{\mathrm{abs}}$. After that hold, stipulate a required amplitude

$$
I_{\mathrm{req}}(\Delta)=I_\infty\left(1+A e^{-(\Delta-t_{\mathrm{abs}})/\tau_r}\right),\qquad \Delta\geq t_{\mathrm{abs}},
$$

with $I_\infty=0.2\,\mathrm{nA}$, dimensionless $A=2$ and recovery [time constant](time-constant.md) $\tau_r=3\,\mathrm{ms}$. Emit a test event exactly when $I\geq I_{\mathrm{req}}(\Delta)$, including equality. For this ideal event readout, assign events to pulse onset and assume the conditioning event is successfully evoked. There is no calculated [membrane potential](membrane-potential-split.md), spike waveform, response latency or stochastic success [probability](probability.md).

<a id="image-chosen-refractory-hold-and-required-test-pulse-amplitude"></a>
![](neuronal-refractory-recovery-curves.png)

**[Figure 11](#image-chosen-refractory-hold-and-required-test-pulse-amplitude). Chosen refractory hold and required test-pulse amplitude**. Original [phenomenological paired-pulse recovery](phenomenological-paired-pulse-recovery.md) rule, not measured data or a channel simulation. The grey region forbids a second event; after $2\,\mathrm{ms}$, the required [electric current](electric-current.md) falls from $0.6$ toward $0.2\,\mathrm{nA}$. Horizontal lines show two chosen test amplitudes; their intersections give different first permitted test delays. The dashed baseline is approached asymptotically.

The [exponential decay](exponential-decay.md) represents a combined recovery deficit; it is neither the [Hodgkin-Huxley model](hodgkin-huxley-model.md)'s $h$ nor a measured [potassium](potassium.md) [electrical conductance](electrical-conductance.md). One such curve cannot separately identify [sodium](sodium.md) recovery and persistent [potassium](potassium.md) [electrical conductance](electrical-conductance.md). A constant pulse-width amplitude criterion also does not establish an equivalent rule for other pulse widths or voltage trajectories.

At the hold boundary, $I_{\mathrm{req}}(2\,\mathrm{ms})=0.2(1+2)=0.6\,\mathrm{nA}$. At $\Delta=4\,\mathrm{ms}$,

$$
I_{\mathrm{req}}=0.2(1+2e^{-2/3})\,\mathrm{nA}\approx0.405367\,\mathrm{nA};
$$

at $\Delta=6\,\mathrm{ms}$,

$$
I_{\mathrm{req}}=0.2(1+2e^{-4/3})\,\mathrm{nA}\approx0.305439\,\mathrm{nA}.
$$

Thus a $0.35\,\mathrm{nA}$ test fails at $1\,\mathrm{ms}$ because of the imposed hold, fails at $4\,\mathrm{ms}$ because recovery is insufficient for that amplitude, and succeeds at $6\,\mathrm{ms}$. At $4\,\mathrm{ms}$, a $0.5\,\mathrm{nA}$ pulse would instead succeed: failure of the weaker pulse was relative refractoriness.

<a id="image-paired-pulses-and-event-readout-at-three-chosen-delays"></a>
![](neuronal-paired-pulse-event-readout.png)

**[Figure 12](#image-paired-pulses-and-event-readout-at-three-chosen-delays). Paired pulses and event readout at three chosen delays**. Each row is a separately reset ideal trial with a $0.65\,\mathrm{nA}$ conditioning pulse assumed to evoke an [action potential](action-potential.md) at time zero and a $0.35\,\mathrm{nA}$ test pulse. Rectangles are imposed [electric current](electric-current.md) pulses; vertical ticks are abstract events, not voltage recordings. Only the $6\,\mathrm{ms}$ test passes the stipulated recovery rule. The $1\,\mathrm{ms}$ and $4\,\mathrm{ms}$ failures have different causes.

For $I>I_\infty$, solve $I\geq I_{\mathrm{req}}(\Delta)$ using the [logarithm](logarithm.md). The earliest allowed delay is

$$
\Delta_{\min}(I)=t_{\mathrm{abs}}+\max\left\{0,\tau_r\ln\left(\frac{A}{I/I_\infty-1}\right)\right\}.
$$

For $I=0.35\,\mathrm{nA}$ this is $2+3\ln(8/3)\approx4.942488\,\mathrm{ms}$; for $I=0.5\,\mathrm{nA}$ it is $2+3\ln(4/3)\approx2.863046\,\mathrm{ms}$. If $I\geq0.6\,\mathrm{nA}$, the imposed $2\,\mathrm{ms}$ hold is the only delay restriction. If $I\leq I_\infty$, no finite delay passes the rule: the required amplitude stays strictly above its asymptotic baseline. A finite experimental “fully recovered” time therefore also needs a tolerance and a readout definition.

## ↑ Ancestors (7)

1. [Neuronal paired-pulse recovery](neuronal-paired-pulse-recovery.md)
2. [Neuronal refractory period](neuronal-refractory-period.md)
3. [Action potential](action-potential.md)
4. [Neuron](neuron.md)
5. [Neuroscience](neuroscience-split.md)
6. [Biology](biology-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Absolute neuronal refractory period](absolute-neuronal-refractory-period.md)
- [Neuronal refractory period](neuronal-refractory-period.md)
- [Phenomenological paired-pulse recovery](phenomenological-paired-pulse-recovery.md)
- [Refractory limits on neuronal firing](refractory-limits-on-neuronal-firing.md)
