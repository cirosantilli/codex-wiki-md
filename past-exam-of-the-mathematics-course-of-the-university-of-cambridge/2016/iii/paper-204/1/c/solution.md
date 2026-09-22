<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use integer [graph vertices](../../../../../../vertex-graph-theory.md) in the boxes: $\Lambda_n=[-n,n]^2\cap\mathbb Z^2$, and set $\Lambda_{-1}=\varnothing$. Thus $\partial\Lambda_0=\{0\}$, $g_0=1$, and $|\partial\Lambda_m|=8m$ for $m\geq1$.

If $0\leftrightarrow\partial\Lambda_{m+n}$, erase loops from an open [graph path](../../../../../../path-in-a-graph.md) to obtain a [self-avoiding walk](../../../../../../self-avoiding-walk.md). Let $x$ be its first [graph vertex](../../../../../../vertex-graph-theory.md) on $\partial\Lambda_m$. Split at $x$. The prefix certifies $A_x=\{0\leftrightarrow x\}$, while a segment of the suffix certifies $B_x=\{x\leftrightarrow x+\partial\Lambda_n\}$: the final [graph vertex](../../../../../../vertex-graph-theory.md) is at [supremum norm](../../../../../../supremum-norm.md) distance at least $n$ from $x$, so the suffix first hits that translated boundary. The two certificates use disjoint [edges](../../../../../../edge-of-a-graph.md). Therefore the [BK boundary-splitting estimate](../../../../../../bk-boundary-splitting-estimate.md), the [union bound](../../../../../../boole-s-inequality.md), the [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md), and translation invariance give

$$
\begin{aligned}
g_{m+n}&\leq\sum_{x\in\partial\Lambda_m}\mathbb P_p(A_x\mathbin\square B_x)\\
&\leq\sum_{x\in\partial\Lambda_m}\mathbb P_p(A_x)\mathbb P_p(B_x)\\
&\leq|\partial\Lambda_m|g_mg_n.
\end{aligned}
$$

The cases $m=0$ or $n=0$ follow directly from $g_0=1$, so this proves the bound including the endpoints.

Here is an explicit way to remove the polynomial boundary factor. For $p>0$ put $b_n=32n^2g_n$, $n\geq1$. By symmetry in $m,n$, assume $m\leq n$. Then

$$
\frac{b_{m+n}}{b_mb_n}\leq\frac{(m+n)^2}{4mn^2}\leq\frac1m\leq1.
$$

Consequently $a_n=\log b_n$ is a [subadditive sequence](../../../../../../subadditive-sequence.md). The [Fekete lemma](../../../../../../fekete-s-lemma.md) states that any real [subadditive sequence](../../../../../../subadditive-sequence.md) satisfies $\lim a_n/n=\inf_{n\geq1}a_n/n$, possibly $-\infty$. In this case the direct horizontal open [graph path](../../../../../../path-in-a-graph.md) gives $g_n\geq p^n$, so this [limit of a sequence](../../../../../../limit-of-a-sequence.md) is bounded below by $\log p$. Since $g_n\leq1$, its upper bound is zero. Finally,

$$
\frac{\log g_n}{n}=\frac{a_n}{n}-\frac{\log(32n^2)}n
$$

has the same [limit of a sequence](../../../../../../limit-of-a-sequence.md). Thus the [percolation one-arm decay rate](../../../../../../percolation-one-arm-decay-rate.md) exists and

$$
\boxed{\gamma=\lim_{n\to\infty}g_n^{1/n}\in[p,1]}.
$$

For $p=0$, every $g_n$ with $n\geq1$ is zero and $\gamma=0$. No exponential-decay theorem or assumption that $p$ is below the [percolation critical probability](../../../../../../percolation-critical-probability.md) is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
