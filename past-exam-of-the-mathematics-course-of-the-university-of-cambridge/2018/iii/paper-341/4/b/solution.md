<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Arrange the interior values into a vector $U$. Represent the [five-point Dirichlet Laplacian as a Kronecker sum](../../../../../../five-point-dirichlet-laplacian-as-a-kronecker-sum.md) $L_h=h^{-2}(D\otimes I+I\otimes D)$, where $D$ is the [tridiagonal matrix](../../../../../../tridiagonal-matrix.md) with diagonal $-2$ and adjacent entries one. This [Kronecker sum](../../../../../../kronecker-sum.md) is real symmetric; the real sampled potential has a real diagonal matrix $D_V$. Thus

$$
iU'=H_hU,\qquad H_h=L_h-D_V=H_h^*.
$$

The generator $-iH_h$ is a [skew-Hermitian matrix](../../../../../../skew-hermitian-matrix.md). Consequently

$$
\frac{d}{dt}(U^*U)
=2\operatorname{Re}(-iU^*H_hU)=0,
\qquad U(t)=e^{-itH_h}U(0).
$$

The [matrix exponential](../../../../../../matrix-exponential.md) is a [unitary matrix](../../../../../../unitary-matrix.md), either by differentiating its product with its adjoint or by [unitary diagonalization of a normal matrix](../../../../../../unitary-diagonalization-of-a-normal-matrix.md). For the two-dimensional [discrete L2 norm](../../../../../../discrete-l2-norm.md) $\|U\|_h^2=h^2\sum_{m,n}|U_{m,n}|^2$, this gives

$$
\boxed{\|U(t)-\widetilde U(t)\|_h
=\|U(0)-\widetilde U(0)\|_h\quad(t\geq0).}
$$

Applying the same equation to a difference proves [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) with a mesh-independent constant one. This is [norm conservation of a semidiscrete Schrödinger equation](../../../../../../norm-conservation-of-a-semidiscrete-schrodinger-equation.md). It concerns continuous time after spatial discretization; an arbitrary subsequent time integrator need not preserve this stability.

**The printed coordinates do not discretize the stated square.** For $[-1,1]^2$ with $M$ interior points in each direction, use $h=2/(M+1)$, $x_m=-1+mh$, $y_n=-1+nh$, and sample $V$ there. The printed $h=1/(M+1)$ and unshifted coordinates instead describe a grid on $[0,1]^2$. The matrix proof is valid for either geometry with its corresponding boundary values, so this transcription-independent statement flaw does not alter the stability conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
