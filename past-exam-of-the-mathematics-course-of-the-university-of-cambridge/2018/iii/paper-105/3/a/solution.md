<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) $H_0^1(U)$, the associated [bilinear form](../../../../../../bilinear-form.md) is

$$
\boxed{B[u,v]=\int_U\left(\sum_{i,j}a^{ij}u_{x_i}v_{x_j}
+\sum_i b^iu_{x_i}v+cuv\right)dx.}
$$

The homogeneous [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) removes the boundary term, so $(Lu,v)_{L^2}=B[u,v]$ for sufficiently regular $u$ and $v\in H_0^1$.

Formal self-adjointness means that $L$ equals its [formal adjoint](../../../../../../formal-adjoint.md), or equivalently $(L\phi,\chi)=(\phi,L\chi)$ for compactly supported smooth functions. Here

$$
L^*v=-\sum_{i,j}(a^{ij}v_{x_i})_{x_j}
-\sum_i b^iv_{x_i}+(c-\operatorname{div}b)v.
$$

With the symmetric real principal coefficients in the question, $L=L^*$ is equivalent to $b=0$. It makes $B$ a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md).

For the assertions in part (b), positivity must mean strict Dirichlet positivity:

$$
\boxed{B[u,u]>0\quad\text{for every nonzero }u\in H_0^1(U).}
$$

This is the [positive-definite operator](../../../../../../positive-definite-operator.md) convention. The weaker [positive semidefinite operator](../../../../../../positive-operator.md) convention $B[u,u]\geq0$ does not suffice: $L=-\Delta-\lambda_1$ has zero energy on a first Dirichlet [eigenfunction](../../../../../../eigenfunction.md). Under strict positivity, the compactness argument in part (b)(i) gives a uniform lower bound as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
