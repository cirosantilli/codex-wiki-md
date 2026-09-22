# Solenoid inductance

↑ **Parent:** [Solenoid](solenoid.md)

For a long vacuum-core or air-core [solenoid](solenoid.md) with fixed geometry and linear magnetic response, neglecting end effects gives [self-inductance](self-inductance.md)

$$
L\approx\frac{\mu_0N^2A}{\ell}
=\mu_0n^2A\ell,
\qquad A=\pi a^2.
$$

Here $N$ is the total number of turns, $n=N/\ell$ is the [solenoid turn density](solenoid-turn-density.md), and $A$ is the interior cross-sectional [area](surface-area.md). The reason for the square of $N$ is physical: more turns produce more [magnetic field](magnetic-field.md), and more turns link the resulting [magnetic flux](magnetic-flux.md). Approximately equal [magnetic flux](magnetic-flux.md) $\Phi\approx BA$ through each turn gives [magnetic flux linkage](magnetic-flux-linkage.md) $\Lambda\approx N\Phi\approx\mu_0N^2AI/\ell$; division by the [electric current](electric-current.md) yields $L$. [MIT 8.02 course notes, Example 11.2: self-inductance of a solenoid](https://s3.amazonaws.com/edx-textbooks/mit_802_textbook/Chapter11.pdf).

For the same $N=1000$, $\ell=0.50\,\mathrm m$, and $a=0.025\,\mathrm m$, the [area](surface-area.md) is $A=\pi(0.025)^2\,\mathrm{m^2}\approx1.9635\times10^{-3}\,\mathrm{m^2}$. The long-coil estimate is

$$
L\approx\frac{(1.256637\times10^{-6})(1000)^2\pi(0.025)^2}{0.50}\,\mathrm H
\approx4.9348\,\mathrm{mH}.
$$

At $I=0.50\,\mathrm A$, each turn links approximately $2.4674\times10^{-6}\,\mathrm{Wb}$ and the total [magnetic flux linkage](magnetic-flux-linkage.md) is approximately $2.4674\times10^{-3}\,\mathrm{Wb}$. Their ratio to $I$ is the stated [self-inductance](self-inductance.md). A real finite coil need not give precisely these values: the axial centre correction above is not by itself a correction formula for [inductance](inductance.md), which depends on [magnetic flux](magnetic-flux.md) across all the turns.

At fixed $A$ and $\ell$, doubling $N$ quadruples $L$. At fixed [solenoid turn density](solenoid-turn-density.md) $n$ and [area](surface-area.md) $A$, doubling $\ell$ doubles both $N$ and $L$. These are different changes to the geometry, so there is no contradiction between $L\propto1/\ell$ at fixed $N$ and $L\propto\ell$ at fixed $n$. A magnetic core requires its own [magnetic permeability](permeability-electromagnetism.md) model; nonlinear [magnetization](magnetization.md) can make a constant-$L$ description inadequate.

**Table of contents**

- [Stored energy of a solenoid](stored-energy-of-a-solenoid.md)

## ↑ Ancestors (6)

1. [Solenoid](solenoid.md)
2. [Magnetic field](magnetic-field.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
