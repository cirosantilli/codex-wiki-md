<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in a [Cartesian coordinate system](../../../../../cartesian-coordinate-system.md), write $\partial_j=\partial/\partial x_j$, and use the [Einstein summation convention](../../../../../einstein-notation.md). For a twice continuously differentiable [vector field](../../../../../vector-field.md), the contraction of two [Levi-Civita symbols](../../../../../levi-civita-symbol.md) gives

$$
\begin{aligned}
[\nabla\times(\nabla\times u)]_i&=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lu_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j\partial_lu_m\\
&=\partial_i(\partial_ju_j)-\partial_j\partial_ju_i.
\end{aligned}
$$

Here the [Kronecker deltas](../../../../../kronecker-delta.md) select components, and equality of mixed [partial derivatives](../../../../../partial-derivative.md) gives the [curl of the curl identity](../../../../../curl-of-the-curl-identity.md)

$$
\boxed{\nabla\times(\nabla\times u)=\nabla(\nabla\cdot u)-\nabla^2u.}
$$

For the second identity, the same contraction followed by the [product rule](../../../../../product-rule.md) yields

$$
\begin{aligned}
[\nabla\times(u\times v)]_i&=\partial_j(u_iv_j-u_jv_i)\\
&=u_i\partial_jv_j-v_i\partial_ju_j+v_j\partial_ju_i-u_j\partial_jv_i.
\end{aligned}
$$

Thus the [curl of a cross product](../../../../../curl-of-a-cross-product.md) is

$$
\boxed{\nabla\times(u\times v)=u(\nabla\cdot v)-v(\nabla\cdot u)+(v\cdot\nabla)u-(u\cdot\nabla)v.}
$$

The directional [derivatives](../../../../../derivative.md) in the last two terms act on the [vector field](../../../../../vector-field.md) immediately to their right.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
