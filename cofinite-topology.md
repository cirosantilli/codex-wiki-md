# Cofinite topology

↑ **Parent:** [Topology](topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cofinite_topology)

The [cofinite topology](cofinite-topology.md) on a [set](set-split.md) $X$ declares the [empty set](empty-set.md) and all [cofinite](cofinite-set.md) [subsets](subset.md) to be [open sets](open-set.md): a nonempty [open set](open-set.md) may exclude only a [finite set](finite-set.md) of points. There is no assumed [metric](metric.md). On an [infinite set](infinite-set.md), this gives a particularly small collection of [open sets](open-set.md) while still making every [singleton](singleton-mathematics.md) a [closed set](closed-set.md). On a [finite set](finite-set.md), every [subset](subset.md) has finite [complement](complement-of-a-set.md), so the [cofinite topology](cofinite-topology.md) is the [discrete topology](discrete-space.md).[Definition 1.1.9: finite complement topology](point-set-topology-by-romyar-sharifi/chapter-1-topological-spaces.md)

For an original example, use $X=\mathbb N_{>0}$ and choose

$$
U=X\setminus\{2,5,8\},\qquad V=X\setminus\{1,3,7\}.
$$

Both are [open sets](open-set.md), and their [intersection](set-intersection.md) is $U\cap V=X\setminus\{1,2,3,5,7,8\}$. Thus $4,6,9,10,\ldots$ are in both. Their finite exclusions cannot separate the infinite remainder. The [finite intersection](finite-intersection.md) of any finite collection of nonempty [open sets](open-set.md) is again a nonempty [open set](open-set.md), since its [complement](complement-of-a-set.md) is a [finite union](finite-union.md) of [finite sets](finite-set.md). An arbitrary nonempty [union](set-union.md) is [open](open-set.md) because its [complement](complement-of-a-set.md) is contained in the finite [complement](complement-of-a-set.md) of any one nonempty member.

<a id="image-two-open-sets-with-finite-exclusions-still-overlap-in-an-infinite-cofinite-topology"></a>
![](cofinite-open-sets-finite-exclusions.png)

**[Figure 3](#image-two-open-sets-with-finite-exclusions-still-overlap-in-an-infinite-cofinite-topology). Two open sets with finite exclusions still overlap in an infinite cofinite topology**. Original sets on $\mathbb N_{>0}$. Only the first sixteen labels are drawn; the dots continue indefinitely and are all included after the last excluded label. Spacing is for readability and defines no [metric](metric.md). Filled circles belong to the displayed [set](set-split.md); crosses are excluded.

The [cofinite topology](cofinite-topology.md) is useful for separating hypotheses that familiar [metric spaces](metric-space.md) package together. An infinite cofinite [topological space](topological-space.md) is a [T1 space](t1-space.md), because its [singletons](singleton-mathematics.md) are [closed](closed-set.md), but is not a [Hausdorff space](hausdorff-space.md), because two nonempty [open sets](open-set.md) cannot be [disjoint sets](disjoint-sets.md). It is a [hyperconnected space](hyperconnected-space.md) and hence a [connected space](connected-space.md). Moreover, [every subset of a cofinite space is compact](every-subset-of-a-cofinite-space-is-compact.md), and [sequence convergence in the cofinite topology](sequence-convergence-in-the-cofinite-topology.md) can have many limits. These are compatible properties, rather than contradictions: the usual uniqueness and closedness results use the [Hausdorff space](hausdorff-space.md) hypothesis.[Example 1.5.10 and Proposition 1.5.11: closed points, overlapping neighbourhoods, non-repeating sequences and uniqueness in Hausdorff spaces](point-set-topology-by-romyar-sharifi/chapter-1-topological-spaces.md)

**Table of contents**

- [Sequence convergence in the cofinite topology](sequence-convergence-in-the-cofinite-topology.md)
- [Every subset of a cofinite space is compact](every-subset-of-a-cofinite-space-is-compact.md)
- [Continuous maps from an infinite cofinite space to a Hausdorff space are constant](continuous-maps-from-an-infinite-cofinite-space-to-a-hausdorff-space-are-constant.md)

## ↑ Ancestors (5)

1. [Topology](topology-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Cofinite topology](cofinite-topology.md)
- [Continuous maps between cofinite and tail topologies](continuous-maps-between-cofinite-and-tail-topologies.md)
- [Continuous maps from an infinite cofinite space to a Hausdorff space are constant](continuous-maps-from-an-infinite-cofinite-space-to-a-hausdorff-space-are-constant.md)
- [Finite subsets do not define a topology on an infinite set](finite-subsets-do-not-define-a-topology-on-an-infinite-set.md)
- [Hyperconnected space](hyperconnected-space.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/4e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/4e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/4f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/14f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/2e/solution.md)
- [Sequence convergence in the cofinite topology](sequence-convergence-in-the-cofinite-topology.md)
- [Sober space](sober-space.md)
- [T1 space](t1-space.md)
- [Upper-ray topology on the real line](upper-ray-topology-on-the-real-line.md)
