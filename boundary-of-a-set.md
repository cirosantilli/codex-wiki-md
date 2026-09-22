# Boundary of a set

↑ **Parent:** [Topological space](topological-space.md)

The [boundary](boundary-of-a-set.md) of a [subset](subset.md) $A$ of a [topological space](topological-space.md) $X$ consists of the points whose every [neighbourhood](neighbourhood-mathematics.md) in $X$ meets both $A$ and its [complement](complement-of-a-set.md) $X\setminus A$. Equivalently,

$$
\partial_X A=\operatorname{cl}_X A\setminus\operatorname{int}_X A
=\operatorname{cl}_X A\cap\operatorname{cl}_X(X\setminus A).
$$

Here the two operations are [closure](closure-topology.md) and [interior](interior-topology.md). The second formula shows that the [boundary](boundary-of-a-set.md) is a [closed set](closed-set.md) and that $A$ and its [complement](complement-of-a-set.md) have the same [boundary](boundary-of-a-set.md). It locates precisely the points where membership cannot be decided from a small [neighbourhood](neighbourhood-mathematics.md) alone. [Jiří Lebl, Basic Analysis, Definition 7.2.23 and Propositions 7.2.26–7.2.27](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_basic_analysis.pdf)

For $A=[0,1)$ in the usual [real line](real-line.md), the [interior](interior-topology.md) is $(0,1)$, the [closure](closure-topology.md) is $[0,1]$, and the [boundary](boundary-of-a-set.md) is $\{0,1\}$. In particular, $0$ belongs both to $A$ and to its [boundary](boundary-of-a-set.md), while $1$ belongs to the [boundary](boundary-of-a-set.md) but not to $A$. A [boundary](boundary-of-a-set.md) point need not be excluded from the original [set](set-split.md): [open sets](open-set.md) exclude all their [boundary](boundary-of-a-set.md) points, [closed sets](closed-set.md) contain all theirs, and this half-open [interval](interval-mathematics.md) does one of each.

<a id="image-relative-openness-in-a-closed-interval-and-the-boundary-of-a-half-open-interval"></a>
![](relative-openness-and-boundary.png)

**[Figure 5](#image-relative-openness-in-a-closed-interval-and-the-boundary-of-a-half-open-interval). Relative openness in a closed interval and the boundary of a half-open interval**.

The upper panel visualizes the relative example from [open set](open-set.md): for $X=[0,1]$ and $A=[0,1/2)$, an [open ball](open-ball.md) about zero in $X$ is $B_X(0,r)=X\cap(-r,r)=[0,r)$ when $0<r<1/2$. This [open ball](open-ball.md) stays in $A$; points outside $X$ are not required. The middle panel shows that $X$ is [clopen](clopen-set.md) in itself, with [interior](interior-topology.md) and [closure](closure-topology.md) both $X$ and empty [boundary](boundary-of-a-set.md), although its [boundary](boundary-of-a-set.md) in the [real line](real-line.md) is $\{0,1\}$. The lower panel returns to ambient space $\mathbb R$ and separates the [interior](interior-topology.md), [closure](closure-topology.md), and [boundary](boundary-of-a-set.md) of $[0,1)$; both marked [boundary](boundary-of-a-set.md) points are included in the [boundary](boundary-of-a-set.md) itself.

**Table of contents**

- [Boundary of a domain](boundary-of-a-domain.md)

## ↑ Ancestors (6)

1. [Topological space](topological-space.md)
2. [Topology](topology-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Boundary of a domain](boundary-of-a-domain.md)
- [Interior (topology)](interior-topology.md)
