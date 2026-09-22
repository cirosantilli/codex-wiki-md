<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

In [Einstein summation convention](../../../../../einstein-notation.md), the [curl](../../../../../curl.md) of a [cross product](../../../../../cross-product.md) has components

$$
\begin{aligned}
[\nabla\times(a\times b)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{k\ell m}a_\ell b_m)\\
&=\partial_j(a_i b_j-a_j b_i)\\
&=a_i\partial_jb_j-b_i\partial_ja_j+b_j\partial_ja_i-a_j\partial_jb_i.
\end{aligned}
$$

The second line uses the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md); the last uses the [product rule](../../../../../product-rule.md). These components prove the [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity, including both [divergence](../../../../../divergence.md) and directional-derivative terms.

Now apply that identity to $m\times v$. On the [orientable surface](../../../../../orientable-surface.md), $m=n$, $m\cdot v=0$, and $|m|=1$. Differentiating $m\cdot m=1$ gives $m_i\partial_jm_i=0$. Taking a [dot product](../../../../../dot-product.md) with $m$ in the [curl of a cross product](../../../../../curl-of-a-cross-product.md) formula therefore gives, on $S$,

$$
\begin{aligned}
n\cdot\nabla\times(m\times v)
&=\nabla\cdot v-(m\cdot v)\nabla\cdot m
+m_i v_j\partial_jm_i-m_i m_j\partial_jv_i\\
&=(\delta_{ij}-n_in_j)\partial_jv_i.
\end{aligned}
$$

Only tangency on the surface is needed; no claim is made that the extension $v$ is tangent away from it. The right side is the [surface divergence](../../../../../surface-divergence.md) of the tangent [vector field](../../../../../vector-field.md).

With the boundary oriented according to [Stokes theorem](../../../../../stokes-theorem.md), cyclic invariance of the [scalar triple product](../../../../../scalar-triple-product.md) gives

$$
(m\times v)\cdot d\mathbf r=v\cdot(d\mathbf r\times n)=v\cdot u\,ds,
$$

where $u$ is the [outward conormal of a surface boundary](../../../../../outward-conormal-of-a-surface-boundary.md). Thus [Stokes theorem](../../../../../stokes-theorem.md) proves

$$
\boxed{\int_S(\delta_{ij}-n_in_j)\partial_jv_i\,dS
=\oint_C u\cdot v\,ds.}
$$

This is the [surface divergence theorem for a tangent field](../../../../../surface-divergence-theorem-for-a-tangent-field.md).

For the disc in the $z=0$ plane, take $n=(0,0,1)$ and $v=\mathbf r=(x,y,z)$. The field is tangent on the disc, and $\partial_jv_i=\delta_{ij}$. The contraction is $3-|n|^2=2$, so the [surface integral](../../../../../surface-integral.md) is $2\pi R^2$. On the positively oriented circular boundary, $u=(\cos\theta,\sin\theta,0)$ and $v=Ru$, so the boundary [flux](../../../../../flux.md) is $R(2\pi R)=2\pi R^2$. **Both sides agree.**

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
