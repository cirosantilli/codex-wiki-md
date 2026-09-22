<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

A fixed-axis diatomic molecule has one bond-stretch vibrational coordinate $q$, reduced mass $m_r$, and angular frequency $\omega$. In the classical harmonic approximation its internal [Hamiltonian](../../../../../hamiltonian.md) is $p^2/(2m_r)+m_r\omega^2q^2/2$. The phase-space contribution per molecule is

$$
z_{\rm vib}=\frac1h\int_{\mathbb R^2}
\exp\left[-\frac{p^2/(2m_r)+m_r\omega^2q^2/2}{kT}\right]dp\,dq
=\boxed{\frac{2\pi kT}{h\omega}=\frac{kT}{\hbar\omega}.}
$$

The Gaussian integrals cancel the reduced mass. Extending the small bond displacement to the whole real line is the usual harmonic approximation. There is no rotational factor because the molecular orientation is fixed.

For $N$ identical dilute molecules of total mass $M$ in volume $V$, translation supplies $V(2\pi MkT/h^2)^{3/2}$. Including indistinguishability gives

$$
Z=\frac1{N!}\left[V\left(\frac{2\pi MkT}{h^2}\right)^{3/2}
\frac{kT}{\hbar\omega}\right]^N.
$$

Using Stirling's approximation and defining $Q=(V/N)(2\pi MkT/h^2)^{3/2}kT/(\hbar\omega)$,

$$
\boxed{F=-NkT(\log Q+1),\qquad S=-F_T=Nk(\log Q+7/2).}
$$

The $7/2$ is $1+5/2$: the logarithm contains $T^{5/2}$, combining three translational quadratic degrees with two vibrational ones. This is a classical result, valid when vibration is thermally classical rather than quantum frozen.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
