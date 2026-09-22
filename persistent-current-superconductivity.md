# Persistent current (superconductivity)

↑ **Parent:** [Superconductivity](superconductivity-split.md)

A [superconducting persistent current](persistent-current-superconductivity.md) is an [electric current](electric-current.md) circulating in a closed path with [superconductivity](superconductivity-split.md) after the external driving [electromotive force](electromotive-force.md) has ceased. Its associated [magnetic field](magnetic-field-split.md) makes the circulation observable without inserting a measuring instrument into the path. This article concerns macroscopic circulation in [superconductivity](superconductivity-split.md). A finite experiment establishes persistence over its observation window with a stated [measurement error](measurement-error.md), rather than directly observing an infinite lifetime.

The ideal circuit connection is [flux conservation in a superconducting loop](flux-conservation-in-a-superconducting-loop.md). In a fixed loop with [self-inductance](self-inductance.md) $L$, a single circulating [electric current](electric-current.md) $I$, and externally imposed linked [magnetic flux](magnetic-flux.md) $\Phi_{\rm ext}$, the lumped circuit approximation gives

$$
L\frac{dI}{dt}+RI=-\frac{d\Phi_{\rm ext}}{dt}.
$$

When the [electrical resistance](electrical-resistance.md) $R$ vanishes, integrating gives $LI+\Phi_{\rm ext}=\text{constant}$. Removing the external linked [magnetic flux](magnetic-flux.md) therefore changes the circulating [electric current](electric-current.md); holding it fixed afterwards preserves that [electric current](electric-current.md). This is a circuit approximation with a specified [self-inductance](self-inductance.md), not a derivation of the microscopic state of [superconductivity](superconductivity-split.md). For thin paths where the carrier contribution matters, [fluxoid and flux quantization in a superconductor](fluxoid-and-flux-quantization-in-a-superconductor.md) supplies the more careful description.

For constant $L>0$, constant effective [electrical resistance](electrical-resistance.md) $R\geq0$, and no changing external linked [magnetic flux](magnetic-flux.md), the [RL circuit](rl-circuit.md) instead predicts

$$
I(t)=I_0e^{-Rt/L},\qquad \tau=\frac{L}{R}\quad(R>0).
$$

This [exponential decay](exponential-decay.md) follows by separating $dI/I=-(R/L)dt$. A long relaxation time tests extremely small [electrical resistance](electrical-resistance.md) without trying to resolve an equally tiny steady [electric potential difference](electric-potential-difference.md). The stored [magnetic energy](magnetic-energy.md) is $U=LI^2/2$, so the same model gives $dU/dt=-RI^2$, exactly the [Joule heating](joule-heating.md) loss. The finite [energy](energy-split.md) stored in the loop supplies the magnetic readout; the circulating [electric current](electric-current.md) is not a continuously powered source of useful work.

## ↑ Ancestors (5)

1. [Superconductivity](superconductivity-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
