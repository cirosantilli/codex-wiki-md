# Rotational partition functions of hydrogen

↑ **Parent:** [Spin isomers of hydrogen](spin-isomers-of-hydrogen.md)

Write the [linear rigid rotor](linear-rigid-rotor.md) [energy eigenvalues](energy-eigenvalue-split.md) as $E_J=k_{\rm B}\theta_r J(J+1)$, where $\theta_r=\hbar^2/(2Ik_{\rm B})=hB/k_{\rm B}$ is the rotational [temperature](temperature-split.md) scale, $I$ the [moment of inertia](moment-of-inertia.md), $B$ the frequency-valued [rotational constant](rotational-constant.md), and $k_{\rm B}$ the [Boltzmann constant](boltzmann-constant.md). Put $t=T/\theta_r$ and $\epsilon_J=J(J+1)$. Define sums that include rotational multiplicity but exclude nuclear-spin multiplicity:

$$
q_{\rm p}(t)=\sum_{J\ \mathrm{even}}(2J+1)e^{-\epsilon_J/t},\qquad
q_{\rm o}(t)=\sum_{J\ \mathrm{odd}}(2J+1)e^{-\epsilon_J/t}.
$$

The [canonical partition function](canonical-partition-function.md) for one equilibrating internal rotor is $q_{\rm eq}=q_{\rm p}+3q_{\rm o}$, so its equilibrium [orthohydrogen](orthohydrogen.md) fraction is

$$
x_{\rm o}^{\rm eq}=\frac{3q_{\rm o}}{q_{\rm p}+3q_{\rm o}},\qquad
\frac{x_{\rm o}^{\rm eq}}{1-x_{\rm o}^{\rm eq}}=\frac{3q_{\rm o}}{q_{\rm p}}.
$$

For $t\ll1$, the lowest allowed levels give $q_{\rm p}\simeq1$ and $q_{\rm o}\simeq3e^{-2/t}$, hence $x_{\rm o}^{\rm eq}\simeq9e^{-2/t}/(1+9e^{-2/t})\to0$. For $t\gg1$, the densely populated even and odd ladders have equal leading sums, $q_{\rm p}\sim q_{\rm o}\sim t/2$, hence $x_{\rm o}^{\rm eq}\to3/4$. The factor nine belongs to the low-[temperature](temperature-split.md) two-level approximation, and the factor three to the high-[temperature](temperature-split.md) spin multiplicities.

A frozen mixture requires two separately normalized [probability distributions](probability-distribution-split.md),

$$
p(J\mid\mathrm p)=\frac{(2J+1)e^{-\epsilon_J/t}}{q_{\rm p}}\quad(J\ \mathrm{even}),\qquad
p(J\mid\mathrm o)=\frac{(2J+1)e^{-\epsilon_J/t}}{q_{\rm o}}\quad(J\ \mathrm{odd}).
$$

Multiply these by the prescribed fractions $1-x$ and $x$, respectively. The nuclear-spin factor three cancels from the conditional [orthohydrogen](orthohydrogen.md) distribution. For fixed counts $N_{\rm o}$ and $N_{\rm p}$, the internal part of the many-[molecule](molecule-split.md) [partition function](canonical-partition-function.md) is proportional to $q_{\rm p}^{N_{\rm p}}(3q_{\rm o})^{N_{\rm o}}$, with combinatorial factors independent of [temperature](temperature-split.md). Its logarithm yields the two conditional means weighted by the fixed counts. Using $q_{\rm p}+3q_{\rm o}$ instead would silently permit conversion and change the physical constraint.

**Table of contents**

- [Hydrogen rotational heat capacity](hydrogen-rotational-heat-capacity.md)

## ↑ Ancestors (7)

1. [Spin isomers of hydrogen](spin-isomers-of-hydrogen.md)
2. [Homonuclear diatomic molecule](homonuclear-diatomic-molecule.md)
3. [Diatomic molecule](diatomic-molecule.md)
4. [Linear molecule](linear-molecule.md)
5. [Molecule](molecule-split.md)
6. [Chemistry](chemistry-split.md)
7. [Codex Wiki](split.md)
