# Path component

↑ **Parent:** [Path-connected space](path-connected-space.md)

A [path component](path-component.md) of a [topological space](topological-space.md) $X$ is a nonempty [subset](subset.md) maximal among its [path-connected](path-connected-space.md) [subsets](subset.md). The [path component](path-component.md) through $x$ can be described as

$$
P_x=\{y\in X:\text{there is a continuous path in }X\text{ from }x\text{ to }y\}.
$$

Every point along such a [continuous path](continuous-path.md) also belongs to $P_x$: the initial part of the [path](continuous-path.md) reaches that point. Thus the [paths](continuous-path.md) witnessing membership stay inside $P_x$. This makes [path components](path-component.md) useful for deciding which allowed positions can be reached from one another by continuous motion.

Every [path component](path-component.md) lies inside one [connected component](connected-component.md), because every [path-connected space](path-connected-space.md) is [connected](connected-space.md). Thus each [connected component](connected-component.md) is a [union](set-union.md) of [path components](path-component.md). In a [locally path-connected space](locally-path-connected-space.md) the two classifications agree, by [connected locally path-connected spaces are path-connected](connected-locally-path-connected-spaces-are-path-connected.md). For a [subset](subset.md) of the [real line](real-line.md) with its usual [subspace topology](subspace-topology.md), the classifications also agree: every [connected component](connected-component.md) is a [real interval](interval-mathematics.md), and interpolation supplies a [continuous path](continuous-path.md) within it.

The [topologist's sine curve](topologist-s-sine-curve.md) shows why the distinction matters in general. Use specifically the closed version

$$
G=\{(x,\sin(1/x)):0<x\le1\},\qquad
L=\{0\}\times[-1,1],\qquad T=G\cup L,
$$

with the [subspace topology](subspace-topology.md) from the usual [Euclidean plane](euclidean-plane.md). It has one [connected component](connected-component.md), $T$, but two [path components](path-component.md), $G$ and $L$. The [graph of a function](graph-of-a-function.md) $G$ is a [continuous image of a connected space](continuous-image-of-a-connected-space.md), and its [closure](closure-topology.md) is $T$, so [closure of a connected set](closure-of-a-connected-set.md) gives [connectedness](connected-space.md). Each of $G,L$ is [path-connected](path-connected-space.md), but a [continuous path](continuous-path.md) crossing from $L$ into $G$ would force its second coordinate to oscillate between $1$ and $-1$ arbitrarily near its departure time, contradicting [continuity](continuous-function.md); the [topologist's sine curve](topologist-s-sine-curve.md) article gives the short argument. Also $G$ is not [closed](closed-set.md) in $T$, so [path components](path-component.md) need not be [closed](closed-set.md), unlike [connected components](connected-component.md).[p. 78, and the discussion after Lemma C4.12, p. 84: the sine-curve obstruction and nonclosed path components; here the positive graph is restricted to $0<x\le1$](general-topology-by-tom-leinster.md)

Being joined by a [continuous path](continuous-path.md) is an [equivalence relation](equivalence-relation.md). Proof outline: the constant [path](continuous-path.md) joins a point to itself; $t\mapsto\gamma(1-t)$ reverses a [path](continuous-path.md); and a [path](continuous-path.md) from $x$ to $y$ followed by one from $y$ to $z$ gives a [path](continuous-path.md) from $x$ to $z$. For the last construction, run each [path](continuous-path.md) on half of $[0,1]$; their values agree at $1/2$, so the [pasting lemma for closed subspaces](pasting-lemma-for-closed-subspaces.md) gives [continuity](continuous-function.md). The [equivalence classes](equivalence-class.md) are [path-connected](path-connected-space.md), are maximal, and form a [partition of a set](partition-of-a-set.md) of $X$ into [path components](path-component.md).[p. 84: path equivalence and maximal path-connected subsets](general-topology-by-tom-leinster.md)

## ↑ Ancestors (5)

1. [Path-connected space](path-connected-space.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Connected locally path-connected spaces are path-connected](connected-locally-path-connected-spaces-are-path-connected.md)
- [Connected subset of the real line](connected-subset-of-the-real-line.md)
- [Euler characteristic and holes](euler-characteristic-and-holes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/4f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-127/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/21h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/11f/solution.md)
- [Path component](path-component.md)
- [Path-connected space](path-connected-space.md)
- [Topologist's sine curve](topologist-s-sine-curve.md)
- [Zeroth homology group](zeroth-homology-group.md)
