<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The variables $y_j=I_je^{i\Omega_j}$ are [complex inclinations](../../../../../../complex-inclination.md), despite the question's description as eccentricities. Diagonalize the [Laplace-Lagrange inclination matrix](../../../../../../laplace-lagrange-inclination-matrix.md): let real [eigenvectors](../../../../../../eigenvector.md) $\mathbf v_k$ satisfy $B\mathbf v_k=\lambda_k\mathbf v_k$, and form $V=(\mathbf v_1,\mathbf v_2,\mathbf v_3)$. The physical matrix is diagonalizable by [positive diagonal symmetrization of a matrix](../../../../../../positive-diagonal-symmetrization-of-a-matrix.md), as shown below.

The [matrix exponential](../../../../../../matrix-exponential.md) solution is

$$
\mathbf y(t)=e^{iBt}\mathbf y(0)
=\sum_{k=1}^3 c_k\mathbf v_ke^{i\lambda_kt},\qquad
(c_1,c_2,c_3)^T=V^{-1}\mathbf y(0).
$$

Write $c_k=I_ke^{i\gamma_k}$ with $I_k\ge0$, and define $I_{jk}=I_kv_{jk}$. This gives

$$
\boxed{y_j(t)=\sum_{k=1}^3I_{jk}e^{i(\lambda_kt+\gamma_k)}.}
$$

The [eigenvalues](../../../../../../eigenvalue.md) determine nodal precession frequencies, the [eigenvectors](../../../../../../eigenvector.md) determine relative inclinations within each [secular eigenmode](../../../../../../secular-eigenmode.md), and the initial [complex inclinations](../../../../../../complex-inclination.md) determine their amplitudes and phases. The real $I_{jk}$ can have either sign, encoding opposite nodal phases. The zero-frequency mode is a common fixed tilt.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
