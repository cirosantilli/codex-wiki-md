<h1 id="13b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [Laplacian](../../../../../../laplacian.md) mode with $\nabla^2=-k^2$, the linearized [chemotaxis](../../../../../../chemotaxis.md) system is

$$
\frac d{dt}\binom uv=
\begin{pmatrix}-\gamma n_0-D_nk^2&\chi n_0k^2\\\alpha&-\beta-D_ck^2\end{pmatrix}\binom uv.
$$

Its [trace](../../../../../../matrix-trace.md) is negative for all $k$. Writing $s=k^2$, its [determinant](../../../../../../determinant.md) is

$$
D_nD_cs^2+(\beta D_n+\gamma n_0D_c-\chi\alpha n_0)s+\beta\gamma n_0.
$$

Instability occurs when this [determinant](../../../../../../determinant.md) is negative, because then one real [eigenvalue](../../../../../../eigenvalue.md) is positive. A quadratic with positive leading and constant coefficients is negative for some $s>0$ precisely when its middle coefficient is negative and its discriminant positive. These conditions combine to

$$
\boxed{\chi\alpha n_0>\beta D_n+\gamma n_0D_c+2\sqrt{\beta\gamma n_0D_nD_c}.}
$$

This proves the printed threshold. In a bounded spatial domain, only its permitted [Laplacian](../../../../../../laplacian.md) eigenmodes are available; the continuous-$k$ threshold describes the onset when wavenumbers can vary freely.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13B](../../13b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
