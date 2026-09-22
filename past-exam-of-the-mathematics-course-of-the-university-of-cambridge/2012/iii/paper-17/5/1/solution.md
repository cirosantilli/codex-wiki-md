<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Riemannian metric](../../../../../../riemannian-metric.md) gives a smooth fibrewise isomorphism $g^\flat:TM\to T^*M$, defined by $g^\flat(v)=g(v,\cdot)$. Its inverse is smooth because the inverse of a smoothly varying invertible matrix is smooth. Define the [Riemannian gradient](../../../../../../riemannian-gradient.md) by

$$
\boxed{V_\sigma=(g^\flat)^{-1}(d\sigma)=\operatorname{grad}_g\sigma.}
$$

It is a smooth [vector field](../../../../../../vector-field.md) satisfying $g(V_\sigma,Y)=d\sigma(Y)=Y(\sigma)$. Nondegeneracy also gives uniqueness. In coordinates its components are $V_\sigma^i=\sum_jg^{ij}\partial_j\sigma$.

Multiplication of $g$ by the globally defined smooth positive function $e^{2\sigma}$ gives a smooth symmetric two-tensor $\widetilde g$. For any nonzero tangent vector $v$,

$$
\widetilde g(v,v)=e^{2\sigma}g(v,v)>0.
$$

Thus **$\widetilde g=e^{2\sigma}g$ is a Riemannian metric**. This [conformal rescaling of a Riemannian metric](../../../../../../conformal-rescaling-of-a-riemannian-metric.md) changes lengths but preserves angles.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
