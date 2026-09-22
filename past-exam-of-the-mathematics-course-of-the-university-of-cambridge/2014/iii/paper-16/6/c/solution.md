<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a [Riemannian metric](../../../../../../riemannian-metric.md) $h$ on $\Sigma$ compatible with its [complex structure](../../../../../../complex-structure.md) $j$, and use $g_J=\omega(\cdot,J\cdot)$ on the target. The [Dirichlet energy of a map](../../../../../../dirichlet-energy-of-a-map.md) is

$$
E(u)=\frac12\int_\Sigma|du|_{h,g_J}^2\,d\operatorname{vol}_h.
$$

It is independent of the particular conformal representative $h$: rescaling $h$ multiplies the squared differential norm by the inverse factor and the area element by the same factor. For a [J-holomorphic curve](../../../../../../pseudoholomorphic-curve.md), the [Energy identity for a J-holomorphic curve](../../../../../../energy-identity-for-a-j-holomorphic-curve.md) is

$$
\boxed{E(u)=\int_\Sigma u^*\omega.}
$$

To prove it, take an oriented $h$-orthonormal frame $e_1,e_2=je_1$ and put $a=du(e_1)$, $b=du(e_2)$. The [J-holomorphic curve](../../../../../../pseudoholomorphic-curve.md) equation says $b=Ja$. The pointwise energy density is therefore $\frac12(|a|_{g_J}^2+|Ja|_{g_J}^2)=|a|_{g_J}^2$, while the pulled-back area density is $\omega(a,Ja)=|a|_{g_J}^2$. Integrating proves the identity.

More generally, the same frame gives

$$
\frac12(|a|^2+|b|^2)-\omega(a,b)=\frac12|b-Ja|^2.
$$

With the full tensor [norm](../../../../../../norm.md) of $\bar\partial_Ju$, its two frame components are $(a+Jb)/2$ and $(b-Ja)/2$, so their squared norms sum to $\frac12|b-Ja|^2$. Hence the full identity is

$$
E(u)=\int_\Sigma u^*\omega+\int_\Sigma|\bar\partial_Ju|^2\,d\operatorname{vol}_h.
$$

This also fixes the normalization of the error term. **The energy is nonnegative and vanishes exactly when $du=0$.** The formulas apply whenever the relevant integrals are defined, in particular on compact source surfaces.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
