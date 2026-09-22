<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Diagonalize the real [Laplace-Lagrange secular matrix](../../../../../../laplace-lagrange-secular-matrix.md) $\mathbf A$. Its [eigenvalue](../../../../../../eigenvalue.md)s are

$$
\boxed{g_{1,2}=\frac{A_{11}+A_{22}}2
\pm\frac12\sqrt{(A_{11}-A_{22})^2+4A_{12}A_{21}}},
$$

and choose corresponding real [eigenvector](../../../../../../eigenvector.md)s $\mathbf v_k$. If $V=(\mathbf v_1\ \mathbf v_2)$, the initial [complex eccentricity](../../../../../../complex-eccentricity.md) vector determines complex mode coefficients

$$
\mathbf c=V^{-1}\mathbf z(0),
\qquad c_k=|c_k|e^{i\beta_k}.
$$

The [matrix exponential](../../../../../../matrix-exponential.md) solution is

$$
\mathbf z(t)=\sum_{k=1}^2c_k\mathbf v_k e^{ig_kt}.
$$

Thus

$$
\boxed{z_j(t)=\sum_{k=1}^2e_{jk}e^{i(g_kt+\beta_k)}},
\qquad e_{jk}=|c_k|v_{jk},
$$

where a negative eigenvector component may equivalently be made positive by adding $\pi$ to its phase. The $g_k$ are secular precession frequencies, each eigenvector fixes the planets' eccentricity ratio and relative apsidal orientation, and $\beta_k$ fixes the phase selected by the initial conditions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
