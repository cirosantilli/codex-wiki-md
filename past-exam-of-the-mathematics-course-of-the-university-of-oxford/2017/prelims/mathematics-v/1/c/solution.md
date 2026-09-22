<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Pair each point $\mathbf x$ of the [square](../../../../../../square.md)'s boundary with $-\mathbf x$. The [vector field](../../../../../../vector-field.md) obeys $\mathbf f(-\mathbf x)=\mathbf f(\mathbf x)$, whereas the outward [unit normal vector](../../../../../../unit-normal.md) changes sign: $\mathbf n(-\mathbf x)=-\mathbf n(\mathbf x)$. Corresponding [arc length](../../../../../../arc-length.md) elements are equal. Thus the two contributions to the [flux](../../../../../../flux.md) cancel, proving without evaluating any boundary [integral](../../../../../../integral-split.md) that

$$
\boxed{\int_C\mathbf f\cdot\mathbf n\,ds=0.}
$$

The same cancellation appears in the [divergence](../../../../../../divergence.md), which is an [odd function](../../../../../../odd-function.md) of $x$ over a region symmetric under $x\mapsto-x$. To justify using the planar [divergence theorem](../../../../../../divergence-theorem.md) despite the lack of [differentiability](../../../../../../differentiability.md) at the origin, remove a disk of radius $\varepsilon<1$. The [vector field](../../../../../../vector-field.md) is continuously differentiable on the remaining region, its [divergence](../../../../../../divergence.md) has zero [double integral](../../../../../../double-integral.md) by this symmetry, and the magnitude of the inner [flux](../../../../../../flux.md) is at most $2\pi\varepsilon^2$, since $\|\mathbf f\|\leq\varepsilon$ there. Letting $\varepsilon\to0$ recovers the result. This is [flux around a removable point singularity](../../../../../../flux-around-a-removable-point-singularity.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
