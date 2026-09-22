<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each [spin](../../../../spin.md) let $\mathcal F_\sigma$ contain the $N_\sigma$ lowest [tight binding](../../../../tight-binding.md) [energy levels](../../../../energy-level.md), and set $n_\sigma=N_\sigma/M$ and $C_\sigma=M^{-1}\sum_{k\in\mathcal F_\sigma}e^{ik}$. The normalized trial [Slater determinant](../../../../slater-determinant.md) is

$$
|\mathcal F\rangle=\prod_{\sigma}\prod_{k\in\mathcal F_\sigma}\widetilde c^\dagger_{\sigma,k}|0\rangle.
$$

Its nearest-neighbour [one-body density matrix](../../../../one-body-density-matrix.md) is $\langle c^\dagger_{\sigma,j}c_{\sigma,j+1}\rangle=C_\sigma$. By [Wick's theorem](../../../../wick-s-theorem.md), [fermionic exchange symmetry](../../../../fermi-dirac-statistics.md) subtracts the squared off-diagonal [one-body density matrix](../../../../one-body-density-matrix.md) from the direct contribution

$$
\langle n_{\sigma,j}n_{\sigma,j+1}\rangle=n_\sigma^2-|C_\sigma|^2,
\qquad
\boxed{\langle H\rangle=M\sum_\sigma\left[-2t\operatorname{Re}C_\sigma+V(n_\sigma^2-|C_\sigma|^2)\right].}
$$

This formula also specifies the finite-$M$ answer exactly, including partially filled terminal [energy levels](../../../../energy-level.md) through the chosen occupied set. For $N_\sigma$ consecutive allowed [wavevectors](../../../../wavevector.md), $|C_\sigma|=|\sin(\pi N_\sigma/M)|/[M\sin(\pi/M)]$; its phase locates the centre of that occupied interval.

Write $\tau=|t|$. In the large-$M$ limit the [Fermi sea](../../../../fermi-sea.md) is centred at $k_0=0$ for $t>0$ and $k_0=\pi$ for $t<0$, with [Fermi wavevector](../../../../fermi-wavevector.md) $k_{F,\sigma}=\pi n_\sigma$ measured from $k_0$. Consequently

$$
C_\sigma\longrightarrow e^{ik_0}\frac{\sin(\pi n_\sigma)}\pi,\qquad
\boxed{\frac{\langle H\rangle}{M}=\sum_{\sigma=\uparrow,\downarrow}\left[-\frac{2\tau}{\pi}\sin(\pi n_\sigma)+V\left(n_\sigma^2-\frac{\sin^2(\pi n_\sigma)}{\pi^2}\right)\right].}
$$

The subtraction due to [fermionic exchange symmetry](../../../../fermi-dirac-statistics.md) is essential: replacing $\langle n_jn_{j+1}\rangle$ by $n^2$ would discard the suppression of neighbouring equal-[spin](../../../../spin.md) occupation. A completely filled [spin](../../../../spin.md) band has zero [kinetic energy](../../../../kinetic-energy.md) and interaction [energy](../../../../energy-split.md) $MV$, as the formula also shows.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
