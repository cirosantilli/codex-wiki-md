<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [compact H-hull](../../../../../../compact-h-hull.md) is a bounded relatively closed set $K\subset\mathbb H$ whose complement $D=\mathbb H\setminus K$ is a [simply connected domain](../../../../../../simply-connected-domain.md). Equivalently one can retain its compact closure in $\overline{\mathbb H}$; real [boundary](../../../../../../boundary-of-a-set.md) points do not affect the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md). The [Riemann mapping theorem](../../../../../../riemann-mapping-theorem.md) and [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md) near infinity give a unique [conformal map](../../../../../../conformal-map.md) $g_K:D\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md). Its [Laurent series](../../../../../../laurent-series.md) is

$$
g_K(z)=z+\frac{a_K}{z}+O(|z|^{-2}),\qquad a_K\in\mathbb R.
$$

The [half-plane capacity](../../../../../../half-plane-capacity.md) is **$\operatorname{hcap}(K)=a_K$**. The missing constant term is part of the normalization, not a choice to be made again when comparing different hulls.

Here are the [conformal map](../../../../../../conformal-map.md) facts we use to justify positivity and comparison. The inverse $f_K:\mathbb H\to D\subset\mathbb H$ has expansion $f_K(w)=w-a_K/w+O(w^{-2})$. The upper-half-plane [Schwarz-Pick theorem](../../../../../../schwarz-pick-theorem.md), applied to $w$ and $iY$ and then letting $Y\to\infty$, implies $\operatorname{Im}f_K(w)\geq\operatorname{Im}w$. Indeed the inequality between pseudohyperbolic distances gives

$$
\frac{4\operatorname{Im}f_K(w)\operatorname{Im}f_K(iY)}{|f_K(w)-\overline{f_K(iY)}|^2}
\geq\frac{4Y\operatorname{Im}w}{|w+iY|^2},
$$

and multiplying by $Y$ gives the height comparison in the limit. At $w=iY$, the inverse expansion reads $\operatorname{Im}f_K(iY)=Y+a_K/Y+O(Y^{-2})$, so $a_K\geq0$.

For $r>0$, uniqueness of the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) gives

$$
g_{rK}(z)=r g_K(z/r)
=z+\frac{r^2a_K}{z}+O(z^{-2}).
$$

Consequently

$$
\boxed{\operatorname{hcap}(rK)=r^2\operatorname{hcap}(K).}
$$

Translation by a real number $b$ similarly gives $g_{K+b}(z)=b+g_K(z-b)$ and leaves [half-plane capacity](../../../../../../half-plane-capacity.md) unchanged.

If $K\subset A$ are [compact H-hulls](../../../../../../compact-h-hull.md), their [mapping-out functions](../../../../../../mapping-out-function-of-a-compact-h-hull.md) compose as $g_A=g_L\circ g_K$, where $L$ is the filled image of $A\setminus K$. Comparing [Laurent series](../../../../../../laurent-series.md) yields

$$
\operatorname{hcap}(A)=\operatorname{hcap}(K)+\operatorname{hcap}(L)\geq\operatorname{hcap}(K).
$$

This proves [monotonicity of half-plane capacity](../../../../../../monotonicity-of-half-plane-capacity.md), rather than assuming it from inclusion alone. The filled half-disc $A=\{z\in\mathbb H:|z-b|\leq R\}$ has [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md)

$$
g_A(z)=z+\frac{R^2}{z-b},
$$

which takes its semicircular [boundary](../../../../../../boundary-of-a-set.md) to the real line and is a [conformal bijection](../../../../../../biholomorphism.md) onto $\mathbb H$. Thus its [half-plane capacity](../../../../../../half-plane-capacity.md) is $R^2$. Enclose $K$ in such a half-disc, compare capacities, and minimize over real centres and radii. This proves the sharp bound

$$
\boxed{\operatorname{hcap}(K)\leq\operatorname{rad}(K)^2.}
$$

If one defines the radius by an infimum, take $R$ strictly larger than that infimum and then let $R$ decrease; no attainment assumption is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
