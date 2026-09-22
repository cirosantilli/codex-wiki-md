<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Changing the summation variable from $y$ to $z=y+1$ gives

$$
S|\xi_x\rangle
=\frac1{\sqrt d}\sum_y\omega_d^{xy}|y+1\rangle
=\omega_d^{-x}\frac1{\sqrt d}\sum_z\omega_d^{xz}|z\rangle
=\boxed{\omega_d^{-x}|\xi_x\rangle}.
$$

Thus the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) diagonalizes the cyclic shift.

For $f:\mathbb Z_m\to\mathbb Z_n$,

$$
U_f=\sum_{x\in\mathbb Z_m}|x\rangle\langle x|\otimes S^{f(x)}.
$$

Consequently the product states

$$
\boxed{|x\rangle|\xi_y\rangle,
\qquad x\in\mathbb Z_m,quad y\in\mathbb Z_n,}
$$

form an [eigenbasis](../../../../../../eigenbasis.md), with corresponding [eigenvalues](../../../../../../eigenvalue.md)

$$
\boxed{\omega_n^{-y f(x)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
