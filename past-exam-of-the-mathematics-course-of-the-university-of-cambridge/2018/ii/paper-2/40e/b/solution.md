<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Subtracting the fixed point from the [weighted Jacobi method](../../../../../../weighted-jacobi-method.md) gives

$$
\mathbf e^{(\nu+1)}=H_\omega\mathbf e^{(\nu)},
\qquad
\boxed{H_\omega=I-\omega D^{-1}A=I+\frac{\omega}{2}A.}
$$

Put $x=\pi/(n+1)$. Acting on the supplied sine [eigenvector](../../../../../../eigenvector.md) gives

$$
(A\mathbf v_k)_i
=\sin((i-1)kx)-2\sin(ikx)+\sin((i+1)kx)
=[-2+2\cos(kx)]\sin(ikx).
$$

Therefore

$$
\boxed{\lambda_k(A)
=-2+2\cos(kx)
=-4\sin^2\frac{kx}{2},}
$$

and the corresponding eigenvalues of the [iteration matrix](../../../../../../iteration-matrix.md) are

$$
\boxed{\lambda_k(\omega)
=1+\frac{\omega}{2}\lambda_k(A)
=1-\omega+\omega\cos(kx)
=1-2\omega\sin^2\frac{kx}{2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
