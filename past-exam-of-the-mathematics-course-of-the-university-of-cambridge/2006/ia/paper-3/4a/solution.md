<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Use [suffix notation](../../../../../einstein-notation.md), summing repeated indices, and write $\partial_i=\partial/\partial x_i$. For a twice continuously differentiable [vector field](../../../../../vector-field.md), mixed derivatives commute. Thus the [divergence](../../../../../divergence.md) of its [curl](../../../../../curl.md) satisfies

$$
\partial_i(\epsilon_{ijk}\partial_jv_k)
=\epsilon_{ijk}\partial_i\partial_jv_k=0,
$$

because the derivatives are symmetric in $i,j$, while the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is antisymmetric in those indices. Hence

$$
\boxed{\nabla\cdot(\nabla\times\mathbf v)=0}.
$$

For the second identity, use the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md):

$$
\begin{aligned}
[\mathbf v\times(\nabla\times\mathbf v)]_i
&=\epsilon_{ijk}v_j\epsilon_{klm}\partial_lv_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})v_j\partial_lv_m\\
&=v_j\partial_iv_j-v_j\partial_jv_i\\
&=\partial_i\left(\tfrac12v_jv_j\right)-[(\mathbf v\cdot\nabla)\mathbf v]_i.
\end{aligned}
$$

Rearranging each component proves the [vorticity cross-product identity](../../../../../vorticity-cross-product-identity.md)

$$
\boxed{(\mathbf v\cdot\nabla)\mathbf v=
\nabla\left(\tfrac12|\mathbf v|^2\right)-\mathbf v\times(\nabla\times\mathbf v)}.
$$

The second identity needs first derivatives; the first additionally uses equality of the mixed second derivatives.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
