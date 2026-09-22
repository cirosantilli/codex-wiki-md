<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The trial space must be a subspace of $H_0^1(0,1)$, not merely of $L^2(0,1)$.** The printed assumptions on the basis do not ensure square-integrable weak derivatives, and boundary traces are not defined for arbitrary [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) functions. For example, $\varphi(x)=x^{1/4}(1-x)$ is continuous, vanishes at both endpoints and belongs to $L^2$, but $|\varphi'(x)|^2\sim x^{-3/2}/16$ is not integrable at zero. Assume the basis belongs to the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md), as it does for the hat functions in part (c).

Write $u_H=\sum_{j=1}^M c_j\varphi_j$. Differentiating the restricted energy with respect to $c_i$, or imposing the [Galerkin method](../../../../../../galerkin-method.md) with test function $\varphi_i$, gives

$$
\boxed{\sum_{j=1}^M A_{ij}c_j=F_i,\qquad
A_{ij}=\int_0^1(\varphi_j'\varphi_i'+\varphi_j\varphi_i)\,dx,\qquad
F_i=\int_0^1x\varphi_i\,dx.}
$$

The derivative term is the usual diffusion [stiffness matrix](../../../../../../stiffness-matrix.md) and the second is the [mass matrix](../../../../../../mass-matrix.md). The full matrix is real symmetric, and for every nonzero coefficient vector $c$,

$$
c^TAc=\int_0^1\left[\left(\sum_jc_j\varphi_j'\right)^2
+\left(\sum_jc_j\varphi_j\right)^2\right]dx>0,
$$

because a basis is [linearly independent](../../../../../../linear-independence.md). Thus it is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), so the restricted [Ritz method](../../../../../../rayleigh-ritz-method.md) has a unique solution and minimum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
