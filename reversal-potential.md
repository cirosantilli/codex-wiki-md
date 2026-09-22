# Reversal potential

↑ **Parent:** [Membrane potential](membrane-potential-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reversal_potential)

A [reversal potential](reversal-potential.md) $E_{\mathrm{rev}}$ is a [membrane potential](membrane-potential-split.md) at which a specified open [ion channel](ion-channel.md), or specified combination of [ion channels](ion-channel.md), carries zero net [electric current](electric-current.md), with the surrounding conditions fixed; the [electric current](electric-current.md) changes sign across that voltage. Specifying which current matters: an individual [ion](ion.md) contribution and a sum of several contributions can reverse at different voltages. Zero net [electric current](electric-current.md) does not mean that all [ions](ion.md) have stopped moving. See [Purves et al., Neuroscience, 2nd edition (2001): reversal of a mixed-ion channel current](https://www.ncbi.nlm.nih.gov/books/NBK11013/).

Throughout these examples, [membrane potential](membrane-potential-split.md) is $V=V_{\mathrm{inside}}-V_{\mathrm{outside}}$, and **[conventional current](conventional-current.md) is inward-positive**. Positive [electric current](electric-current.md) corresponds to net positive [electric charge](electric-charge-split.md) entering or net negative [electric charge](electric-charge-split.md) leaving. Negative [electric current](electric-current.md) corresponds to the reverse charge transfer. A convenient Ohmic approximation is

$$
I_{\mathrm{in}}=g(E_{\mathrm{rev}}-V),\qquad g\geq0,
$$

where $g$ is the available [electrical conductance](electrical-conductance.md). For fixed $g>0$, $V<E_{\mathrm{rev}}$ gives positive [electric current](electric-current.md), $V=E_{\mathrm{rev}}$ gives zero, and $V>E_{\mathrm{rev}}$ gives negative [electric current](electric-current.md); the line has slope $-g$. If $g=0$, the modeled pathway carries zero [electric current](electric-current.md) at every voltage: closing it does not locate its [reversal potential](reversal-potential.md). [3.1 Synapses](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/3-1-synapses.md) (§3.1: conductance-based synaptic current) uses outward-positive $g(V-E)$; the formula here reverses that sign to match this wiki's inward-positive convention.

For the stipulated single-pathway example from [ion channel](ion-channel.md), $E_{\mathrm{rev}}=-80\,\mathrm{mV}$ and $g=10\,\mathrm{nS}$ give

$$
\begin{array}{c|rrr}
V\ (\mathrm{mV})&-100&-80&-60\\
E_{\mathrm{rev}}-V\ (\mathrm{mV})&20&0&-20\\
I_{\mathrm{in}}\ (\mathrm{pA})&200&0&-200
\end{array}
$$

The open [ion channel](ion-channel.md) carries zero net [electric current](electric-current.md) at $-80\,\mathrm{mV}$ even though $g$ remains positive. Near that point a change of [membrane potential](membrane-potential-split.md) changes the [electric current](electric-current.md), which is why zero current at one voltage does not make an open pathway electrically irrelevant; see [shunting inhibition](shunting-inhibition.md).

<a id="image-inward-positive-electric-current-one-reversal-and-two-channel-cancellation"></a>
![](ion-channel-current-and-reversal.png)

**[Figure 3](#image-inward-positive-electric-current-one-reversal-and-two-channel-cancellation). Inward-positive electric current: one reversal and two-channel cancellation**. Original computed curves for stipulated constant [electrical conductances](electrical-conductance.md) and fixed [reversal potentials](reversal-potential.md). Left: $g=10\,\mathrm{nS}$, $E_{\mathrm{rev}}=-80\,\mathrm{mV}$. Right: a [potassium](potassium.md) pathway with $g_{\mathrm K}=10\,\mathrm{nS}$, $E_{\mathrm K}=-80\,\mathrm{mV}$ and a [sodium](sodium.md) pathway with $g_{\mathrm{Na}}=2\,\mathrm{nS}$, $E_{\mathrm{Na}}=+50\,\mathrm{mV}$. Their net [electric current](electric-current.md) vanishes at $-58.3333\,\mathrm{mV}$ while both individual [electric currents](electric-current.md) remain nonzero. These are model values, not empirical measurements.

For an [ion channel](ion-channel.md) passing only one [ion](ion.md) species by [passive transport](passive-transport.md), its [reversal potential](reversal-potential.md) can equal that species' [Nernst equilibrium potential](nernst-equilibrium-potential.md), where the chemical and electrical contributions to [electrochemical potential](electrochemical-potential.md) balance. At that [thermodynamic equilibrium](thermodynamic-equilibrium.md), passage in both directions can continue with no net transport. For an [ion channel](ion-channel.md) admitting several [ion](ion.md) species, opposing contributions can cancel while each species continues to have net transport. Such a [reversal potential](reversal-potential.md) is not generally any one species' [Nernst equilibrium potential](nernst-equilibrium-potential.md). See the Purves reference above.

To work out that cancellation explicitly, put two Ohmic [ion channel](ion-channel.md) populations across the same [cell membrane](cell-membrane-split.md). Stipulate constant [electrical conductances](electrical-conductance.md) and fixed [reversal potentials](reversal-potential.md):

$$
g_{\mathrm K}=10\,\mathrm{nS},\quad E_{\mathrm K}=-80\,\mathrm{mV},\qquad g_{\mathrm{Na}}=2\,\mathrm{nS},\quad E_{\mathrm{Na}}=+50\,\mathrm{mV}.
$$

The [potassium](potassium.md) and [sodium](sodium.md) contributions add because both pathways experience the same [membrane potential](membrane-potential-split.md):

$$
\begin{aligned}
I_{\mathrm{total}}&=g_{\mathrm K}(E_{\mathrm K}-V)+g_{\mathrm{Na}}(E_{\mathrm{Na}}-V)\\
&=(g_{\mathrm K}+g_{\mathrm{Na}})(E_{\mathrm{eff}}-V),\\
E_{\mathrm{eff}}&=\frac{g_{\mathrm K}E_{\mathrm K}+g_{\mathrm{Na}}E_{\mathrm{Na}}}{g_{\mathrm K}+g_{\mathrm{Na}}}
=\frac{-700}{12}\,\mathrm{mV}\approx-58.3333\,\mathrm{mV}.
\end{aligned}
$$

Thus $I_{\mathrm{total}}=12\,\mathrm{nS}(E_{\mathrm{eff}}-V)$. This [weighted mean](weighted-arithmetic-mean.md) follows simply by expanding and regrouping the two current terms; it assumes additive Ohmic contributions and a positive total [electrical conductance](electrical-conductance.md). At $V=E_{\mathrm{eff}}$, the inward-positive individual [electric currents](electric-current.md) are

$$
I_{\mathrm K}=-\frac{650}{3}\,\mathrm{pA}\approx-216.6667\,\mathrm{pA},\qquad
I_{\mathrm{Na}}=+\frac{650}{3}\,\mathrm{pA}\approx+216.6667\,\mathrm{pA}.
$$

The [potassium](potassium.md) contribution is outward and the [sodium](sodium.md) contribution inward. Equal and opposite [electric currents](electric-current.md) give $I_{\mathrm{total}}=0$; neither pathway has stopped transporting its [ions](ion.md). The calculation treats two distinct pathways. Applying it to one mixed-species [ion channel](ion-channel.md) would additionally require a justified decomposition into independent Ohmic contributions; a general mixed-channel [reversal potential](reversal-potential.md) cannot be obtained by assuming those hypotheses silently.

This is an instantaneous balance of the specified passive [electric currents](electric-current.md). It would be the stationary voltage of a passive [capacitance](capacitance.md) model containing only these constant pathways and no applied [electric current](electric-current.md), but it is not a complete prediction of a living cell's resting [membrane potential](membrane-potential-split.md). Other [electric currents](electric-current.md), voltage-dependent gating, and pumps involved in [active transport](active-transport.md) can matter. Pumps that transfer net [electric charge](electric-charge-split.md) are electrogenic and contribute their own [electric current](electric-current.md). See [Purves et al.: functional properties of the sodium/potassium pump](https://www.ncbi.nlm.nih.gov/books/NBK10857/).

The toy model holds [ion](ion.md) [concentrations](concentration.md) and therefore the stipulated [reversal potentials](reversal-potential.md) fixed. Continuing inward [sodium](sodium.md) and outward [potassium](potassium.md) transport would change finite reservoirs unless [active transport](active-transport.md) or external control maintained them. Transport can be a small fraction of the reservoir's [ions](ion.md) over a short interval, making fixed [concentrations](concentration.md) a useful approximation; it is not a claim that the reservoirs never change. See [Gerstner et al., Neuronal Dynamics (2014), §2.1: equilibrium potentials, channel currents and maintained gradients](https://neuronaldynamics.epfl.ch/online/Ch2.S1.html).

A [reversal potential](reversal-potential.md) makes the effect of opening an [ion channel](ion-channel.md) predictable from the present [membrane potential](membrane-potential-split.md). The same open pathway can carry inward or outward [electric current](electric-current.md) as $V$ crosses its [reversal potential](reversal-potential.md). The two-pathway example reveals a particularly useful distinction: zero net charge transfer can coexist with continuing exchange of different substances. That distinction connects [membrane transport](membrane-transport.md) to [electric current](electric-current.md) measurements without mistaking electrical balance for [thermodynamic equilibrium](thermodynamic-equilibrium.md).

**Table of contents**

- [Nernst equilibrium potential](nernst-equilibrium-potential.md)

## ↑ Ancestors (4)

1. [Membrane potential](membrane-potential-split.md)
2. [Biological cell](biological-cell-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Hodgkin-Huxley model](hodgkin-huxley-model.md)
- [Ion channel](ion-channel.md)
- [Ionotropic receptor](ionotropic-receptor.md)
- [Leaky integrate-and-fire model](leaky-integrate-and-fire-model.md)
- [Membrane potential](membrane-potential-split.md)
- [Metabotropic receptor](metabotropic-receptor.md)
- [Nernst equilibrium potential](nernst-equilibrium-potential.md)
- [Passive dendritic cable](passive-dendritic-cable.md)
- [Passive membrane response in current clamp](passive-membrane-response-in-current-clamp.md)
- [Passive spatial and conductance integration](passive-spatial-and-conductance-integration.md)
- [Patch-clamp series resistance](patch-clamp-series-resistance.md)
- [Reversal potential](reversal-potential.md)
- [Shunting inhibition](shunting-inhibition.md)
- [Single-channel current-voltage relation](single-channel-current-voltage-relation.md)
- [Spatial summation](spatial-summation.md)
- [Synapse](synapse.md)
- [Synaptic integration](synaptic-integration.md)
- [Synaptic potential](synaptic-potential.md)
- [Two-state ion-channel gating](two-state-ion-channel-gating.md)
