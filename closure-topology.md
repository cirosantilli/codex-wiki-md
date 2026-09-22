# Closure (topology)

↑ **Parent:** [Topology](topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closure_(topology))

The [closure](closure-topology.md) of a [subset](subset.md) $A$ of a [topological space](topological-space.md) $X$ is the smallest [closed set](closed-set.md) containing $A$. Equivalently, it is the [intersection](set-intersection.md) of all [closed sets](closed-set.md) containing $A$, or the [set](set-split.md) of points whose every [neighbourhood](neighbourhood-mathematics.md) in $X$ meets $A$. The notation $\operatorname{cl}_X A$ makes the ambient [topological space](topological-space.md) explicit. This definition works without a [metric](metric.md) or any appeal to [sequences](sequence.md). [James Munkres, Topology, closure and interior of a set](https://math.mit.edu/~hrm/palestine/munkres-topology.pdf)

For $A=[0,1)$ in the usual [real line](real-line.md), $\overline A=[0,1]$: every [neighbourhood](neighbourhood-mathematics.md) of $1$ meets $A$, while a point outside $[0,1]$ has an [open ball](open-ball.md) disjoint from $A$. Passing to the [closure](closure-topology.md) adds the missing endpoint and retains all original points, including [isolated points](isolated-point.md) when present. In general, the [closure](closure-topology.md) is $A$ together with its [limit points](limit-point.md); its individual points are the [adherent points](adherent-point.md) of $A$.

The [closure](closure-topology.md) turns an arbitrary [subset](subset.md) into a [closed set](closed-set.md) with no unnecessary added points. It satisfies $A\subseteq\overline A$ and $\overline{\overline A}=\overline A$; a [subset](subset.md) is [closed](closed-set.md) exactly when $A=\overline A$. In a [metric space](metric-space.md), $x\in\overline A$ exactly when some [sequence](sequence.md) of points of $A$ has [limit of a sequence](limit-of-a-sequence.md) $x$: choose its $n$th point in $A\cap B(x,1/n)$. For a general [topological space](topological-space.md), keep the [neighbourhood](neighbourhood-mathematics.md) definition; [sequences](sequence.md) need not detect every point of the [closure](closure-topology.md).

**Table of contents**

- [Adherent point](adherent-point.md)

## ↑ Ancestors (5)

1. [Topology](topology-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
