# Eligibility trace

↑ **Parent:** [Synaptic plasticity](synaptic-plasticity.md)

A decaying record of recent activity that marks a state or connection as eligible for modification by a later teaching signal. An accumulating value-learning trace is $e_t=\gamma\lambda e_{t-1}+x(s_t)$, giving $\Delta w=\alpha\delta_t e_t$. Other traces record action-policy [gradients](gradient.md) or pre/post synaptic events. The update and episode-boundary convention must be specified; an [eligibility trace](eligibility-trace.md) is not automatically identical to the visual activity trace used for [trace learning](trace-learning.md).

## ↑ Ancestors (6)

1. [Synaptic plasticity](synaptic-plasticity.md)
2. [Synapse](synapse.md)
3. [Neuron](neuron-split.md)
4. [Neuroscience](neuroscience-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Eligibility trace](eligibility-trace.md)
- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/5/solution.md)
- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/6/solution.md)
- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022/4/solution.md)
