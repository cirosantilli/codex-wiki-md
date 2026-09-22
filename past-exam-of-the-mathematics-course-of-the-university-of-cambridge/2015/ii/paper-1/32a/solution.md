<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

The [Rayleigh quotient](../../../../../rayleigh-quotient.md) is $R[\psi]=\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle$, interpreted through the energy [quadratic form](../../../../../quadratic-form.md) for trial states in its form domain. Expanding in normalized energy eigenstates gives $R[\psi]=\sum E_n|c_n|^2/\sum|c_n|^2\geq E_0$. If the ground state is unique, equality requires all coefficients outside its one-dimensional [eigenspace](../../../../../eigenspace.md) to vanish. Thus equality means the same ground-state ray, allowing normalization and an overall phase.

Use the normalized trial function $\sqrt{2/a}\cos(\pi x/a)$ on $|x|<a/2$, zero outside. Its [kinetic energy](../../../../../kinetic-energy.md) is $\pi^2\hbar^2/(2ma^2)$ and its mean square position is $c_0a^2$, where $c_0=1/12-1/(2\pi^2)$. The energy is

$$
R_0(a)=\frac{\pi^2\hbar^2}{2ma^2}+\frac{m\omega^2c_0a^2}{2}.
$$

Minimization gives $a^4=\pi^2\hbar^2/(m^2\omega^2c_0)$ and

$$
\boxed{E_0\leq\hbar\omega\sqrt{\frac{\pi^2}{12}-\frac12}\approx0.56786\hbar\omega}.
$$

For the first excited well state use $\sqrt{2/a}\sin(2\pi x/a)$, zero outside. Now the [kinetic energy](../../../../../kinetic-energy.md) is $2\pi^2\hbar^2/(ma^2)$ and the position factor is $c_1=1/12-1/(8\pi^2)$. Minimizing gives $a^4=4\pi^2\hbar^2/(m^2\omega^2c_1)$ and

$$
\boxed{E_1\leq\hbar\omega\sqrt{\frac{\pi^2}{3}-\frac12}\approx1.67029\hbar\omega}.
$$

**This particular excited-state estimate is an upper bound.** The trial function is odd and the oscillator ground state is even, so it is exactly orthogonal to the ground state. Its spectral expansion therefore contains only energies at least $E_1$, giving the same variational bound on that orthogonal subspace. An arbitrary trial state without this [orthogonality](../../../../../orthogonal-vectors.md) would bound only $E_0$, not $E_1$. The compactly supported trial functions belong to the quadratic-form domain despite [derivative](../../../../../derivative.md) jumps at the well edges; their kinetic energies are correctly computed as $\hbar^2\int|\psi'|^2/(2m)$.

## ↑ Ancestors (10)

1. [32A](../32a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
