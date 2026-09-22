<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the unitary [discrete Fourier transform](../../../../discrete-fourier-transform-split.md)

$$
a_j=\frac1{\sqrt L}\sum_ke^{ikj}b_k,\qquad b_k=\frac1{\sqrt L}\sum_je^{-ikj}a_j,\qquad k=\frac{2\pi\ell}{L},\quad \ell=0,\ldots,L-1.
$$

The finite-sum orthogonality identity gives $[b_k,b_q^\dagger]=\delta_{kq}$. It also gives $\sum_ja_{j+1}^\dagger a_j=\sum_ke^{-ik}b_k^\dagger b_k$. Substituting $A,B$ from [solution](../c/solution.md) therefore gives the [dispersion relation](../../../../dispersion-relation-split.md)

$$
\boxed{H_{\rm LSW}=\sum_k\epsilon(k)b_k^\dagger b_k,\qquad\epsilon(k)=2S[J(1+u)-J\cos k-D\sin k].}
$$

Using the opposite sign in the [Fourier transform](../../../../fourier-transform-split.md) reverses $k$ and the sine term together, without changing the spectrum.

For $u\gg1$ every $\epsilon(k)>0$, so the [ground state](../../../../ground-state.md) of this quadratic [Hamiltonian](../../../../hamiltonian.md) is the bosonic vacuum, $b_k|{\rm GS}\rangle=0$ for every $k$. In the original [spin](../../../../spin.md) variables it is the fully $+z$ polarized product state. Its [energy](../../../../energy-split.md) is zero after the constant subtraction. Repeating the construction about the fully $-z$ polarized state describes the other easy-axis sector of the original [Hamiltonian](../../../../hamiltonian.md).

A one-[magnon](../../../../magnon.md) excitation $b_k^\dagger|{\rm GS}\rangle$ has [energy](../../../../energy-split.md) $\epsilon(k)$ above the reference [ground state](../../../../ground-state.md). A normalized many-[magnon](../../../../magnon.md) [Fock state](../../../../fock-state.md) with occupations $n_k$ has excitation [energy](../../../../energy-split.md) $\sum_kn_k\epsilon(k)$, within the dilute regime of the [linear spin-wave approximation](../../../../linear-spin-wave-approximation.md). The lowest excitation in this sector has the minimum allowed $\epsilon(k)$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
