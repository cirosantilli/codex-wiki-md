# Electrostatic model of ionic binding

↑ **Parent:** [Ionic bonding](ionic-bonding-split.md)

For two point [electric charges](electric-charge-split.md) in [vacuum](vacuum.md), [Coulomb's law](coulomb-s-law.md) gives the interaction [potential energy](potential-energy.md)

$$
U_{ij}(r_{ij})=\frac{z_i z_j e^2}{4\pi\epsilon_0 r_{ij}},
$$

with zero at infinite separation. Here $r_{ij}$ is the distance between them and $\epsilon_0$ is the [vacuum permittivity](vacuum-permittivity.md). Opposite signs give negative [potential energy](potential-energy.md) and attraction; equal signs give positive [potential energy](potential-energy.md) and repulsion. For a finite collection of distinct point [electric charges](electric-charge-split.md), sum over $i<j$ to count each pair once. A bulk [ionic crystal](ionic-crystal.md) requires the extended lattice sum, including both signs, rather than multiplying one attractive pair by the [coordination number](coordination-number.md).[§8–1, equations (8.1)–(8.3); §8–3, many-neighbour lattice sum](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

At short distances, overlapping [electron density](electron-density.md) makes the simple point-charge picture inadequate. [Quantum mechanics](quantum-mechanics-split.md), including the [Pauli exclusion principle](pauli-exclusion-principle.md), matters to the steep repulsive contribution. Pure attraction proportional to $-1/r$ would collapse as $r\to0$; it cannot set an equilibrium spacing on its own. A useful illustrative model is

$$
U(r)=-\frac{A}{r}+\frac{B}{r^n},\qquad A>0,\quad B>0,\quad n>1.
$$

Here $r$ scales an assumed fixed arrangement, $A$ packages its attractive contribution, and $B/r^n$ represents short-range repulsion. The constants have units [energy](energy-split.md) times length and [energy](energy-split.md) times length to the power $n$, respectively. This is a model, not a fitted description of a named [salt](salt-chemistry.md).[§8–3, close-distance repulsion and limits of a purely electrostatic lattice calculation](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

Differentiating gives $r_0=(nB/A)^{1/(n-1)}$ and $U''(r_0)=(n-1)A/r_0^3>0$, so the stationary spacing is a stable minimum. For the diagram's stipulated $n=9$, put $x=r/r_0$ and $E_0=A(1-1/n)/r_0>0$. Then

$$
\frac{U(r)}{E_0}=\frac{-9/x+1/x^9}{8},\qquad U(r_0)=-E_0.
$$

The [dimensionless](dimensionless-quantity.md) curves show how competing interactions select a spacing. Their [energy](energy-split.md) scale and exponent are synthetic; neither is a measured [lattice energy](lattice-energy.md) or a [melting](melting.md) prediction.

**Table of contents**

- [Madelung constant](madelung-constant.md)

## ↑ Ancestors (4)

1. [Ionic bonding](ionic-bonding-split.md)
2. [Chemical bond](chemical-bond-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)
