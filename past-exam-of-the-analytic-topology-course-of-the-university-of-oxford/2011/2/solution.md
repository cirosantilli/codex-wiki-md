<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Compactifications.** A [Hausdorff compactification](../../../hausdorff-compactification.md) of $X$ is a compact [Hausdorff space](../../../hausdorff-space.md) $K$ together with a [topological embedding](../../../topological-embedding.md) $j:X\to K$ having dense image. We identify $X$ with that image.

For noncompact locally compact Hausdorff $X$, adjoin $\infty$ and give $X^+=X\cup\{\infty\}$ its [one-point compactification](../../../alexandroff-extension.md) topology: retain the open sets of $X$, and take $\{\infty\}\cup(X\setminus C)$, with $C$ compact, as a neighborhood base at $\infty$. Compact subsets are closed, making this a topology with the original [subspace topology](../../../subspace-topology.md) on $X$.

An open cover contains a neighborhood of $\infty$, leaving a compact subset of $X$ to cover by finitely many more members. Hence $X^+$ is compact. Points of $X$ are separated using its Hausdorff property; to separate $x\in X$ from $\infty$, use local compactness to choose an open $U\ni x$ with compact closure and take $X^+\setminus\overline U$ at $\infty$. Finally every neighborhood of $\infty$ meets $X$, because $X$ itself is not compact. Thus $X$ is dense and **$X^+$ is a [Hausdorff compactification](../../../hausdorff-compactification.md) with one-point remainder**.

**Comparison maps.** The [Stone-Čech compactification](../../../stone-cech-compactification.md) of a [Tychonoff space](../../../completely-regular-hausdorff-space.md) has the universal property that every [continuous map](../../../continuous-map.md) from $X$ to a compact [Hausdorff space](../../../hausdorff-space.md) extends continuously to $\beta X$. Applying it to any [Hausdorff compactification](../../../hausdorff-compactification.md) $K$ gives a continuous surjection $\pi:\beta X\to K$ fixing $X$. Surjectivity follows because its compact image is closed and contains the dense set $X$.

We need the [fibers of compactification comparison maps](../../../fibers-of-compactification-comparison-maps.md) property

$$
\boxed{\pi^{-1}(X)=X.}
$$

Suppose $\pi(z)=x\in X$ with $z\ne x$. By regularity of compact Hausdorff $\beta X$, choose an [open neighborhood](../../../open-neighbourhood.md) $U$ of $x$ with $z\notin\overline U$. The embedding $X\subseteq K$ supplies open $V\subseteq K$ containing $x$ and satisfying $V\cap X\subseteq U\cap X$. The open set $\pi^{-1}(V)$ contains $z$. Density of $X$ implies $z\in\overline{\pi^{-1}(V)\cap X}=\overline{V\cap X}\subseteq\overline U$, a contradiction. Thus the displayed identity holds.

**Equivalence of (a), (b), (c).** Clearly (b) implies (c). If (c) holds in $K$, inverse images under $\pi$ and $\pi^{-1}(X)=X$ show that $X$ is a [G-delta set](../../../g-delta-set.md) in $\beta X$, giving (a). Conversely assume (a) and write $X=\bigcap_n U_n$ in $\beta X$. The sets $F_n=\beta X\setminus U_n$ are compact and miss $X$. Their images $\pi(F_n)$ are closed in $K$ and miss $X$ by the fiber identity. Since $\pi$ is onto, they exhaust $K\setminus X$. Hence

$$
\boxed{X=\bigcap_n\bigl(K\setminus\pi(F_n)\bigr).}
$$

This proves (b), for every $K$. This [G-delta compactification invariance](../../../g-delta-compactification-invariance.md) defines a [Čech-complete space](../../../cech-complete-space.md).

**The Baire property.** Suppose $X=\bigcap_n G_n$ in a compact Hausdorff $K$, with $X$ dense and all $G_n$ open. Each $G_n$ is dense. For dense open subsets $U_n$ of $X$, choose open $O_n\subseteq K$ with $U_n=X\cap O_n$. Every nonempty open subset of $K$ meets $X$ in a nonempty relatively open set and hence meets $U_n$, so each $O_n$ is dense in $K$.

The assumed [Baire category theorem](../../../baire-category-theorem.md) in $K$ makes $\bigcap_n(G_n\cap O_n)$ dense in $K$. This set lies in $X$ and equals $\bigcap_n U_n$, so it is also dense in $X$. Therefore **[Čech-complete spaces are Baire spaces](../../../cech-complete-spaces-are-baire-spaces.md)**.

Enumerate $\mathbb Q=\{q_n:n\in\omega\}$. Each $\mathbb Q\setminus\{q_n\}$ is open and dense in $\mathbb Q$, while their intersection is empty. Thus $\mathbb Q$ is not a [Baire space](../../../baire-space.md), and consequently

$$
\boxed{\mathbb Q\text{ is not a }G_\delta\text{ in any Hausdorff compactification of }\mathbb Q.}
$$

If $\mathbb Q$ were a [G-delta set](../../../g-delta-set.md) in $\mathbb R$, it would also be one in $\mathbb R^+$: the subspace $\mathbb R$ is open in its [one-point compactification](../../../alexandroff-extension.md), and adjoining that open condition to a countable intersection preserves the [G-delta set](../../../g-delta-set.md) property. Since $\mathbb Q$ is dense in $\mathbb R$ and hence in $\mathbb R^+$, this would be a [Hausdorff compactification](../../../hausdorff-compactification.md) of $\mathbb Q$ contradicting the preceding conclusion. Therefore $\boxed{\mathbb Q\text{ is not }G_\delta\text{ in }\mathbb R}$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2011](../../2011-split.md)
3. [Past exam of the analytic topology course of the University of Oxford](../../split.md)
4. [Analytic topology course of the University of Oxford](../../../analytic-topology-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
