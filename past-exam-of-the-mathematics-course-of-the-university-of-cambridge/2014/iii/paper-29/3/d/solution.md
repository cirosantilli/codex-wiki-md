<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $v(z)=\operatorname{Im}g_K(z)$, a positive [harmonic function](../../../../../../harmonic-function.md) on $D$. First justify its boundary behavior. For $z_n\to p\in\partial D$ with $p$ finite, part (c) makes $g_K(z_n)$ bounded. Any subsequential limit $w$ lies in $\overline{\mathbb H}$. If $\operatorname{Im}w>0$, continuity of the inverse inside $\mathbb H$ would give $p=g_K^{-1}(w)\in D$, a contradiction. Thus

$$
v(z)\longrightarrow0\quad\text{as }z\to p\in\partial D.
$$

This [boundary degeneration under a mapping-out function](../../../../../../boundary-degeneration-under-a-mapping-out-function.md) is valid without a smooth or locally connected hull boundary.

The [harmonic function](../../../../../../harmonic-function.md) $u(z)=v(z)-\operatorname{Im}z$ consequently has nonpositive finite-boundary values. Its value tends uniformly to zero at infinity, by the [Laurent series](../../../../../../laurent-series.md). On the bounded domain $D\cap\{|z|<R\}$, the [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) bounds $u$ by $\max(0,\varepsilon_R)$, where $\varepsilon_R=\sup_{D\cap\{|z|=R\}}|g_K(z)-z|\to0$. Let $R\to\infty$ with $z$ fixed. We obtain

$$
\boxed{\operatorname{Im}g_K(z)\leq\operatorname{Im}z.}
$$

This is the [height contraction of a hydrodynamically normalized mapping-out function](../../../../../../height-contraction-of-a-hydrodynamically-normalized-mapping-out-function.md). The exhaustion controls infinity explicitly, which is necessary when using a maximum principle on an unbounded domain.

## ↑ Ancestors (11)

1. [D](../d.md)
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
