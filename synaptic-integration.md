# Synaptic integration

↑ **Parent:** [Neuron](neuron.md)

[Synaptic integration](synaptic-integration.md) is the conversion of inputs at a [neuron](neuron.md)'s [synapses](synapse.md) into a changing [membrane potential](membrane-potential-split.md) and, in a spiking [neuron](neuron.md), the timing or absence of [action potentials](action-potential.md). [Spatial summation](spatial-summation.md) concerns inputs at different locations; [temporal summation](temporal-summation.md) concerns inputs at different times. A useful question is whether individually ineffective inputs can act together, and whether an [inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md) changes that cooperation. The answer depends on location, timing and the receiving [neuron](neuron.md)'s state.

A [synaptic potential](synaptic-potential.md) is a voltage response, whereas [synaptic conductance](synaptic-conductance.md) describes activated [ion channels](ion-channel.md). With inward-positive [electric current](electric-current.md), the contribution of input $j$ is

$$
I_j(t)=g_j(t)(E_j-V).
$$

Here $g_j$ is its [synaptic conductance](synaptic-conductance.md), $E_j$ its [reversal potential](reversal-potential.md) and $V$ the local [membrane potential](membrane-potential-split.md). The driving force $E_j-V$ is an [electric potential difference](electric-potential-difference.md). An [EPSP](excitatory-postsynaptic-potential.md) generally brings the [membrane potential](membrane-potential-split.md) toward a more positive [reversal potential](reversal-potential.md), but its driving force shrinks during [depolarization](depolarization.md). An [IPSP](inhibitory-postsynaptic-potential.md) need not produce [hyperpolarization](hyperpolarization.md): a [reversal potential](reversal-potential.md) above rest but below the [neuronal firing threshold](neuronal-firing-threshold.md) can produce [depolarization](depolarization.md) while opposing a larger excursion. At $E_j=V$, the added [synaptic conductance](synaptic-conductance.md) initially carries zero [electric current](electric-current.md) yet can cause [shunting inhibition](shunting-inhibition.md) of another input.[§3.1, equation (3.1), and §3.1.1: conductance, reversal and voltage-dependent sign; our current convention is inward-positive](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/3-1-synapses.md)

Two distinct nonlinearities matter. Even a passive [cell membrane](cell-membrane-split.md) can show sublinear [synaptic integration](synaptic-integration.md) when added [synaptic conductances](synaptic-conductance.md) reduce driving force and effective [electrical resistance](electrical-resistance.md). Active [voltage-gated ion channels](voltage-gated-ion-channel.md) and [NMDA receptors](nmda-receptor.md) can instead amplify sufficiently concentrated inputs and produce a [dendritic spike](dendritic-spike.md). Neither summing prescribed [electric currents](electric-current.md) nor adding separate measured [EPSPs](excitatory-postsynaptic-potential.md) is an exact universal rule for a branching [neuron](neuron.md).[§1.4.2 and §1.4.4: shunting, saturation and active dendritic interactions](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/1-4-limitations-of-the-leaky-integrate-and-fire-model.md)

**Table of contents**

- [Spatial summation](spatial-summation.md)
  - [Passive dendritic cable](passive-dendritic-cable.md)
  - [Passive spatial and conductance integration](passive-spatial-and-conductance-integration.md)
- [Temporal summation](temporal-summation.md)
  - [Membrane time constant](membrane-time-constant.md)
- [Neuronal firing threshold](neuronal-firing-threshold.md)
- [Dendritic spike](dendritic-spike.md)
- [NMDA receptor](nmda-receptor.md)

## ↑ Ancestors (4)

1. [Neuron](neuron.md)
2. [Neuroscience](neuroscience-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Homeostasis](homeostasis.md)
- [Neuron](neuron.md)
- [Synaptic integration](synaptic-integration.md)
