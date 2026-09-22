# Stored energy of a solenoid

↑ **Parent:** [Solenoid inductance](solenoid-inductance.md)

The [magnetic energy](magnetic-energy.md) stored in a linear [solenoid](solenoid.md) of constant [self-inductance](self-inductance.md) $L$ is

$$
U=\frac12LI^2,
\qquad
U\approx\frac{B^2}{2\mu_0}A\ell
$$

in the [long-solenoid approximation](long-solenoid-approximation.md). The first formula is an [inductor](inductor.md) relation; the second identifies its storage with [magnetic energy](magnetic-energy.md) in the interior [magnetic field](magnetic-field-split.md), under the vacuum-core approximation. This agreement joins the [electrical circuit](electrical-circuit-split.md) description to the spatial [magnetic field](magnetic-field-split.md) description. The expression $B^2/(2\mu_0)$ is the vacuum magnetic [energy density](energy-density.md). [MIT 8.02 course notes, §11.3: magnetic energy and its density](https://s3.amazonaws.com/edx-textbooks/mit_802_textbook/Chapter11.pdf).

A short derivation starts from the terminal [electric potential difference](electric-potential-difference.md) $v_L=L\,dI/dt$, with positive [electric current](electric-current.md) entering the terminal at higher potential. The absorbed [power](power.md) is $v_LI$, and integrating from zero [electric current](electric-current.md) gives

$$
U=\int_0^I Li\,di=\frac12LI^2.
$$

The result describes recoverable storage in the [inductor](inductor.md); [Joule heating](joule-heating.md) in the wire is a separate expenditure of [energy](energy-split.md). [Feynman lectures, II.17–8: inductance and magnetic energy](https://www.feynmanlectures.caltech.edu/II_17.html#Ch17-S8).

For the long-coil example, $L\approx4.9348\,\mathrm{mH}$ and $I=0.50\,\mathrm A$ give $U\approx6.1685\times10^{-4}\,\mathrm J=0.61685\,\mathrm{mJ}$. Substituting the ideal $B\approx1.256637\,\mathrm{mT}$ and volume $A\ell\approx9.8175\times10^{-4}\,\mathrm{m^3}$ into $B^2A\ell/(2\mu_0)$ gives the same value. Doubling [electric current](electric-current.md) quadruples stored [magnetic energy](magnetic-energy.md). In a real coil, reducing [electric current](electric-current.md) can return this [energy](energy-split.md) to an [electrical circuit](electrical-circuit-split.md), or release it as [Joule heating](joule-heating.md) in a closed [RL circuit](rl-circuit.md).

## ↑ Ancestors (7)

1. [Solenoid inductance](solenoid-inductance.md)
2. [Solenoid](solenoid.md)
3. [Magnetic field](magnetic-field-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
