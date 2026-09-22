<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $c_n$ count $n$-step [self-avoiding walks](../../../../../../self-avoiding-walk.md) on the [square lattice](../../../../../../square-lattice.md) from one fixed [graph vertex](../../../../../../vertex-graph-theory.md). Splitting a [self-avoiding walk](../../../../../../self-avoiding-walk.md) after $m$ steps and dropping the avoidance constraint on its suffix gives $c_{m+n}\leq c_mc_n$. The [Fekete lemma](../../../../../../fekete-s-lemma.md) therefore gives the [connective constant](../../../../../../connective-constant.md) $\mu=\lim c_n^{1/n}$. The [planar dual graph](../../../../../../planar-dual-graph.md) of the [square lattice](../../../../../../square-lattice.md) is a translated copy of it, so its [connective constant](../../../../../../connective-constant.md) is also $\mu$.

Put $q=1-p$ and assume $q\mu<1$. Choose $a>\mu$ with $qa<1$. The definition of the [connective constant](../../../../../../connective-constant.md) provides a finite $K$ such that $c_j\leq Ka^j$ for every $j\geq0$. A simple dual [graph cycle](../../../../../../cycle-in-a-graph.md) of length $\ell$ surrounding $0$ has a [graph vertex](../../../../../../vertex-graph-theory.md) in a box of radius $\ell+1$: its diameter is at most $\ell$, and its coordinate ranges straddle the origin. Choose such a [graph vertex](../../../../../../vertex-graph-theory.md) as the starting point, orient the [graph cycle](../../../../../../cycle-in-a-graph.md), and omit its closing [edge](../../../../../../edge-of-a-graph.md). The remaining [self-avoiding walk](../../../../../../self-avoiding-walk.md) has length $\ell-1$. Consequently the number $N_\ell$ of these [graph cycles](../../../../../../cycle-in-a-graph.md) obeys

$$
N_\ell\leq K_0\ell^2 c_{\ell-1}\leq K_1\ell^2a^{\ell-1}
$$

for fixed finite constants. A specified [graph cycle](../../../../../../cycle-in-a-graph.md) is open in [dual bond percolation](../../../../../../dual-bond-percolation.md), equivalently all its crossed primal [edges](../../../../../../edge-of-a-graph.md) are closed, with [probability](../../../../../../probability.md) $q^\ell$. Hence

$$
\sum_{\ell\geq L}N_\ell q^\ell\longrightarrow0\quad\text{as }L\to\infty.
$$

To make this tail argument valid for every $q\mu<1$, rather than only extremely small $q$, use a [finite modification of Bernoulli percolation](../../../../../../finite-modification-of-bernoulli-percolation.md). Condition all primal [edges](../../../../../../edge-of-a-graph.md) within $\Lambda_N$ to be open. This event has positive [probability](../../../../../../probability.md) for $p>0$. If the resulting [percolation cluster](../../../../../../percolation-cluster.md) of $0$ is finite, its outer boundary contains a simple closed dual [graph cycle](../../../../../../cycle-in-a-graph.md) surrounding the whole box. Such a [graph cycle](../../../../../../cycle-in-a-graph.md) has length tending to infinity with $N$ and crosses no forced-open [edge](../../../../../../edge-of-a-graph.md). Under the conditioning its remaining [edge](../../../../../../edge-of-a-graph.md) states retain the original independent law, so its [probability](../../../../../../probability.md) is still $q^\ell$. Choose $N$ so that the above tail is less than $1/2$. The conditional [probability](../../../../../../probability.md) that $0$ belongs to an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) is then at least $1/2$, and thus $\theta(p)>0$.

This [connective-constant Peierls bound](../../../../../../connective-constant-peierls-bound.md) proves that every $p>1-\mu^{-1}$ is above or at the onset of positive [percolation probability](../../../../../../percolation-probability.md). Taking the infimum gives

$$
\boxed{p_c\leq1-\mu^{-1}}.
$$

The case $p=1$ is immediate. This proof uses the [Peierls argument](../../../../../../peierls-argument.md), without assuming the exact [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
