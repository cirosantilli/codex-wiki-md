<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D\in\mathbb R^{M\times M}$ be the [Toeplitz antisymmetric tridiagonal matrix](../../../../../../toeplitz-antisymmetric-tridiagonal-matrix.md) with $D_{m,m+1}=1$, $D_{m,m-1}=-1$, and zero diagonal. Fixed homogeneous endpoint values give the homogeneous update

$$
\left(I-\frac\mu4D\right)u^{n+1}
=\left(I+\frac\mu4D\right)u^n.
$$

The hint gives the eigenvalues

$$
d_j=2i\cos\frac{j\pi}{M+1},
\qquad 1\leq j\leq M.
$$

Because each $d_j$ is purely imaginary, $1-(\mu/4)d_j\ne0$ for every real $\mu$, so the left matrix is invertible. The two matrices are polynomials in $D$ and therefore have the same orthonormal eigenvectors. The amplification matrix

$$
Q=\left(I-\frac\mu4D\right)^{-1}
\left(I+\frac\mu4D\right)
$$

has eigenvalues

$$
q_j=
\frac{1+i(\mu/2)\cos(j\pi/(M+1))}
{1-i(\mu/2)\cos(j\pi/(M+1))}.
$$

The numerator and denominator are complex conjugates, so $|q_j|=1$. Moreover, the common orthonormal eigenbasis makes $Q$ a [normal matrix](../../../../../../normal-matrix.md). By the [matrix 2-norm of a normal matrix](../../../../../../matrix-2-norm-of-a-normal-matrix.md),

$$
\lVert Q^n\rVert_2=\rho(Q^n)=1
$$

for every $n$. Thus the [Crank-Nicolson centered-advection scheme on a finite interval](../../../../../../crank-nicolson-centered-advection-scheme-on-a-finite-interval.md) is unconditionally stable:

$$
\boxed{\text{every }\mu>0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
