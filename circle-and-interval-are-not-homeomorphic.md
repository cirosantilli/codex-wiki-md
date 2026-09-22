# Circle and interval are not homeomorphic

↑ **Parent:** [Homeomorphism](homeomorphism.md)

The [circle](circle.md) $S^1$ and the [closed interval](closed-real-interval.md) $[0,1]$ are both [compact](compact-space.md) and [connected](connected-space.md), so those two properties alone do not distinguish them. Instead examine [connectedness](connected-space.md) after removing a point. Every punctured [circle](circle.md) is [connected](connected-space.md): after rotating the missing point to $(1,0)$, the [continuous map](continuous-map.md) $t\mapsto(\cos t,\sin t)$ from the [connected](connected-space.md) [open interval](open-interval.md) $(0,2\pi)$ maps onto it. [Continuous maps](continuous-map.md) preserve [connectedness](connected-space.md). [MIT Analysis II, Theorem 1.29](https://ocw.mit.edu/courses/18-101-analysis-ii-fall-2005/babd982be745679b6d691f78b1c18f53_lectures.pdf)

If a [homeomorphism](homeomorphism.md) $h:S^1\to[0,1]$ existed, choose $p=h^{-1}(1/2)$. Its restriction would give a [homeomorphism](homeomorphism.md) between $S^1\setminus\{p\}$ and $[0,1]\setminus\{1/2\}$. But the latter splits into two nonempty disjoint [open sets](open-set.md) in its [subspace topology](subspace-topology.md), $[0,1/2)$ and $(1/2,1]$, contradicting [connectedness](connected-space.md) of the punctured [circle](circle.md). Removing an endpoint of $[0,1]$ leaves a [connected space](connected-space.md); the proof deliberately chooses the preimage of an interior point. This illustrates how a simple [connectedness](connected-space.md) test can rule out every possible [homeomorphism](homeomorphism.md).

## ↑ Ancestors (6)

1. [Homeomorphism](homeomorphism.md)
2. [Topology](topology-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
