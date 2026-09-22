# Compact space

↑ **Parent:** [Topology](topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_space)

A [topological space](topological-space.md) $X$ is [compact](compact-space.md) when every [open cover](open-cover.md) has a [finite subcover](finite-subcover.md): whenever [open sets](open-set.md) $U_i$ satisfy $X=\bigcup_{i\in I}U_i$, some finite selection satisfies $X=U_{i_1}\cup\cdots\cup U_{i_m}$. A [subset](subset.md) $K$ of an ambient [topological space](topological-space.md) is [compact](compact-space.md) when its [subspace topology](subspace-topology.md) is [compact](compact-space.md); equivalently, every [open cover](open-cover.md) of $K$ by ambient [open sets](open-set.md) has a [finite subcover](finite-subcover.md). The word _every_ matters: finding one [finite subcover](finite-subcover.md) of one [open cover](open-cover.md) is not enough to establish [compactness](compact-space.md). [MIT Analysis II, section 1.6 and Definition 1.23](https://ocw.mit.edu/courses/18-101-analysis-ii-fall-2005/babd982be745679b6d691f78b1c18f53_lectures.pdf)

The [closed interval](closed-real-interval.md) $[0,1]$ is [compact](compact-space.md) by the [Heine-Borel theorem](heine-borel-theorem.md). For a concrete [open cover](open-cover.md), take the three [open intervals](open-interval.md) $(-0.1,0.45)$, $(0.35,0.8)$, and $(0.7,1.1)$. Their [union](set-union.md) is $(-0.1,1.1)$, so they cover every point of $[0,1]$, including both endpoints. The overlaps have lengths $0.1$ and $0.1$, leaving no gaps. Each member is necessary for this particular [open cover](open-cover.md): removing them respectively leaves $0$, $0.5$, or $1$ uncovered.

<a id="image-a-finite-subcover-of-a-closed-interval-and-an-open-cover-with-no-finite-subcover"></a>
![](compact-open-cover.png)

**[Figure 8](#image-a-finite-subcover-of-a-closed-interval-and-an-open-cover-with-no-finite-subcover). A finite subcover of a closed interval, and an open cover with no finite subcover**.

Above, hollow markers denote the excluded endpoints of the covering [open intervals](open-interval.md), while the solid endpoints belong to the covered [closed interval](closed-real-interval.md). Below, each displayed [open interval](open-interval.md) is one member of an infinite [open cover](open-cover.md) of $(0,1)$; finitely many rows always leave points near zero uncovered. The rows are vertically separated for readability and all refer to the same [real line](real-line.md).

The [open interval](open-interval.md) $(0,1)$ is a [bounded set](bounded-set.md) but is not [compact](compact-space.md): the [open sets](open-set.md)

$$
U_n=(1/n,1),\qquad n\geq2,
$$

give an [open cover](open-cover.md) of $(0,1)$, since every $0<x<1$ has $1/n<x$ for sufficiently large $n$. These are also [open sets](open-set.md) for the [subspace topology](subspace-topology.md) on $(0,1)$. Any nonempty finite selection has a largest index $N$, so its [union](set-union.md) is just $(1/N,1)$ and misses the point $1/(N+1)$, which still belongs to $(0,1)$. Thus no [finite subcover](finite-subcover.md) exists, however many members we select. The same family is not an [open cover](open-cover.md) of $[0,1]$, since it misses both endpoints.

In a [metric space](metric-space.md), [compactness](compact-space.md) is equivalent to [sequential compactness](sequentially-compact-space.md): every [sequence](sequence.md) in the [subset](subset.md) has a [convergent subsequence](convergent-subsequence.md) whose [limit of a sequence](limit-of-a-sequence.md) belongs to that [subset](subset.md). This equivalence does not extend to all [topological spaces](topological-space.md). For example, $x_n=1/n$ for $n\geq2$ has [limit of a sequence](limit-of-a-sequence.md) zero in $[0,1]$. The same [sequence](sequence.md) lies in $(0,1)$, but every [subsequence](subsequence.md) still has [limit of a sequence](limit-of-a-sequence.md) zero on the [real line](real-line.md), so no [subsequence](subsequence.md) converges to a point of $(0,1)$. Merely approaching a [boundary](boundary-of-a-set.md) is harmless when the required point remains available. [MIT Analysis I, Compactness vs. Sequential Compactness, Theorem 1 and its metric-space proof](https://ocw.mit.edu/courses/18-100b-analysis-i-fall-2010/b7780b2a0629359b11c5de998c72a147_MIT18_100BF10_compactness.pdf)

<a id="image-the-same-sequence-approaches-an-included-endpoint-in-a-closed-interval-and-a-missing-endpoint-in-an-open-interval"></a>
![](compactness-missing-endpoint.png)

**[Figure 9](#image-the-same-sequence-approaches-an-included-endpoint-in-a-closed-interval-and-a-missing-endpoint-in-an-open-interval). The same sequence approaches an included endpoint in a closed interval and a missing endpoint in an open interval**.

Both panels show the [sequence](sequence.md) $x_n=1/n$ for $n\geq2$ approaching zero. In the [closed interval](closed-real-interval.md), zero is an allowed [limit of a sequence](limit-of-a-sequence.md); in the [open interval](open-interval.md), the hollow marker identifies the missing point. This single [sequence](sequence.md) disproves [sequential compactness](sequentially-compact-space.md) of $(0,1)$; [compactness](compact-space.md) of $[0,1]$ still requires control of every [open cover](open-cover.md) or every [sequence](sequence.md), supplied by the [Heine-Borel theorem](heine-borel-theorem.md).

An [infinite set](infinite-set.md) with the [discrete topology](discrete-space.md) similarly fails [compactness](compact-space.md), using the [open cover](open-cover.md) by all its [singletons](singleton-mathematics.md). Every [finite set](finite-set.md) is [compact](compact-space.md) in any [topology](topology-split.md): select one covering [open set](open-set.md) for each point. The [empty set](empty-set.md) is [compact](compact-space.md) because the empty selection is a [finite subcover](finite-subcover.md). This [open cover](open-cover.md) definition does not require the [topological space](topological-space.md) to be [Hausdorff](hausdorff-space.md); in [algebraic geometry](algebraic-geometry-split.md) it is often called [quasi-compactness](compact-space.md).

The beauty of [compactness](compact-space.md) is that information valid around each point can often be controlled using finitely many regions. A [finite subcover](finite-subcover.md) lets us combine finitely many local bounds, or choose the smallest of finitely many positive tolerances, to obtain control across the whole [compact space](compact-space.md). This is why [compactness](compact-space.md) repeatedly turns approximation into existence and why it is so useful in [optimization](mathematical-optimization-split.md) through the [extreme value theorem](extreme-value-theorem.md).

Every [closed set](closed-set.md) in a [compact space](compact-space.md) is [compact](compact-space.md), and a [continuous image of a compact space](continuous-image-of-a-compact-space.md) is [compact](compact-space.md). The latter proof pulls an [open cover](open-cover.md) back by [inverse images](preimage.md), selects a [finite subcover](finite-subcover.md), and maps forward. This makes [compactness](compact-space.md) useful for proving existence: the [extreme value theorem](extreme-value-theorem.md) guarantees that a [continuous function](continuous-function.md) from a nonempty [compact space](compact-space.md) to the [real line](real-line.md) attains both a [minimum](minimum-of-a-subset-of-a-total-order.md) and a [maximum](maximum-of-a-subset-of-a-total-order.md). For example, $q(x)=x(1-x)=1/4-(x-1/2)^2$ on $[0,1]$ has [maximum](maximum-of-a-subset-of-a-total-order.md) $1/4$ at $1/2$ and [minimum](minimum-of-a-subset-of-a-total-order.md) zero at its endpoints. On $(0,1)$ its [infimum](infimum.md) is still zero but is never attained. [MIT Analysis II, Theorems 1.24-1.25](https://ocw.mit.edu/courses/18-101-analysis-ii-fall-2005/babd982be745679b6d691f78b1c18f53_lectures.pdf)

**Table of contents**

- [Ultrafilter characterization of compactness](ultrafilter-characterization-of-compactness.md)
- [Compact exhaustion](compact-exhaustion.md)
- [Compact Hausdorff space](compact-hausdorff-space.md)
  - [Supremum convergence for decreasing continuous functions](supremum-convergence-for-decreasing-continuous-functions.md)
  - [Closed relation generated by a set-split pair of compact Hausdorff maps](closed-relation-generated-by-a-set-split-pair-of-compact-hausdorff-maps.md)
  - [Separable compactification need not be metrizable](separable-compactification-need-not-be-metrizable.md)
- [Heine-Borel theorem](heine-borel-theorem.md)
- [Finite intersection property](finite-intersection-property.md)
- [Continuous image of a compact space](continuous-image-of-a-compact-space.md)
- [Quotient of a compact space](quotient-of-a-compact-space.md)
- [Lebesgue number lemma](lebesgue-number-lemma.md)
- [Normality of a compact Hausdorff space](normality-of-a-compact-hausdorff-space.md)
- [Alexander's subbase lemma](alexander-s-subbase-lemma.md)
- [Locally compact space](locally-compact-space.md)
  - [Compactly detected closed-set theorem in a locally compact Hausdorff space](compactly-detected-closed-set-theorem-in-a-locally-compact-hausdorff-space.md)

## ↑ Ancestors (5)

1. [Topology](topology-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (43)

- [Compact graph of a continuous map](compact-graph-of-a-continuous-map.md)
- [Compact metric space](compact-metric-space.md)
- [Compact space](compact-space.md)
- [Compact subset of a Hausdorff space](compact-subset-of-a-hausdorff-space.md)
- [Continuous image of a compact space](continuous-image-of-a-compact-space.md)
- [Countable product compactness implies countable choice](countable-product-compactness-implies-countable-choice.md)
- [Extreme value theorem](extreme-value-theorem.md)
- [Heine-Borel theorem](heine-borel-theorem.md)
- [Homeomorphism](homeomorphism.md)
- [Lattice approximation from two-point approximation](lattice-approximation-from-two-point-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/13b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/3g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106/4/solution.md)
- [5](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106/5.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/13e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/3g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/12e/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/21h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-130/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/25h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/10g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-130/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-131/1/b/solution.md)
- [Supremum norm](supremum-norm.md)
- [Tychonoff's theorem](tychonoff-s-theorem.md)
- [Ultrafilter characterization of compact Hausdorff spaces](ultrafilter-characterization-of-compact-hausdorff-spaces.md)
- [Ultralimit](ultralimit.md)
