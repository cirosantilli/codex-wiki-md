<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the curvature sign convention implicit in part (c): the [Jacobi field](../../../../../../jacobi-field.md) equation is $D_t^2J+K_{\dot\gamma}J=0$, so the operator in a positively curved normal direction has positive [eigenvalue](../../../../../../eigenvalue.md). With the alternative convention $R_{\mathrm{std}}(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ used for the catalog's [Jacobi curvature operator](../../../../../../jacobi-curvature-operator.md), the paper's tensor is $R=-R_{\mathrm{std}}$, and its operator is $K_v(x)=R_{\mathrm{std}}(x,v)v$. This fixes the sign throughout Q1.

Let $r(A,B,C,D)=\langle R(A,B)C,D\rangle$. Pair interchange for the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) gives

$$
\langle K_vx,y\rangle=r(v,x,v,y)=r(v,y,v,x)=\langle x,K_vy\rangle.
$$

Thus **$K_v$ is [self-adjoint](../../../../../../self-adjoint-operator.md)** with respect to the [Riemannian metric](../../../../../../riemannian-metric.md). The curvature sign does not affect this conclusion. The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) therefore supplies the real orthonormal [eigenbasis](../../../../../../eigenbasis.md) used in part (b). Also $K_vv=0$, so the tangent direction is a zero-eigenvalue direction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
