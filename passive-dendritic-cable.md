# Passive dendritic cable

↑ **Parent:** [Spatial summation](spatial-summation.md)

A [passive dendritic cable](passive-dendritic-cable.md) models a uniform [dendrite](dendrite.md) with axial [electrical resistance](electrical-resistance.md), membrane leak and [membrane capacitance](membrane-capacitance.md), excluding active [ion channels](ion-channel.md). Let $r_a$ be axial [electrical resistance](electrical-resistance.md) per length, $r_m$ membrane [electrical resistance](electrical-resistance.md) times length, and $c_m$ [membrane capacitance](membrane-capacitance.md) per length. For voltage deviation $v=V-E_L$ from the leak [reversal potential](reversal-potential.md), [electric charge conservation](charge-conservation.md) gives the [partial differential equation](partial-differential-equation-split.md)

$$
c_m\frac{\partial v}{\partial t}=\frac{1}{r_a}\frac{\partial^2v}{\partial x^2}-\frac{v}{r_m}+i(x,t),\qquad \tau_m=r_mc_m,\qquad \lambda=\sqrt{\frac{r_m}{r_a}}.
$$

$i$ is imposed inward [electric current](electric-current.md) per length. Units are $r_a:\Omega/\mathrm m$, $r_m:\Omega\,\mathrm m$ and $c_m:\mathrm F/\mathrm m$, so $\tau_m$ is a time and $\lambda$ a length. On a source-free semi-infinite cable with imposed $v(0)=v_0$ and $v(x)\to0$ as $x\to\infty$, the [steady state](steady-state.md) is

$$
v(x)=v_0e^{-x/\lambda}.
$$

Differentiate twice to verify the [ordinary differential equation](ordinary-differential-equation.md) $\lambda^2v''-v=0$. At $x=\lambda$, the amplitude is $e^{-1}\approx0.368$ of the boundary amplitude. This is a stationary attenuation law, not the complete waveform of a brief [EPSP](excitatory-postsynaptic-potential.md). Transient passive spread also broadens and delays responses. Finite ends, branch points and the [soma](soma-biology.md)'s load alter the solution; distance alone cannot specify every real [synaptic potential](synaptic-potential.md).[§3.2.1, equations (3.17)–(3.20): passive cable and length scale; §3.2.2, Figure 3.7: transient attenuation and delay](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/3-2-spatial-structure-the-dendritic-tree.md)

## ↑ Ancestors (6)

1. [Spatial summation](spatial-summation.md)
2. [Synaptic integration](synaptic-integration.md)
3. [Neuron](neuron.md)
4. [Neuroscience](neuroscience-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Dendritic spike](dendritic-spike.md)
- [Passive dendritic cable](passive-dendritic-cable.md)
- [Spatial summation](spatial-summation.md)
- [Temporal summation](temporal-summation.md)
