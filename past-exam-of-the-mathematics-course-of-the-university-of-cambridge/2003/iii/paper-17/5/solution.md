<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [compatible almost complex structure](../../../../../compatible-almost-complex-structure.md) is a smooth endomorphism $J:TX\to TX$ satisfying $J^2=-I$, preserving $\omega$, and making $g_J(u,v)=\omega(u,Jv)$ a positive-definite [inner product](../../../../../inner-product.md). Preservation and $J^2=-I$ make this [bilinear form](../../../../../bilinear-form.md) symmetric.

To construct one, choose any [Riemannian metric](../../../../../riemannian-metric.md) $h$ and define $A$ by $h(Au,v)=\omega(u,v)$. The endomorphism $A$ is skew-adjoint and invertible. Consequently $-A^2$ is positive definite and self-adjoint. Let $B=(-A^2)^{1/2}$ be its positive square root and set

$$
\boxed{J=B^{-1}A.}
$$

The [spectral theorem](../../../../../spectral-theorem.md) gives $B$ fibrewise, and the positive-square-root operation is smooth on positive-definite matrices, so this defines a smooth endomorphism. Since $A$ commutes with $B$, $J^2=-I$. Also $J^*=-J$, so $J^*J=I$. Commutation then gives

$$
\omega(Ju,Jv)=h(AJu,Jv)=h(Au,v)=\omega(u,v),\qquad
\omega(u,Ju)=h(Bu,u)>0\quad(u\ne0).
$$

This is the [metric construction of a compatible almost complex structure](../../../../../metric-construction-of-a-compatible-almost-complex-structure.md), proving nonemptiness.

If we start with $h=g_J$ for an already compatible $J$, then $h(Ju,v)=\omega(u,v)$, so $A=J$, $B=I$, and the construction recovers $J$. For two compatible structures, linearly interpolate their metrics,

$$
h_t=(1-t)g_{J_0}+t g_{J_1},\qquad0\leq t\leq1,
$$

and apply the construction to $h_t$. This is a continuous smooth-in-$t$ path with endpoints $J_0,J_1$. Thus **the space is nonempty and path connected**. Interpolating instead to a single fixed auxiliary metric actually gives the [contractibility of compatible almost complex structures](../../../../../contractibility-of-compatible-almost-complex-structures.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
