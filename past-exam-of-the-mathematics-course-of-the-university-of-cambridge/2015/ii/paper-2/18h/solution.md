<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

A [covering map](../../../../../covering-space.md) is a continuous surjection $p:\widetilde X\to X$ for which each point has an open neighbourhood $U$ with $p^{-1}(U)$ a disjoint union of open sets, each mapped homeomorphically onto $U$. A connected simply connected [covering space](../../../../../covering-space.md) is a [universal cover](../../../../../universal-cover.md).

There is a necessary connectedness qualification in the printed conclusion. Let $A_0$ be the path component of $a_0$ in $A$. Then $p(\widetilde A)=A_0$: one inclusion follows by projecting paths, and the other by lifting a path in $A_0$ from $a_0$. Thus the asserted surjection onto all of $A$ requires $A$ to be path connected. Without it, take $p$ to be the identity of $\mathbb R$ and $A$ to be two disjoint intervals; a selected component cannot cover both.

To prove the assertion about a [component of a pulled-back universal cover](../../../../../component-of-a-pulled-back-universal-cover.md), choose an evenly covered neighbourhood $U$ in $X$. Local path connectedness of $A$ supplies a path-connected relatively open neighbourhood $V\subseteq U\cap A_0$. Each inverse sheet over $V$ is path connected, so it lies wholly in $\widetilde A$ or is disjoint from it. These sheets evenly cover $V$ under $p|_{\widetilde A}$. Therefore **$p|_{\widetilde A}:\widetilde A\to A_0$ is a [covering map](../../../../../covering-space.md)**.

Under the [classification of connected covering spaces](../../../../../classification-of-connected-covering-spaces.md), its [subgroup](../../../../../subgroup.md) consists of based loops in $A_0$ whose lifts close at $\widetilde a_0$. A loop viewed in $X$ closes in the [universal cover](../../../../../universal-cover.md) exactly when its class in $\pi_1(X,a_0)$ is trivial. Hence the [subgroup](../../../../../subgroup.md) is

$$
\boxed{p_*\pi_1(\widetilde A,\widetilde a_0)=\ker\{\pi_1(A,a_0)\xrightarrow{i_*}\pi_1(X,a_0)\}.}
$$

Here $\pi_1(A,a_0)=\pi_1(A_0,a_0)$, so the [subgroup](../../../../../subgroup.md) formula itself needs no change. Injectivity of the covering's induced fundamental-group map is the usual homotopy-lifting property.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
