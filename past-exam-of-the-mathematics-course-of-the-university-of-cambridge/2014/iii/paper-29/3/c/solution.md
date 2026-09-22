<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f=g_K^{-1}$. The reflection at infinity used in part (a) gives analytic expansions there for both inverse maps. In particular,

$$
f(w)=w-\frac{a_K}{w}+O(w^{-2}),
$$

uniformly for large $w\in\mathbb H$, including approach close to the real axis.

Fix $R<\infty$. If $g_K$ were unbounded on $D\cap\{|z|\leq R\}$, there would be points $z_n$ there with $w_n=g_K(z_n)$ tending to infinity in modulus. The inverse expansion would imply $z_n=f(w_n)=w_n+O(1/w_n)$, contradicting boundedness of $z_n$. Thus **$g_K$ is bounded on every bounded portion of its domain**, including points arbitrarily near a rough hull boundary. This is the [inverse-at-infinity criterion for local boundedness of a mapping-out function](../../../../../../inverse-at-infinity-criterion-for-local-boundedness-of-a-mapping-out-function.md).

On the region $|z|>R$ for sufficiently large $R$, the expansion of $g_K$ gives $g_K(z)-z=O(1/z)$. On the remaining bounded region, the preceding bound for $g_K$ and the bound for $z$ give a finite bound for their difference. Therefore

$$
\boxed{\sup_{z\in D}|g_K(z)-z|<\infty.}
$$

The argument uses reflection near infinity only. It does not assume that the real part of the map extends continuously at every point of an arbitrary hull; the [sharp displacement bound for a compact H-hull](../../../../../../sharp-displacement-bound-for-a-compact-h-hull.md) is a further quantitative version of this boundedness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
