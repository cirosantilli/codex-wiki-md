# Hodgkin-Huxley model

↑ **Parent:** [Computational neuroscience](computational-neuroscience.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hodgkin-Huxley_model)

A conductance-based [Hodgkin-Huxley model](hodgkin-huxley-model.md) couples [membrane potential](membrane-potential-split.md) to voltage-dependent channel-gating variables. It explains generation of [action potentials](action-potential.md) through regenerative and opposing ionic [electric currents](electric-current.md), while its parameters and channel assumptions determine its biological domain of validity.

In the classical model, $m$ describes [sodium](sodium.md) activation, $h$ describes availability against [sodium](sodium.md) inactivation, and $n$ describes [potassium](potassium.md) activation. Each follows [two-state ion-channel gating](two-state-ion-channel-gating.md), with its own voltage-dependent rates. The available [electrical conductances](electrical-conductance.md) are

$$
g_{\mathrm{Na}}=\bar g_{\mathrm{Na}}m^3h,\qquad g_{\mathrm K}=\bar g_{\mathrm K}n^4.
$$

The barred quantities are maximum [electrical conductances](electrical-conductance.md). The factors have the interpretation of [independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md): three activation factors and a distinct inactivation-availability factor for [sodium](sodium.md), and four identical activation factors for [potassium](potassium.md). Large $h$ means availability; small $h$ means inactivation. These are model assumptions, not a literal structural description of every [ion channel](ion-channel.md). See [Gerstner, Kistler, Naud and Paninski, Neuronal Dynamics (2014), §2.2: model definition and stochastic opening](https://neuronaldynamics.epfl.ch/online/Ch2.S2.html).

With inward-positive [electric current](electric-current.md), a single-compartment form is

$$
C\frac{dV}{dt}=I_{\mathrm{ext}}+g_{\mathrm{Na}}(E_{\mathrm{Na}}-V)+g_{\mathrm K}(E_{\mathrm K}-V)+g_L(E_L-V).
$$

Here $C$ is membrane [capacitance](capacitance.md), $I_{\mathrm{ext}}$ is imposed inward [electric current](electric-current.md), $g_L$ is leak [electrical conductance](electrical-conductance.md), and each $E$ is a [reversal potential](reversal-potential.md). Use consistent units, and either whole-compartment quantities throughout or quantities per membrane area throughout. Opening changes [electrical conductance](electrical-conductance.md); the [reversal potential](reversal-potential.md) and present [membrane potential](membrane-potential-split.md) determine the associated [electric current](electric-current.md). Coupling this equation to the voltage-dependent gates makes a generally nonlinear system of [ordinary differential equations](ordinary-differential-equation.md); a gate's fixed-voltage limit alone does not specify its evolving state during an [action potential](action-potential.md).

The original quantitative account is [Hodgkin and Huxley (1952), A quantitative description of membrane current and its application to conduction and excitation in nerve, Journal of Physiology 117, 500–544, doi:10.1113/jphysiol.1952.sp004764](https://pmc.ncbi.nlm.nih.gov/articles/PMC1392413/). The contrast with the [leaky integrate-and-fire model](leaky-integrate-and-fire-model.md) is useful: here an [action potential](action-potential.md) emerges from evolving ionic [electric currents](electric-current.md), whereas the simpler model records a threshold event and imposes a reset.

## ↑ Ancestors (4)

1. [Computational neuroscience](computational-neuroscience.md)
2. [Neuroscience](neuroscience-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Action potential](action-potential.md)
- [Hodgkin-Huxley model](hodgkin-huxley-model.md)
- [Independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md)
- [Leaky integrate-and-fire model](leaky-integrate-and-fire-model.md)
- [Neuronal refractory period](neuronal-refractory-period.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/2/solution.md)
- [Phenomenological paired-pulse recovery](phenomenological-paired-pulse-recovery.md)
- [Relative neuronal refractory period](relative-neuronal-refractory-period.md)
- [Two-state ion-channel gating](two-state-ion-channel-gating.md)
