# Synaptic potential

↑ **Parent:** [Synapse](synapse.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Synaptic_potential)

A [synaptic potential](synaptic-potential.md) is a postsynaptic change in [membrane potential](membrane-potential.md) caused by activity at a [synapse](synapse.md). Unlike the regenerative [action potential](action-potential.md), a passive [synaptic potential](synaptic-potential.md) is graded: its size depends on input strength, the initial [membrane potential](membrane-potential.md) and the receiving [cell membrane](cell-membrane.md)'s properties. Local voltage changes can decay before reaching the [soma](soma-biology.md); their timing and overlap help determine whether an [action potential](action-potential.md) follows. See [Ion Channels and the Electrical Properties of Membranes](molecular-biology-of-the-cell-4th-edition-by-bruce-alberts-and-others/ion-channels-and-the-electrical-properties-of-membranes.md).

[Depolarization](depolarization.md) means that the interior becomes less negative relative to the exterior; [hyperpolarization](hyperpolarization.md) means that it becomes more negative. Excitation and inhibition instead describe whether an input promotes or opposes postsynaptic [action potential](action-potential.md) generation. An [inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md) can be depolarizing, and [shunting inhibition](shunting-inhibition.md) can occur with no voltage change at rest. The [receptor](receptor-biochemistry.md), permeating [ions](ion.md), ionic gradients and [reversal potential](reversal-potential.md) matter. See [Purves and colleagues: excitation, inhibition and depolarizing inhibition](https://www.ncbi.nlm.nih.gov/books/NBK11117/).

A worked passive model treats the receiving membrane as one compartment with [capacitance](capacitance.md) $C>0$, leak conductance $g_L>0$, and activated synaptic conductances $g_e,g_i\geq0$:

$$
C\frac{dV}{dt}=g_L(E_L-V)+g_e(E_e-V)+g_i(E_i-V)+I_{\mathrm{ext}}.
$$

All [electric currents](electric-current.md) are inward-positive. Each term $g(E-V)$ vanishes at its [reversal potential](reversal-potential.md) $E$; $\mathrm{nS}\times\mathrm{mV}=\mathrm{pA}$. With constant parameters, the [ordinary differential equation](ordinary-differential-equation.md) has

$$
G=g_L+g_e+g_i,\qquad V_\infty=\frac{g_LE_L+g_eE_e+g_iE_i+I_{\mathrm{ext}}}{G},\qquad \tau=\frac{C}{G},
$$



$$
V(t)=V_\infty+(V(0)-V_\infty)e^{-t/\tau}.
$$

Here $G$ is total conductance, $1/G$ is effective [electrical resistance](electrical-resistance.md), $V_\infty$ is the [steady state](steady-state.md) and $\tau$ the [time constant](time-constant.md). Without imposed [electric current](electric-current.md), $V_\infty$ is a conductance-weighted average of the [reversal potentials](reversal-potential.md). This approximation omits spatial structure, changing ionic gradients and active [voltage-gated ion channels](voltage-gated-ion-channel.md); it calculates passive voltage responses, not actual [action potential](action-potential.md) waveforms. See [3.1 Synapses](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/3-1-synapses.md) for the mechanism behind the terms; the inward-positive convention here reverses that source's synaptic-current sign.

Take the same illustrative leak and [capacitance](capacitance.md) as under [shunting inhibition](shunting-inhibition.md), start at $V(0)=-65\,\mathrm{mV}$ and set $I_{\mathrm{ext}}=0$. Opening $g_e=2\,\mathrm{nS}$ with $E_e=0\,\mathrm{mV}$ gives $V_\infty=-650/12\simeq-54.167\,\mathrm{mV}$ and $\tau\simeq16.667\,\mathrm{ms}$. Its initial inward [electric current](electric-current.md) is $2(0+65)=130\,\mathrm{pA}$. Adding $g_i=20\,\mathrm{nS}$ with $E_i=-65\,\mathrm{mV}$ changes $V_\infty$ to $(-650-1300)/32=-60.9375\,\mathrm{mV}$ and $\tau=6.25\,\mathrm{ms}$. This is [shunting inhibition](shunting-inhibition.md) of the same excitatory drive.

For comparison, $g_i=20\,\mathrm{nS}$ with $E_i=-75\,\mathrm{mV}$ alone gives $V_\infty\simeq-71.667\,\mathrm{mV}$: [hyperpolarization](hyperpolarization.md). With $E_i=-60\,\mathrm{mV}$ instead, it alone gives $V_\infty\simeq-61.667\,\mathrm{mV}$: [depolarization](depolarization.md). Yet adding this depolarizing conductance to the $g_e=2\,\mathrm{nS}$ excitatory drive lowers that drive's $V_\infty$ from $-54.167$ to $(-650-1200)/32=-57.8125\,\mathrm{mV}$. At an illustrative firing threshold $V=-50\,\mathrm{mV}$, its [electric current](electric-current.md) is $20(-60+50)=-200\,\mathrm{pA}$, opposing threshold approach. The combined trace initially rises faster than the excitatory drive alone, before settling below it. Thus the sign of a voltage change at rest alone does not determine excitation or inhibition; a claim about firing must specify input strength, timing and the [neuron](neuron.md)'s state.

<a id="image-reversal-potential-passive-synaptic-potentials-and-shunting-inhibition"></a>
![](synaptic-conductance-and-shunting.png)

**[Figure 52](#image-reversal-potential-passive-synaptic-potentials-and-shunting-inhibition). Reversal potential, passive synaptic potentials and shunting inhibition**. Computed illustrations, not recordings. Left: inward [electric current](electric-current.md) for a $1\,\mathrm{nS}$ conductance with four [reversal potentials](reversal-potential.md). Upper right: constant-conductance steps at time zero in the one-compartment model with $C=200\,\mathrm{pF}$, $g_L=10\,\mathrm{nS}$ and $E_L=V(0)=-65\,\mathrm{mV}$. Lower right: the same $100\,\mathrm{pA}$ test [electric current](electric-current.md) with and without $20\,\mathrm{nS}$ of added conductance at $E_i=-65\,\mathrm{mV}$. All plotted trajectories are passive; no [action potential](action-potential.md) generation or reset is included.

**Table of contents**

- [Synaptic conductance](synaptic-conductance.md)
- [Excitatory postsynaptic potential](excitatory-postsynaptic-potential.md)
- [Inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md)

## ↑ Ancestors (5)

1. [Synapse](synapse.md)
2. [Neuron](neuron.md)
3. [Neuroscience](neuroscience.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Chemical synapse](chemical-synapse.md)
- [Current clamp](current-clamp.md)
- [Depolarization](depolarization.md)
- [Excitatory postsynaptic potential](excitatory-postsynaptic-potential.md)
- [Inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md)
- [Neuron](neuron.md)
- [Passive dendritic cable](passive-dendritic-cable.md)
- [Passive spatial and conductance integration](passive-spatial-and-conductance-integration.md)
- [Shunting inhibition](shunting-inhibition.md)
- [Spatial summation](spatial-summation.md)
- [Synapse](synapse.md)
- [Synaptic conductance](synaptic-conductance.md)
- [Synaptic integration](synaptic-integration.md)
- [Synaptic potential](synaptic-potential.md)
