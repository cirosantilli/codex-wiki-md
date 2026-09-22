# Passive spatial and conductance integration

↑ **Parent:** [Spatial summation](spatial-summation.md)

The spatial panel uses two compartments with [membrane potentials](membrane-potential.md) $V_s,V_d$, one representing the [soma](soma-biology.md) and one a [dendrite](dendrite.md). Set $v_s=V_s-E_L$, $v_d=V_d-E_L$, with leak [reversal potential](reversal-potential.md) $E_L=-65\,\mathrm{mV}$, each [membrane capacitance](membrane-capacitance.md) $C=100\,\mathrm{pF}$, each leak [electrical conductance](electrical-conductance.md) $g_L=5\,\mathrm{nS}$ and axial [electrical conductance](electrical-conductance.md) $g_c=10\,\mathrm{nS}$. [Electric charge conservation](charge-conservation.md) gives

$$
C\dot v_s=-(g_L+g_c)v_s+g_cv_d+I_s,\qquad C\dot v_d=g_cv_s-(g_L+g_c)v_d+I_d.
$$

This chosen passive model has two decay [time constants](time-constant.md), $C/g_L=20\,\mathrm{ms}$ for the equal-voltage mode and $C/(g_L+2g_c)=4\,\mathrm{ms}$ for the voltage-difference mode. Starting from rest, a $100\,\mathrm{pA}$ step into the [soma](soma-biology.md) gives, with $u$ the time since onset,

$$
v_s(u)=10(1-e^{-u/20})+2(1-e^{-u/4})\quad\mathrm{mV},
$$

while the same step into the [dendrite](dendrite.md) gives

$$
v_s(u)=10(1-e^{-u/20})-2(1-e^{-u/4})\quad\mathrm{mV}.
$$

$u$ is expressed in $\mathrm{ms}$. Their long-time rises are $12$ and $8\,\mathrm{mV}$ respectively. Applying both inputs gives $20(1-e^{-u/20})\,\mathrm{mV}$ exactly: spatial attenuation coexists with linear summation of prescribed [electric currents](electric-current.md). After the steps end, both modes decay with their respective [time constants](time-constant.md). This deliberately coarse model is not a reconstructed [dendrite](dendrite.md) or a fit to the experiment above.

The conductance panels use the existing one-compartment [synaptic potential](synaptic-potential.md) equation, with $C=200\,\mathrm{pF}$, $g_L=10\,\mathrm{nS}$, $E_L=-65\,\mathrm{mV}$ and excitatory [reversal potential](reversal-potential.md) $E_e=0\,\mathrm{mV}$. For a constant excitatory [synaptic conductance](synaptic-conductance.md) $g_e$, the [steady state](steady-state.md) voltage rise and [membrane time constant](membrane-time-constant.md) are

$$
\Delta V_\infty=\frac{g_e(E_e-E_L)}{g_L+g_e},\qquad \tau_{\mathrm{eff}}=\frac{C}{g_L+g_e}.
$$

Each isolated $2\,\mathrm{nS}$ input has a limiting rise $130/12\approx10.833\,\mathrm{mV}$. Adding those isolated rises predicts $21.667\,\mathrm{mV}$, but opening both together gives $260/14\approx18.571\,\mathrm{mV}$. The two conductances share a changing driving force. This is sublinear input summation even though the voltage [ordinary differential equation](ordinary-differential-equation.md) is linear for each prescribed conductance waveform.

Add $g_i=20\,\mathrm{nS}$ with [reversal potential](reversal-potential.md) $E_i=E_L$ to the joint $4\,\mathrm{nS}$ excitation. The limiting rise becomes $260/34\approx7.647\,\mathrm{mV}$ and the [membrane time constant](membrane-time-constant.md) becomes $200/34\approx5.882\,\mathrm{ms}$. The shunt alone leaves rest unchanged. At the joint-excitation-only [steady state](steady-state.md) $V\approx-46.429\,\mathrm{mV}$, however, its inward [electric current](electric-current.md) would be $20(-65+46.429)\approx-371.429\,\mathrm{pA}$: it opposes that excursion. The finite $50\,\mathrm{ms}$ traces in the diagram approach, but need not reach, these limiting voltages. See [shunting inhibition](shunting-inhibition.md) for the constant-[electric current](electric-current.md) comparison.

## ↑ Ancestors (6)

1. [Spatial summation](spatial-summation.md)
2. [Synaptic integration](synaptic-integration.md)
3. [Neuron](neuron.md)
4. [Neuroscience](neuroscience.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Spatial summation](spatial-summation.md)
