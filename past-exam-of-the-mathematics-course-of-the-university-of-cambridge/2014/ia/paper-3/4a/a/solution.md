<h1 id="4a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Parametrize the smooth path by $\gamma:[0,1]\to G$. The [chain rule](../../../../../../chain-rule.md) turns the [line integral](../../../../../../line-integral.md) of the [gradient](../../../../../../gradient.md) into a one-variable derivative:

$$
\int_\gamma\mathbf F\cdot d\mathbf x
=\int_0^1\nabla\phi(\gamma(t))\cdot\gamma'(t)\,dt
=\int_0^1\frac{d}{dt}\phi(\gamma(t))\,dt
=\boxed{\phi(\mathbf b)-\phi(\mathbf a)}.
$$

This is the [fundamental theorem for line integrals](../../../../../../fundamental-theorem-for-line-integrals.md); in particular the integral has [path independence](../../../../../../path-independence.md).

For a twice continuously differentiable [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md), the [curl](../../../../../../curl.md) of its [gradient](../../../../../../gradient.md) vanishes because mixed [partial derivatives](../../../../../../partial-derivative.md) commute:

$$
(\nabla\times\nabla\phi)_i=\epsilon_{ijk}\partial_j\partial_k\phi=0.
$$

**A smooth [gradient](../../../../../../gradient.md) field is necessarily [curl](../../../../../../curl.md)-free.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4A](../../4a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
