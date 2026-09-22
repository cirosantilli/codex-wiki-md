<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Let $e=\tfrac12(|A|^2+|B|^2)$. The time equations and the [dot product](../../../../../dot-product.md) [differentiation](../../../../../differentiation.md) rule give the local identity

$$
\partial_t e=A\cdot(\nabla\times B)-B\cdot(\nabla\times A).
$$

The [divergence of a cross product](../../../../../divergence-of-a-cross-product.md) is

$$
\nabla\cdot(A\times B)=B\cdot(\nabla\times A)-A\cdot(\nabla\times B).
$$

Combining them yields $\partial_t e+\nabla\cdot(A\times B)=0$. On a fixed bounded region with a [boundary](../../../../../boundary-of-a-set.md) regular enough for the [divergence theorem](../../../../../divergence-theorem.md), differentiating under the [integral](../../../../../integral.md) and applying that theorem gives

$$
\boxed{\frac d{dt}\left[\frac12\int_V(|A|^2+|B|^2)\,dV\right]
=-\int_{\partial V}(A\times B)\cdot n\,dS.}
$$

Here $n$ is the outward [unit normal](../../../../../unit-normal.md), so the sign expresses loss of the interior quadratic quantity by outward flux. No vanishing-boundary assumption is required.

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
