# Heine-Borel theorem

↑ **Parent:** [Compact space](compact-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heine–Borel_theorem)

For every finite $d\geq1$, a [subset](subset.md) $K\subseteq\mathbb R^d$ of [Euclidean space](euclidean-norm.md) is [compact](compact-space.md) if and only if it is a [closed set](closed-set.md) and a [bounded set](bounded-set.md). Here [closed](closed-set.md) means [closed](closed-set.md) in the ambient [Euclidean space](euclidean-norm.md), not merely in $K$ itself, and the [bounded set](bounded-set.md) condition uses the [Euclidean norm](euclidean-norm.md). The [empty set](empty-set.md) is included: it is a [closed set](closed-set.md), a [bounded set](bounded-set.md), and [compact](compact-space.md). [Jiří Lebl, Basic Analysis, Theorem 7.4.14](https://www.jirka.org/ra/html/sec_metcompact.html)

This makes an apparently infinite test practical. To verify [compactness](compact-space.md) of a [closed interval](closed-real-interval.md) $[a,b]$ with finite endpoints, we need not examine every [open cover](open-cover.md): it is [closed](closed-set.md) in the [real line](real-line.md) and a [bounded set](bounded-set.md). By contrast, the [open interval](open-interval.md) $(0,1)$ is a [bounded set](bounded-set.md) but is not [closed](closed-set.md) in the [real line](real-line.md), as the missing-endpoint figure in [compact space](compact-space.md) illustrates. The whole [real line](real-line.md) is [closed](closed-set.md) but is not a [bounded set](bounded-set.md), so it too fails [compactness](compact-space.md). These examples show why both hypotheses are needed.

The same criterion holds in any real or complex [finite-dimensional vector space](finite-dimensional-vector-space.md) equipped with a [norm](norm.md): all [norms](norm.md) there are [equivalent norms](equivalent-norms.md), so they give the same [open sets](open-set.md), [closed sets](closed-set.md), and [bounded sets](bounded-set.md). Since [compactness](compact-space.md) depends only on the [topology](topology-split.md), choosing a different [norm](norm.md) does not change the conclusion. Without an appropriate [topology](topology-split.md), a bare [vector space](vector-space-split.md) alone has no notion of [compactness](compact-space.md).

The restriction to a [finite-dimensional vector space](finite-dimensional-vector-space.md) is essential. In the [l2 sequence space](l2-sequence-space.md), an [infinite-dimensional vector space](infinite-dimensional-vector-space.md) that is also a [Hilbert space](hilbert-space-split.md), let $e_n$ be the [vectors](vector.md) of its standard [orthonormal basis](orthonormal-basis.md). All lie in the [closed unit ball](closed-unit-ball.md) $B=\{x:\lVert x\rVert\leq1\}$, which is a [closed set](closed-set.md) and a [bounded set](bounded-set.md) in the [norm topology](norm-topology.md). For distinct indices, their [inner product](inner-product.md) is zero, giving

$$
\lVert e_n-e_m\rVert^2=\lVert e_n\rVert^2+\lVert e_m\rVert^2-2\operatorname{Re}\langle e_n,e_m\rangle=2.
$$

Thus distinct terms remain distance $\sqrt2$ apart. No [subsequence](subsequence.md) is a [Cauchy sequence](cauchy-sequence.md), hence none is a [convergent sequence](convergent-sequence.md). The equivalence of [compactness](compact-space.md) and [sequential compactness](sequentially-compact-space.md) in a [metric space](metric-space.md) proves that this [closed unit ball](closed-unit-ball.md) is not [compact](compact-space.md). The conclusion concerns the [norm topology](norm-topology.md).

A short proof outline in [Euclidean space](euclidean-norm.md) explains the role of a [finite-dimensional vector space](finite-dimensional-vector-space.md). For a [sequence](sequence.md) in a [bounded set](bounded-set.md), apply the [Bolzano-Weierstrass theorem](bolzano-weierstrass-theorem.md) to each of the [Cartesian coordinates](cartesian-coordinate-system.md) in turn, retaining a [subsequence](subsequence.md) at each of the finitely many steps. The final [subsequence](subsequence.md) is a [convergent sequence](convergent-sequence.md) in all [Cartesian coordinates](cartesian-coordinate-system.md), and a [closed set](closed-set.md) contains its [limit of a sequence](limit-of-a-sequence.md). This yields [sequential compactness](sequentially-compact-space.md), hence [compactness](compact-space.md). Conversely, a [compact subset](compact-space.md) of a [metric space](metric-space.md) is a [closed set](closed-set.md) and a [bounded set](bounded-set.md). [Lebl, Basic Analysis, proof of Theorem 7.4.14](https://www.jirka.org/ra/html/sec_metcompact.html)

## ↑ Ancestors (6)

1. [Compact space](compact-space.md)
2. [Topology](topology-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Bounded-orbit fixed point for a strictly distance-decreasing Euclidean map](bounded-orbit-fixed-point-for-a-strictly-distance-decreasing-euclidean-map.md)
- [Brouwer fixed-point theorem](brouwer-fixed-point-theorem.md)
- [Closed real interval](closed-real-interval.md)
- [Compact group](compact-group.md)
- [Compact interval](compact-interval.md)
- [Compact space](compact-space.md)
- [Norm-compact unit ball criterion](norm-compact-unit-ball-criterion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/10e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/25i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/12g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/2i/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2/4e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/12e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/12f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/2h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/19i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/10e/i/solution.md)
