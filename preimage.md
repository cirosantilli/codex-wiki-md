# Preimage

↑ **Parent:** [Image and preimage of a function](image-and-preimage-of-a-function.md)

For a [function](function-split.md) $f:X\to Y$ and a [subset](subset.md) $U\subseteq Y$, its [preimage](preimage.md) is

$$
f^{-1}(U)=\{x\in X:f(x)\in U\}.
$$

It is a [subset](subset.md) of the original [domain of a function](domain-of-a-function.md). The notation does not require an [inverse function](inverse-function.md): the [preimage](preimage.md) of a [singleton set](singleton-mathematics.md) can have no members, one member, or many members. In the finite example, $f^{-1}(\{0\})=\{a,b\}$, $f^{-1}(\{1\})=\{c\}$ and $f^{-1}(\{3\})=\varnothing$. The [preimage](preimage.md) of a [singleton set](singleton-mathematics.md) is also its [fiber of a function](fiber-of-a-function.md).

For [subsets](subset.md) $U,V\subseteq Y$, [preimages](preimage.md) preserve both [unions](set-union.md) and [intersections](set-intersection.md):

$$
f^{-1}(U\cup V)=f^{-1}(U)\cup f^{-1}(V),\qquad
f^{-1}(U\cap V)=f^{-1}(U)\cap f^{-1}(V).
$$

For the [intersection](set-intersection.md), the same input $x$ belongs precisely when its single output $f(x)$ belongs to both $U$ and $V$. There is no opportunity to choose different witnesses, which is what made the image counterexample fail. The identities also hold for arbitrary families of output [subsets](subset.md).

In the finite example, choose $U=\{0,1\}$ and $V=\{0,2\}$. Then

$$
f^{-1}(U)=\{a,b,c\},\qquad f^{-1}(V)=\{a,b,d\},\qquad
f^{-1}(U\cap V)=f^{-1}(\{0\})=\{a,b\}.
$$

The [intersection](set-intersection.md) of the two preimages is exactly the same [set](set-split.md) $\{a,b\}$. Complements are preserved with respect to the appropriate source and target [sets](set-split.md):

$$
f^{-1}(Y\setminus U)=X\setminus f^{-1}(U).
$$

For example, the unused output three contributes no extra input: with $U=\{0,2\}$, both sides of the complement identity are $\{c\}$. See [Lebl, Proposition 0.3.15: preimages of unions, intersections and complements](https://www.jirka.org/ra/html/sec_basicset.html).

This makes [preimages](preimage.md) useful for transporting conditions. The [solution set](solution-set.md) of $g(x)=0$ is $g^{-1}(\{0\})$, and a [zero set](zero-set.md) is a preimage of zero. Requiring two output conditions takes the [intersection](set-intersection.md) of their preimages. In [topology](topology-split.md), a [continuous function](continuous-function.md) pulls every [open set](open-set.md) back to an [open set](open-set.md); a [measurable function](measurable-function.md) pulls the specified [measurable sets](measurable-set.md) in its [codomain](codomain.md) back to [measurable sets](measurable-set.md) in its [domain of a function](domain-of-a-function.md). These definitions use [preimages](preimage.md) because their set operations remain consistent even when the [function](function-split.md) is noninjective.

**Table of contents**

- [Dimension of the preimage of a vector subspace](dimension-of-the-preimage-of-a-vector-subspace.md)

## ↑ Ancestors (6)

1. [Image and preimage of a function](image-and-preimage-of-a-function.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (79)

- [Borel measurable function](borel-measurable-function.md)
- [Canonical projection of a quotient set](canonical-projection-of-a-quotient-set.md)
- [Closure characterization of continuity](closure-characterization-of-continuity.md)
- [Continuity into a product space](continuity-into-a-product-space.md)
- [Dimension of the preimage of a vector subspace](dimension-of-the-preimage-of-a-vector-subspace.md)
- [Entire function](entire-function.md)
- [Essential range](essential-range.md)
- [Fiber of a function](fiber-of-a-function.md)
- [Finer topology](finer-topology.md)
- [Finite-coordinate basis for the product topology](finite-coordinate-basis-for-the-product-topology.md)
- [Fortissimo space](fortissimo-space.md)
- [Great Picard theorem](great-picard-theorem.md)
- [Hash collision](hash-collision.md)
- [Image and preimage of a function](image-and-preimage-of-a-function.md)
- [Image of a function](image-of-a-function.md)
- [Inverse function](inverse-function.md)
- [Kernel (algebra)](kernel-algebra.md)
- [Lebesgue measurable function](lebesgue-measurable-function.md)
- [Line with two origins](line-with-two-origins.md)
- [Little Picard theorem](little-picard-theorem.md)
- [Open map](open-map.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2007/4/c/solution.md)
- [Solution](past-exam-of-the-algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/6/b/solution.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2017/1/c/i/solution.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2015/1/c/solution.md)
- [Solution](past-exam-of-the-lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford/2008/b/7/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2007/a/1/a/ii/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2007/a/1/b/i/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2007/a/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/14a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/1d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-i/3/a/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2008/e/e1/a/i/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2008/e/e1/b/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2009/e/e1/a/ii/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2009/e/e1/b/ii/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2009/e/e2/a/ii/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2004/d/d4/c/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2008-printed-variant/e/e3/a/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2008/e/e3/a/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/e/e3/a/iii/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/e/e4/c/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2007/e/2/iii/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2007/e/2/iv/solution.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2021/4/b/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2014/1/a/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2014/1/b/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2014/1/c/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/1/f/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/1/f/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/2/d/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/1/a/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/iii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/iv/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/discrete-mathematics-probability-and-continuous-mathematics/1/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/discrete-mathematics-probability-and-continuous-mathematics/1/d/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/1/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/1/a/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/1/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/1/b/iv/solution.md)
- [Pasting lemma for closed subspaces](pasting-lemma-for-closed-subspaces.md)
- [Preimage](preimage.md)
- [Pushforward filter](pushforward-filter.md)
- [Quotient topological space](quotient-topological-space.md)
- [Quotient topology](quotient-topology.md)
- [Quotient topology of a cofinite space](quotient-topology-of-a-cofinite-space.md)
- [Simon coset state](simon-coset-state.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
- [Strictly increasing function](strictly-increasing-function.md)
- [Topological disjoint union](topological-disjoint-union.md)
- [Total variation distance under a measurable map](total-variation-distance-under-a-measurable-map.md)
- [Zero set](zero-set.md)
