<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the endpoint values zero, move the new-level differences to the left and keep the old-level differences on the right. Then $B$ is tridiagonal with diagonal $1+\mu$ and off-diagonal entries $-\mu/2$, while $C$ has diagonal $1-\mu$ and off-diagonal entries $\mu/2$. Thus **$Bu^{n+1}=Cu^n$**.

Part (a) supplies their common [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md). Their [eigenvalues](../../../../../../eigenvalue.md) are $1+\mu(1-\cos\theta_k)$ and $1-\mu(1-\cos\theta_k)$. For $\mu\geq0$, $B$ is invertible, and the step [matrix](../../../../../../matrix.md) $B^{-1}C$ has [eigenvalues](../../../../../../eigenvalue.md)

$$
\eta_k=\frac{1-\mu(1-\cos\theta_k)}{1+\mu(1-\cos\theta_k)},\qquad |\eta_k|\leq1.
$$

Since the eigenbasis is orthonormal, $\|(B^{-1}C)^n\|_2=\max_k|\eta_k|^n\leq1$, uniformly in the number of steps and mesh. Hence the method is **unconditionally stable for every $\mu\geq0$**, which includes all physical positive time steps. For negative $\mu$, every nonzero modal parameter has modulus larger than one whenever its denominator is nonzero; if a denominator vanishes the step is undefined. Thus the algebraic stable range is exactly $[0,\infty)$. This proof uses simultaneous [matrix](../../../../../../matrix.md) diagonalization, not Fourier stability analysis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
