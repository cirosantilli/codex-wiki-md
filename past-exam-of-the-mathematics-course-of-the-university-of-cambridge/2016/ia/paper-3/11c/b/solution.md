<h1 id="11c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [Einstein summation convention](../../../../../../einstein-notation.md), the [curl](../../../../../../curl.md) is

$$
(\nabla\times\mathbf V)_i=\epsilon_{ijk}\partial_jV_k.
$$

Apply another [curl](../../../../../../curl.md) and use the [contraction of two Levi-Civita symbols](../../../../../../contraction-of-two-levi-civita-symbols.md):

$$
\begin{aligned}(\nabla\times(\nabla\times\mathbf V))_i&=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lV_m\\&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j\partial_lV_m\\&=\partial_i(\partial_jV_j)-\partial_j\partial_jV_i.\end{aligned}
$$

Smoothness allows the [partial derivatives](../../../../../../partial-derivative.md) to commute. **This proves the [curl of the curl identity](../../../../../../curl-of-the-curl-identity.md):**

$$
\boxed{\nabla\times(\nabla\times\mathbf V)=\nabla(\nabla\cdot\mathbf V)-\nabla^2\mathbf V.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
