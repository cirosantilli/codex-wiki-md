# Finite proton-shell correction to hydrogen ground energy

↑ **Parent:** [Hydrogen atom](hydrogen-atom.md)

Model a [proton](proton.md) as a uniformly charged thin [spherical shell](spherical-shell.md) of radius $b$. Write $C=e^2/(4\pi\epsilon_0)$. The [shell theorem](spherical-shell-theorem.md) gives an electron [potential energy](potential-energy.md) $-C/b$ inside the shell and $-C/r$ outside. Relative to a point [Coulomb potential](coulomb-potential-energy.md), the perturbation is consequently $C(1/r-1/b)$ for $r<b$ and zero otherwise.

For the [hydrogen atom](hydrogen-atom.md) [ground state](ground-state.md), [time-independent perturbation theory](time-independent-perturbation-theory.md) gives the [first-order energy correction](first-order-energy-correction.md)

$$
\Delta E=\frac{4C}{a_0^3}\int_0^b e^{-2r/a_0}\left(r-\frac{r^2}{b}\right)\,dr
=\frac{2Cb^2}{3a_0^3}+O\left(\frac{Cb^3}{a_0^4}\right).
$$

Since $E_{1s}=-C/(2a_0)$, the signed fractional change is $\Delta E/E_{1s}=-4b^2/(3a_0^2)+O((b/a_0)^3)$. The correction $\Delta E$ is positive: distributing the positive charge weakens the attraction near the origin and reduces the magnitude of the binding energy. Here $a_0$ is the [Bohr radius](bohr-radius.md) and $b\ll a_0$ is the small-radius approximation.

## ↑ Ancestors (4)

1. [Hydrogen atom](hydrogen-atom.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017/1/c/solution.md)
