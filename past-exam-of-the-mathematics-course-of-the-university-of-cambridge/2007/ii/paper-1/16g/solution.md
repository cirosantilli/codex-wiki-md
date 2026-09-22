<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A [complete lattice](../../../../../complete-lattice.md) has every [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md), hence every directed and finite join. Conversely, if a [partially ordered set](../../../../../partially-ordered-set.md) is [directed-complete](../../../../../directed-complete-partial-order.md) and has finite joins including the empty join, then for any subset $A$ the set of joins of its finite subsets is nonempty and [directed](../../../../../directed-set.md). Its [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) is $\bigvee A$. Including the empty join supplies a bottom element and handles $A=\varnothing$.

For a [directed set](../../../../../directed-set.md) of [partial functions](../../../../../partial-function.md) from $A$ to $B$, their union is a function: any two functions have a common extension, so they agree wherever their domains overlap. This union is exactly their [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) in the extension order, proving directed completeness.

Write $C_x$ for the intersection of all sets containing $x$ and closed under $f$ and directed joins. Then $x\mathrel R y$ means $y\in C_x$. Reflexivity is immediate, and transitivity follows because any closed set containing $x$ must contain $y$ and then every $z$ with $y\mathrel R z$. The upper set $[x,\infty)$ is closed: $f$ is [inflationary](../../../../../inflationary-map.md), and a directed join of elements above $x$ is above $x$. Thus $x\mathrel R y$ implies $x\le y$, proving antisymmetry.

If $h,k\in H$, then $x\mathrel R k(x)\mathrel R h(k(x))$, so $h\circ k\in H$. Moreover $h(k(x))\ge h(x)$ by [monotonicity](../../../../../monotonic-function.md), and $h(k(x))\ge k(x)$ by inflationarity. This proves that $H x$ is [directed](../../../../../directed-set.md). Define $h_0(x)=\bigvee H x$. Pointwise monotonicity of every $h$ implies monotonicity of $h_0$. Since $H x\subseteq C_x$ and $C_x$ is closed under directed joins, $x\mathrel R h_0(x)$; hence $h_0\in H$.

The original map $f$ belongs to $H$ by the definition of closedness, so $f\circ h_0\in H$ and $f(h_0(x))\le h_0(x)$ by the definition of the join. Inflationarity gives the reverse inequality. Finally, if $p=f(p)$ and $p\ge x$, the lower set $(-\infty,p]$ is closed by monotonicity of $f$ and the join property. Thus every $h(x)$ is at most $p$, and so is $h_0(x)$. This proves the [least fixed point from a directed family of maps](../../../../../least-fixed-point-from-a-directed-family-of-maps.md): $h_0(x)$ is the least [fixed point](../../../../../fixed-point.md) above $x$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
