<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [proper filter](../../../../../proper-filter.md) $\mathcal F$ on $X$ is a nonempty family of [subsets](../../../../../subset.md), [closed](../../../../../closed-set.md) under finite [intersection](../../../../../set-intersection.md) and passage to [supersets](../../../../../superset.md), with $\varnothing\notin\mathcal F$. An [ultrafilter](../../../../../ultrafilter.md) is a maximal [proper filter](../../../../../proper-filter.md), equivalently one which contains, for each $A\subseteq X$, exactly one of $A$ and $X\setminus A$. The [pushforward filter](../../../../../pushforward-filter.md) is

$$
f_*\mathcal F=\{B\subseteq Y:f^{-1}[B]\in\mathcal F\}.
$$

[Inverse images](../../../../../preimage.md) preserve [intersections](../../../../../set-intersection.md) and [complements](../../../../../complement-of-a-set.md). Thus it is a [proper filter](../../../../../proper-filter.md), and the either-a-set-or-its-complement criterion shows it is an [ultrafilter](../../../../../ultrafilter.md) whenever $\mathcal F$ is one.

[Convergence of a filter](../../../../../convergence-of-a-filter.md) $\mathcal F\to x$ means that every [neighborhood](../../../../../neighbourhood-mathematics.md) of $x$ belongs to $\mathcal F$. A mapping is [continuous](../../../../../continuous-function.md) exactly when $\mathcal F\to x$ implies $f_*\mathcal F\to f(x)$ for all [proper filters](../../../../../proper-filter.md) and points. The forward implication follows from [inverse images](../../../../../preimage.md) of [neighborhoods](../../../../../neighbourhood-mathematics.md). For the converse apply the criterion to the [neighborhood](../../../../../neighbourhood-mathematics.md) [proper filter](../../../../../proper-filter.md) at $x$: each [inverse image](../../../../../preimage.md) of a [neighborhood](../../../../../neighbourhood-mathematics.md) of $f(x)$ must be a [neighborhood](../../../../../neighbourhood-mathematics.md) of $x$, which is [continuity](../../../../../continuous-function.md) at $x$.

A [topological space](../../../../../topological-space.md) is [compact](../../../../../compact-space.md) exactly when every [ultrafilter](../../../../../ultrafilter.md) converges to at least one point; equivalently every [proper filter](../../../../../proper-filter.md) has a cluster point. For completeness, in a [compact space](../../../../../compact-space.md) the [closed sets](../../../../../closed-set.md) $\overline A$, $A\in\mathcal U$, have the [finite intersection property](../../../../../finite-intersection-property.md), hence a common point $x$. Every [neighborhood](../../../../../neighbourhood-mathematics.md) $N$ of $x$ belongs to the [ultrafilter](../../../../../ultrafilter.md). Indeed, if $N$ did not, choose an [open](../../../../../open-set.md) $V$ with $x\in V\subseteq N$. Then $V$ would not belong either, so $X\setminus V$ would belong. That [set](../../../../../set-split.md) is [closed](../../../../../closed-set.md) and excludes $x$, contradicting the choice of $x$ in every [closure](../../../../../closure-topology.md). Conversely, if an [open cover](../../../../../open-cover.md) has no finite subcover, its [closed](../../../../../closed-set.md) [complements](../../../../../complement-of-a-set.md) generate a [proper filter](../../../../../proper-filter.md). An [ultrafilter](../../../../../ultrafilter.md) extension cannot converge anywhere, because each point has a covering [neighborhood](../../../../../neighbourhood-mathematics.md) whose [complement](../../../../../complement-of-a-set.md) belongs to that [ultrafilter](../../../../../ultrafilter.md). This proves the compactness criterion using the permitted extension principle.

Now suppose $b\in\overline{f[A]}$. The family

$$
\{A\cap f^{-1}[V]:V\text{ is an open neighborhood of }b\}
$$

is a [filter base](../../../../../filter-base.md) of nonempty [sets](../../../../../set-split.md): [closure](../../../../../closure-topology.md) guarantees each [intersection](../../../../../set-intersection.md) is nonempty, and finite [intersections](../../../../../set-intersection.md) correspond to [intersections](../../../../../set-intersection.md) of [neighborhoods](../../../../../neighbourhood-mathematics.md). Extend its generated [proper filter](../../../../../proper-filter.md) to an [ultrafilter](../../../../../ultrafilter.md) $\mathcal H$. It contains $A$ and every $f^{-1}[V]$, so $f_*\mathcal H\to b$.

Conversely, if such an [ultrafilter](../../../../../ultrafilter.md) exists, each [neighborhood](../../../../../neighbourhood-mathematics.md) $V$ of $b$ has $f^{-1}[V]\in\mathcal H$. Its [intersection](../../../../../set-intersection.md) with $A\in\mathcal H$ is nonempty. Thus $V$ meets $f[A]$, proving

$$
\boxed{b\in\overline{f[A]}\quad\Longleftrightarrow\quad\exists\mathcal H\text{ ultrafilter}:A\in\mathcal H,\ f_*\mathcal H\to b.}
$$

This part includes the unnumbered [proper filter](../../../../../proper-filter.md) definitions and criteria preceding the printed subparts.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
