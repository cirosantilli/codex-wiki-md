# Refractory limits on neuronal firing

↑ **Parent:** [Neuronal refractory period](neuronal-refractory-period.md)

If every [interspike interval](interspike-interval.md) is at least $t_{\mathrm{abs}}>0$, a sustained [spike train](spike-train.md) has mean firing rate at most $1/t_{\mathrm{abs}}$. Across a window of duration $T$, the event count satisfies $N(T)\leq1+T/t_{\mathrm{abs}}$; dividing by $T$ and taking the long-time limit gives the bound. The extra one accounts for a possible first event. The bound permits much slower firing and says nothing about whether stronger drive can maintain the limiting rate in a real [neuron](neuron.md).

For the chosen [phenomenological paired-pulse recovery](phenomenological-paired-pulse-recovery.md), the hold alone gives $500\,\mathrm{Hz}$. Add the further assumption that every successful event resets precisely the same recovery curve, with no accumulation from earlier events. Then $0.35\,\mathrm{nA}$ onset-timed pulses can sustain at most $1000/4.942488\approx202.327\,\mathrm{Hz}$ in that model. This repeatable reset is an extra assumption: a two-pulse result alone cannot establish it. A real [neuron](neuron.md)'s sustained rate also depends on [neural adaptation](neural-adaptation.md), input delivery and evolving [ion-channel inactivation](ion-channel-inactivation.md). The existing [leaky integrate-and-fire model](leaky-integrate-and-fire-model.md) similarly adds integration time to its imposed hold.

A homogeneous [Poisson process](poisson-process-split.md) of rate $\lambda$ has [interspike intervals](interspike-interval.md) with an [exponential distribution](exponential-distribution.md), so

$$
\Pr(S<t_{\mathrm{abs}})=1-e^{-\lambda t_{\mathrm{abs}}}>0.
$$

With the purely illustrative choices $\lambda=100\,\mathrm{Hz}$ and $t_{\mathrm{abs}}=0.002\,\mathrm{s}$, this is $1-e^{-0.2}\approx0.181269$. Thus about $18.13\%$ of intervals predicted by that model violate this chosen hold. Matching a mean [spike train](spike-train.md) count does not make a stimulus-only [Poisson process](poisson-process-split.md) respect recent firing.

A minimal alternative is a [renewal process](renewal-process.md) with [independent and identically distributed](independent-and-identically-distributed-random-variables.md) intervals $S=t_{\mathrm{abs}}+X$, where $X$ has an [exponential distribution](exponential-distribution.md) of rate $\lambda$. Its [hazard function](hazard-function.md) is zero during the hold and $\lambda$ afterwards. Its mean interval is $t_{\mathrm{abs}}+1/\lambda$ and long-run firing rate is

$$
f=\frac{\lambda}{1+\lambda t_{\mathrm{abs}}}.
$$

The same $100\,\mathrm{s}^{-1}$ rate after a $2\,\mathrm{ms}$ hold gives $83.333\,\mathrm{Hz}$, not $100\,\mathrm{Hz}$. This separate stochastic example has no gradual relative recovery; it illustrates why an available-state rate differs from an observed mean firing rate. Smooth dependence on time since the last event can extend the [hazard function](hazard-function.md), while longer histories require more than this simple [renewal process](renewal-process.md). [Time-rescaled spike-train diagnostics](time-rescaled-spike-train-diagnostics.md) can test the resulting history-dependent predictions against recorded [spike trains](spike-train.md).

## ↑ Ancestors (6)

1. [Neuronal refractory period](neuronal-refractory-period.md)
2. [Action potential](action-potential.md)
3. [Neuron](neuron.md)
4. [Neuroscience](neuroscience-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Neuronal refractory period](neuronal-refractory-period.md)
