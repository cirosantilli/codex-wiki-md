<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Apply a [discrete Fourier transform](../../../../../../discrete-fourier-transform.md), with lattice spacing one:

$$
a_n=\frac1{\sqrt N}\sum_k a_ke^{ikn},\qquad k=\frac{2\pi m}{N}\pmod{2\pi}.
$$

The [wavevectors](../../../../../../wavevector.md) lie in a [Brillouin zone](../../../../../../brillouin-zone.md), which we choose as $[-\pi,\pi)$. Pairing $k$ with $-k$ makes the quadratic [Hamiltonian](../../../../../../hamiltonian.md)

$$
H_2=-NJS^2+\sum_k\left[Aa_k^\dagger a_k+\frac{B_k}{2}(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)\right],\qquad A=2JS,\quad B_k=2JS\cos k.
$$

A [bosonic Bogoliubov diagonalization](../../../../../../bosonic-bogoliubov-diagonalization.md) uses $a_k=\cosh\theta_k\,\alpha_k-\sinh\theta_k\,\alpha_{-k}^\dagger$. The [canonical commutation relations](../../../../../../canonical-commutation-relation.md) hold because $\cosh^2\theta_k-\sinh^2\theta_k=1$. The anomalous terms vanish when $\tanh2\theta_k=B_k/A=\cos k$, giving

$$
H_2=E_0+\sum_k\omega_k\alpha_k^\dagger\alpha_k,\qquad E_0=-NJS^2+\frac12\sum_k(\omega_k-A),\qquad \boxed{\omega_k=\sqrt{A^2-B_k^2}=2JS|\sin k|}.
$$

Near $k=0$ and $k=\pi$, the [dispersion relation](../../../../../../dispersion-relation.md) is linear: $\omega_k\sim2JS|k-k_0|$. These are the low-energy [antiferromagnetic spin waves](../../../../../../antiferromagnetic-spin-wave.md); the two zeroes are related by the two-sublattice description. The transformation is singular at the exact zero modes, which require an infrared regulator or separate treatment of the collective rotation.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
