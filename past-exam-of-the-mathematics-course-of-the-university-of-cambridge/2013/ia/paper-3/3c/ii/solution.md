<h1 id="3c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [arc length](../../../../../../arc-length.md) coordinate oriented in the direction of increasing $t$: $s(t)=\int_0^t2e^\tau\,d\tau=2(e^t-1)$, with $s>-2$. Also $\mathbf r''=e^t(\sqrt2,-2\cos t,-2\sin t)$, giving $|\mathbf r''|^2=6e^{2t}$ and $\mathbf r'\cdot\mathbf r''=4e^{2t}$. The [Lagrange identity for the cross product](../../../../../../lagrange-identity-for-the-cross-product.md) yields

$$
|\mathbf r'\times\mathbf r''|^2=|\mathbf r'|^2|\mathbf r''|^2-(\mathbf r'\cdot\mathbf r'')^2=8e^{4t}.
$$

The [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md) is therefore

$$
\boxed{\kappa(t)=\frac{|\mathbf r'\times\mathbf r''|}{|\mathbf r'|^3}
=\frac{e^{-t}}{2\sqrt2},\qquad
\kappa(s)=\frac1{\sqrt2(s+2)}.}
$$

For the forward portion $t\ge0$, this has ordinary nonnegative [arc length](../../../../../../arc-length.md) $s\ge0$. If instead nonnegative distance is measured backwards from $t=0$, put $s_b=2(1-e^t)$ for $t\le0$; that branch has $\kappa=1/[\sqrt2(2-s_b)]$, $0\le s_b<2$. Choosing orientation avoids confusing the two points at the same unoriented distance.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3C](../../3c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
