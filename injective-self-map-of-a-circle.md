# Injective self-map of a circle

↑ **Parent:** [Circle](circle.md)

Every continuous injective map $g:S^1\to S^1$ is a [homeomorphism](homeomorphism.md). After normalizing $g(1)=1$ by a rotation, it is [homotopic](homotopy-split.md) either to the identity or to complex conjugation, and has [degree](degree-of-a-continuous-mapping.md) $1$ or $-1$.

To see this without assuming surjectivity, lift $t\mapsto g(e^{2\pi it})$ on $[0,1]$ through the [covering map](covering-space.md) $u\mapsto e^{2\pi iu}$ to a path $G$ with $G(0)=0$. Injectivity makes $G$ injective on $[0,1)$, hence strictly monotone. Its endpoint $d=G(1)$ is an integer. Strict monotonicity excludes $d=0$; if $|d|>1$, the [intermediate value theorem](intermediate-value-theorem.md) gives an interior integer value, contradicting injectivity of $g$. Thus $d=\pm1$, and $\exp(2\pi i((1-s)G(t)+sdt))$ descends to a [homotopy](homotopy-split.md) from $g$ to $z\mapsto z^d$. If $g$ omitted a point, a continuous branch of the [complex argument](argument-complex-analysis.md) on the punctured circle would make it [null-homotopic](null-homotopic-map.md), contradicting this nonzero [degree](degree-of-a-continuous-mapping.md). Hence it is surjective. A continuous bijection from a [compact space](compact-space.md) to a [Hausdorff space](hausdorff-space.md) is a [homeomorphism](homeomorphism.md).

## ↑ Ancestors (7)

1. [Circle](circle.md)
2. [Topological space](topological-space.md)
3. [Topology](topology-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-topology-and-groups-course-of-the-university-of-oxford/2010/1/solution.md)
