<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the centered [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) in each direction. With $T=\operatorname{tridiag}(1,-2,1)$ put $A=T\otimes I$, $B=I\otimes T$ and $\mu=\Delta t/h^2$. Thus $h^{-2}A$ and $h^{-2}B$ are the physical derivative approximations; the factor $h^{-2}$ has been absorbed into the [Courant number](../../../../../../courant-number.md) in the written update. Equivalently use the scaled derivative [matrices](../../../../../../matrix.md) and the time parameter $\Delta t$.

For a one-dimensional vector with endpoint values $v_0=v_{m+1}=0$,

$$
v^TTv=-\sum_{j=0}^m(v_{j+1}-v_j)^2\leq0.
$$

Thus $A$ and $B$ are real symmetric negative-definite [matrices](../../../../../../matrix.md). An orthonormal [eigenvector](../../../../../../eigenvector.md) basis shows that all [eigenvalues](../../../../../../eigenvalue.md) of each exponential lie in $(0,1]$ for $\mu\geq0$, so

$$
\|E(\mu;A,B)\|_2
\leq\|e^{\mu A/2}\|_2^2\|e^{\mu B}\|_2\leq1.
$$

Iterating gives **$\|U^n\|_2\leq\|U^0\|_2$ for every nonnegative step parameter**, a mesh-independent unconditional [stability](../../../../../../stability-of-a-numerical-method.md) bound. Multiplying the squared norm by the grid-area weight $h^2$ leaves the same estimate. In this natural tensor-grid choice $AB=BA=T\otimes T$, so $E(\mu;A,B)=e^{\mu(A+B)}$: the split update is even the exact semidiscrete diffusion flow. Contractivity of a product of these negative symmetric exponentials would prove [stability](../../../../../../stability-of-a-numerical-method.md) even without commutation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
