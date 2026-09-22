# Inductor

↑ **Parent:** [Self-inductance](self-inductance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inductor)

An [inductor](inductor.md) is an [electrical circuit](electrical-circuit.md) component designed to provide [self-inductance](self-inductance.md), often a coil such as a [solenoid](solenoid.md). An ideal linear [inductor](inductor.md) has constant $L>0$ and zero [electrical resistance](electrical-resistance.md). Its stored [magnetic energy](magnetic-energy.md), with zero chosen at zero [electric current](electric-current.md), is

$$
U=\frac12LI^2.
$$

For [self-inductance](self-inductance.md) $0.5\,\mathrm H$ and [electric current](electric-current.md) $3\,\mathrm A$, this gives $U=2.25\,\mathrm J$. Unlike [Joule heating](joule-heating.md), ideal storage is recoverable: the [inductor](inductor.md) can return [energy](energy.md) to an [electrical circuit](electrical-circuit.md) when its [electric current](electric-current.md) decreases. [OpenStax University Physics 2, §14.3: energy stored by an inductor](https://openstax.org/books/university-physics-volume-2/pages/14-3-energy-in-a-magnetic-field).

The short derivation uses the terminal convention in [self-inductance](self-inductance.md). The [power](power.md) absorbed by an ideal [inductor](inductor.md) is

$$
P_L=v_L I=LI\frac{dI}{dt}=\frac{d}{dt}\left(\frac12LI^2\right).
$$

Starting from zero [electric current](electric-current.md), the [integral](integral.md) of this [power](power.md) gives

$$
U=\int_0^t P_L(t')\,dt'=\int_0^I Li\,di=\frac12LI^2.
$$

Positive $P_L$ increases stored [magnetic energy](magnetic-energy.md); negative $P_L$ returns [energy](energy.md). At constant [electric current](electric-current.md) $3\,\mathrm A$ in the example, $P_L=0$ and induced [electromotive force](electromotive-force.md) is zero, but $U=2.25\,\mathrm J$ still resides in the [magnetic field](magnetic-field.md). The [battery](electric-battery.md) in the steady [RL circuit](rl-circuit.md) supplies [Joule heating](joule-heating.md) in the [electrical resistance](electrical-resistance.md), rather than further increasing the [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md).

<a id="image-stored-magnetic-energy-and-its-release-as-joule-heating-in-an-rl-circuit"></a>
![](inductor-energy-storage-and-release.png)

**[Figure 37](#image-stored-magnetic-energy-and-its-release-as-joule-heating-in-an-rl-circuit). Stored magnetic energy and its release as Joule heating in an RL circuit**. Left: the [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md) during buildup and a separate decay experiment starting at $3\,\mathrm A$. Right: the [power](power.md) of [Joule heating](joule-heating.md) during decay; the shaded [integral](integral.md) over all time is $2.25\,\mathrm J$. The decay path stays closed through [electrical resistance](electrical-resistance.md) $2\,\Omega$ and [self-inductance](self-inductance.md) $0.5\,\mathrm H$.

During the closed-loop release in [RL circuit](rl-circuit.md), stored [magnetic energy](magnetic-energy.md) plus accumulated [Joule heating](joule-heating.md) stays $2.25\,\mathrm J$. A real coil also has [electrical resistance](electrical-resistance.md), so its [Joule heating](joule-heating.md) must be included separately from ideal [inductor](inductor.md) storage. The constant-$L$ formulas assume a fixed linear magnetic response.

## ↑ Ancestors (6)

1. [Self-inductance](self-inductance.md)
2. [Inductance](inductance.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Electrical engineering](electrical-engineering-split.md)
- [Electrical impedance](electrical-impedance.md)
- [Electrical reactance](electrical-reactance.md)
- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
- [Inductance](inductance.md)
- [Inductor](inductor.md)
- [Reactance phase convention](reactance-phase-convention.md)
- [RL circuit](rl-circuit.md)
- [RLC circuit](rlc-circuit.md)
- [Self-inductance](self-inductance.md)
- [Series RLC circuit](series-rlc-circuit.md)
- [Solenoid](solenoid.md)
- [Stored energy of a solenoid](stored-energy-of-a-solenoid.md)
