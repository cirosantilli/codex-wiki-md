# Linear combination of atomic orbitals

↑ **Parent:** [Molecular orbital theory](molecular-orbital-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_combination_of_atomic_orbitals)

The [LCAO](linear-combination-of-atomic-orbitals.md) approximation builds a [molecular orbital](molecular-orbital.md) as a [linear combination](linear-combination.md) of single-centre [atomic orbitals](atomic-orbital.md). For two equivalent normalized real $1s$ functions $\phi_A$ and $\phi_B$, choose their signs positive and define their [orbital overlap](orbital-overlap.md) $S$. At nonzero separation, $0<S<1$, and the normalized combinations are

$$
\sigma_\pm(\mathbf r)=\frac{\phi_A(\mathbf r)\pm\phi_B(\mathbf r)}{\sqrt{2(1\pm S)}},\qquad
S=\int_{\mathbb R^3}\phi_A(\mathbf r)\phi_B(\mathbf r)\,d^3\mathbf r.
$$

Here $\sigma_+=\sigma_g$ and $\sigma_-=\sigma_u^*$. Equal coefficients use the equivalence of the two centres; a general [LCAO](linear-combination-of-atomic-orbitals.md) need not have equal coefficients. See [Field, MIT 5.61, lecture 24, pp. 3–6: LCAO coefficients and overlap integrals](https://ocw.mit.edu/courses/5-61-physical-chemistry-fall-2017/ef9da1132ff6233d732a1d6115099467_MIT5_61F17_lec24.pdf).

For the [Gaussian function](gaussian-function.md) toy's $a=1$, the two denominators are $\sqrt{2(1+S)}\approx1.654013$ and $\sqrt{2(1-S)}\approx1.124385$. To check [wavefunction normalization](wavefunction-normalization.md), expand the square: $\int(\phi_A\pm\phi_B)^2=1+1\pm2S$. Dividing by $2(1\pm S)$ gives one. The local [probability density](probability-density.md) is

$$
|\sigma_\pm|^2=\frac{\phi_A^2+\phi_B^2\pm2\phi_A\phi_B}{2(1\pm S)}.
$$

The cross term is the [interference](interference-wave-propagation.md); adding the separate densities first would lose it. These formulas normalize the chosen [linear combination](linear-combination.md) exactly, while the restricted choice of [atomic orbitals](atomic-orbital.md) remains an approximation to an actual [molecular orbital](molecular-orbital.md).

**Table of contents**

- [Orbital overlap](orbital-overlap.md)

## ↑ Ancestors (4)

1. [Molecular orbital theory](molecular-orbital-theory.md)
2. [Quantum chemistry](quantum-chemistry.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Atomic orbital](atomic-orbital.md)
- [Molecular orbital theory](molecular-orbital-theory.md)
