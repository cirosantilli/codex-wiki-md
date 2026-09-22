# Shunting inhibition

↑ **Parent:** [Chemical synapse](chemical-synapse.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shunting_inhibition)

[Shunting inhibition](shunting-inhibition.md) is suppression of another input's effect through increased [synaptic conductance](synaptic-conductance.md): opening additional [ion channels](ion-channel.md) lowers effective [electrical resistance](electrical-resistance.md), reducing the voltage response to a given added [electric current](electric-current.md). When the added [reversal potential](reversal-potential.md) equals the resting [membrane potential](membrane-potential.md), there can be no voltage change at rest and still be inhibition of a simultaneous input. See [1.4 Limitations of the Leaky Integrate-and-Fire Model](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/1-4-limitations-of-the-leaky-integrate-and-fire-model.md).

Use the passive [synaptic potential](synaptic-potential.md) model below with leak $g_L=10\,\mathrm{nS}$, $E_L=-65\,\mathrm{mV}$ and [capacitance](capacitance.md) $C=200\,\mathrm{pF}$. A sustained inward test [electric current](electric-current.md) of $I_{\mathrm{ext}}=100\,\mathrm{pA}$ alone gives a steady voltage increase of $I_{\mathrm{ext}}/g_L=10\,\mathrm{mV}$, so $V_\infty=-55\,\mathrm{mV}$. Effective [electrical resistance](electrical-resistance.md) is $100\,\mathrm{M\Omega}$ and the [time constant](time-constant.md) is $20\,\mathrm{ms}$.

Now hold a shunting conductance $g_i=20\,\mathrm{nS}$ open with $E_i=E_L=-65\,\mathrm{mV}$. With no test [electric current](electric-current.md), rest stays at $-65\,\mathrm{mV}$. With the same $100\,\mathrm{pA}$ test [electric current](electric-current.md), total conductance becomes $30\,\mathrm{nS}$, so the steady voltage increase is only $100/30\simeq3.333\,\mathrm{mV}$: $V_\infty\simeq-61.667\,\mathrm{mV}$. Effective [electrical resistance](electrical-resistance.md) is $33.333\,\mathrm{M\Omega}$ and the [time constant](time-constant.md) is $200/30\simeq6.667\,\mathrm{ms}$. A faster response can therefore be smaller. At the original rest the shunting [electric current](electric-current.md) is zero; at $V=-55\,\mathrm{mV}$ it is $20(-65+55)=-200\,\mathrm{pA}$, opposing the voltage excursion.

The factor of three reduction applies to this constant-[electric current](electric-current.md), constant-conductance example. A finite pulse, conductance-driven input or spatially extended [dendrite](dendrite.md) need not have the same reduction. The interesting feature is conditional action: the shunt can leave a quiet [neuron](neuron.md)'s voltage unchanged yet reshape its response when another input arrives. A model that represents all inhibition as a fixed outward [electric current](electric-current.md) misses this behavior.

## ↑ Ancestors (6)

1. [Chemical synapse](chemical-synapse.md)
2. [Synapse](synapse.md)
3. [Neuron](neuron.md)
4. [Neuroscience](neuroscience.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Hyperpolarization](hyperpolarization.md)
- [Inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md)
- [Ionotropic receptor](ionotropic-receptor.md)
- [Membrane time constant](membrane-time-constant.md)
- [Neuron](neuron.md)
- [Passive spatial and conductance integration](passive-spatial-and-conductance-integration.md)
- [Reversal potential](reversal-potential.md)
- [Shunting inhibition](shunting-inhibition.md)
- [Spatial summation](spatial-summation.md)
- [Synapse](synapse.md)
- [Synaptic conductance](synaptic-conductance.md)
- [Synaptic integration](synaptic-integration.md)
- [Synaptic potential](synaptic-potential.md)
