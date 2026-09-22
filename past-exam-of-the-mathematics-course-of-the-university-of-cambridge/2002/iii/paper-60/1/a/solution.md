<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h=1/(m+1)$ and impose homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), as required by the stated continuum [eigenvalues](../../../../../../eigenvalue.md). Let $T=\operatorname{tridiag}(1,-2,1)$ be the unscaled one-dimensional [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md). For $1\leq k\leq m$, the vectors $v_j^{(k)}=\sin(jk\pi h)$ satisfy

$$
Tv^{(k)}=\tau_kv^{(k)},\qquad \tau_k=2\cos(k\pi h)-2=-4\sin^2\frac{k\pi h}{2}.
$$

The identity follows by adding the two neighboring [sines](../../../../../../sine.md); the values at $j=0,m+1$ vanish. These $m$ mutually orthogonal vectors form the [discrete sine transform](../../../../../../discrete-sine-transform.md) basis. Consequently their [tensor products](../../../../../../tensor-product.md) give all $m^2$ two-dimensional modes, not merely a few candidate [eigenvectors](../../../../../../eigenvector.md).

In a compatible grid ordering the axial operator is $A_5=h^{-2}(T\otimes I+I\otimes T)$. The nine-point operator is

$$
A_9=A_5+\frac1{6h^2}T\otimes T.
$$

Indeed, the added [Kronecker product](../../../../../../kronecker-product.md) supplies the diagonal neighbors with weight $1/6$, subtracts $1/3$ from each axial neighbor and adds $2/3$ to the central coefficient. Thus it has exactly the coefficients of the second discretization. On $v^{(k)}\otimes v^{(l)}$ the [eigenvalues](../../../../../../eigenvalue.md) are

$$
\boxed{\lambda_{5,kl}=-\frac4{h^2}\left(\sin^2\frac{k\pi h}{2}+\sin^2\frac{l\pi h}{2}\right),}
$$

and

$$
\boxed{\lambda_{9,kl}=\lambda_{5,kl}+\frac8{3h^2}\sin^2\frac{k\pi h}{2}\sin^2\frac{l\pi h}{2},\qquad 1\leq k,l\leq m.}
$$

Equivalently, $h^2\lambda_{9,kl}=-10/3+4[\cos(k\pi h)+\cos(l\pi h)]/3+2\cos(k\pi h)\cos(l\pi h)/3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
