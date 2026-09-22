<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the vertical slit, choose the branch of $\sqrt{z^2+1}$ asymptotic to $z$ at infinity. It is the [mapping-out function of a compact H-hull](../../../../../../mapping-out-function-of-a-compact-h-hull.md) for $(0,i]$, and

$$
\sqrt{z^2+1}=z+\frac1{2z}+O(z^{-3}).
$$

Thus [half-plane capacity of a vertical slit](../../../../../../half-plane-capacity-of-a-vertical-slit.md) gives

$$
\boxed{\operatorname{hcap}([0,i])=\frac12.}
$$

The endpoint $0$ is merely part of the [boundary](../../../../../../boundary-of-a-set.md) [closure](../../../../../../closure-topology.md) convention.

For the filled upper half-disc $K=\{z\in\mathbb H:|z|\leq1\}$, the [conformal map](../../../../../../conformal-map.md) $g_K(z)=z+1/z$ maps the exterior half-disc onto $\mathbb H$. Indeed, it sends the semicircle to $[-2,2]$, the remaining real [boundary](../../../../../../boundary-of-a-set.md) to the complementary intervals, and its inverse is the branch of $(w+\sqrt{w^2-4})/2$ asymptotic to $w$. Hence [half-plane capacity of a half-disc](../../../../../../half-plane-capacity-of-a-half-disc.md) gives

$$
\boxed{\operatorname{hcap}(K)=1.}
$$

If $\mathbb D$ denotes the open [unit disc](../../../../../../unit-disc.md), the printed $\mathbb H\cap\mathbb D$ is not relatively closed and is literally not a [compact H-hull](../../../../../../compact-h-hull.md). The intended value is the one for its filled relative [closure](../../../../../../closure-topology.md) $K$. With a closed-disc convention the displayed notation already represents that hull.

For a nonempty [compact H-hull](../../../../../../compact-h-hull.md) $A$, its [closure](../../../../../../closure-topology.md) meets $\mathbb R$: otherwise a nonempty [compact set](../../../../../../compact-space.md) strictly inside $\mathbb H$ would be separated from the lower half-plane in the complement, contradicting the [simply connected domain](../../../../../../simply-connected-domain.md) condition for $\mathbb H\setminus A$. Choose $x\in\overline A\cap\mathbb R$ and put $d=\operatorname{diam}(A)$. Taking limits in the definition of [diameter](../../../../../../diameter.md) shows $|z-x|\leq d$ for every $z\in A$. Thus $A$ lies in the filled half-disc of radius $d$ centered at $x$. Its [half-plane capacity](../../../../../../half-plane-capacity.md) is $d^2$ by [scaling and translation of half-plane capacity](../../../../../../scaling-and-translation-of-half-plane-capacity.md). Using [monotonicity of half-plane capacity](../../../../../../monotonicity-of-half-plane-capacity.md),

$$
\boxed{\operatorname{hcap}(A)\leq\operatorname{diam}(A)^2.}
$$

For the empty [compact H-hull](../../../../../../compact-h-hull.md), use [diameter](../../../../../../diameter.md) zero. This proves the unit-constant version of [half-plane capacity is bounded by squared diameter](../../../../../../half-plane-capacity-is-bounded-by-squared-diameter.md); no claim of optimality of the constant is needed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
