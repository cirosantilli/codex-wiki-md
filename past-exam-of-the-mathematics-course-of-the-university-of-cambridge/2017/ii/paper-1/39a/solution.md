<h1 id="39a/solution">Solution</h1>

↑ **Parent:** [39A](../39a.md)

The [Householder-John theorem](../../../../../householder-john-theorem.md) states that if $A=M-N$ is Hermitian positive definite and $M^*+N$ is also Hermitian positive definite, then $M$ is invertible and $\rho(M^{-1}N)<1$. The associated stationary iteration $x^{(k+1)}=M^{-1}Nx^{(k)}+M^{-1}b$ therefore converges from every starting vector. For designing a method, choose a splitting with easily solved $M$ and verify the positive-definiteness condition on $M^*+N$; it is a sufficient certificate and does not require computing every iteration-matrix [eigenvalue](../../../../../eigenvalue.md).

For completeness, put $C=M^*+N=M^*+M-A$. If $Mv=0$ for $v\ne0$, then $v^*Cv=-v^*Av<0$, a contradiction. If $M^{-1}Nv=zv$, then $Av=(1-z)Mv$. The case $z=1$ contradicts invertibility of $A$. Taking scalar products and using Hermitian symmetry gives

$$
(1-|z|^2)v^*Av=|1-z|^2v^*Cv>0,
$$

hence $|z|<1$. The usual spectral-radius convergence criterion now proves the stated conclusion.

For the given scheme take the [matrix splitting](../../../../../matrix-splitting.md)

$$
M=D/\omega+L,\qquad N=(1/\omega-1)D-U.
$$

Since $A$ is real symmetric, $U=L^T$, and since it is positive definite, every diagonal entry in $D$ is positive. Thus

$$
M^T+N=(2/\omega-1)D
$$

is positive definite exactly for $0<\omega<2$. The theorem applies, and the iteration [matrix](../../../../../matrix.md) has [spectral radius](../../../../../spectral-radius.md) below one. The unique solution $x_*=A^{-1}b$ is its [fixed point](../../../../../fixed-point.md), so $x^{(k)}-x_*=(M^{-1}N)^k(x^{(0)}-x_*)\to0$. Therefore

$$
\boxed{x^{(k)}\to A^{-1}b\quad\text{for every }x^{(0)}\text{ and }0<\omega<2}.
$$

The scheme is [successive over-relaxation](../../../../../successive-over-relaxation.md); at $\omega=1$ it becomes the **[Gauss-Seidel method](../../../../../gauss-seidel-method.md)**.

## ↑ Ancestors (10)

1. [39A](../39a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
