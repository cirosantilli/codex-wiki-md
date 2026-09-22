# Equivalence class

↑ **Parent:** [Equivalence relation](equivalence-relation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivalence_class)

An equivalence class collects all the [set elements](element-of-a-set.md) indistinguishable from a specified [set element](element-of-a-set.md) under an [equivalence relation](equivalence-relation.md). For an [equivalence relation](equivalence-relation.md) $R$ on a [set](set-split.md) $X$, the precise definition is

$$
[x]_R=\{y\in X:xRy\},\qquad x\in X.
$$

The ambient [set](set-split.md) matters: a finite class for [integer congruence](integer-congruence.md) restricted to $\{0,\ldots,8\}$ differs from the infinite [residue class](residue-class.md) for the same [integer congruence](integer-congruence.md) on all [integers](integer-split.md). We write $[x]$ when the [equivalence relation](equivalence-relation.md) and ambient [set](set-split.md) are clear.

In the finite modulo-three example,

$$
[0]=[3]=[6]=\{0,3,6\},\qquad
[1]=[4]=[7]=\{1,4,7\},\qquad
[2]=[5]=[8]=\{2,5,8\}.
$$

There are nine names $[x]$ but only three distinct [equivalence classes](equivalence-class.md). In particular, $3\in[0]$, whereas $[3]=[0]$: the first statement is membership of a [set element](element-of-a-set.md); the second is equality of two [sets](set-split.md).

For any [equivalence relation](equivalence-relation.md) on $X$, the essential rule is

$$
xRy\quad\Longleftrightarrow\quad[x]_R=[y]_R
\quad\Longleftrightarrow\quad[x]_R\cap[y]_R\ne\varnothing.
$$

[Reflexivity](reflexive-relation.md) puts $x$ in $[x]_R$, so the [equivalence classes](equivalence-class.md) are nonempty and cover $X$. If two [equivalence classes](equivalence-class.md) share $z$, the [symmetric relation](symmetric-relation.md) property and [transitivity](transitive-relation.md) relate their defining elements through $z$; [transitivity](transitive-relation.md) then makes their members coincide. Thus distinct [equivalence classes](equivalence-class.md) are disjoint, giving a [partition of a set](partition-of-a-set.md). Conversely, declare two [set elements](element-of-a-set.md) equivalent when they belong to the same block of a [partition of a set](partition-of-a-set.md). The three relation properties follow immediately and its [equivalence classes](equivalence-class.md) recover the blocks. [Patrick Brosnan, Undergraduate Algebra, §2.10, Lemma 2.81, Corollary 2.82 and Theorem 2.83](https://www.math.umd.edu/~pbrosnan/notes/ugalg/sect0018.html)

**Table of contents**

- [Equivalence class representative](equivalence-class-representative.md)

## ↑ Ancestors (8)

1. [Equivalence relation](equivalence-relation.md)
2. [Binary relation](binary-relation.md)
3. [Finitary relation](finitary-relation.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (120)

- [Canonical projection of a quotient set](canonical-projection-of-a-quotient-set.md)
- [Circle modulo reflection](circle-modulo-reflection.md)
- [Collapsing a subset to a point](collapsing-a-subset-to-a-point.md)
- [Communicating class](communicating-class.md)
- [Connected component](connected-component.md)
- [Equality-only grouping lower bound](equality-only-grouping-lower-bound.md)
- [Equivalence class](equivalence-class.md)
- [Equivalence class representative](equivalence-class-representative.md)
- [Equivalence relation](equivalence-relation.md)
- [Essential infimum and essential supremum](essential-infimum-and-essential-supremum.md)
- [Essential range](essential-range.md)
- [Essentially bounded function](essentially-bounded-function.md)
- [Failure of Minkowski inequality below exponent one](failure-of-minkowski-inequality-below-exponent-one.md)
- [Fiber of a function](fiber-of-a-function.md)
- [Germ (mathematics)](germ-mathematics.md)
- [Hash table resizing](hash-table-resizing.md)
- [Integer congruence](integer-congruence.md)
- [Intersection of equivalence relations](intersection-of-equivalence-relations.md)
- [Kernel (algebra)](kernel-algebra.md)
- [Key equality](key-equality.md)
- [L-infinity norm](l-infinity-norm.md)
- [Line with two origins](line-with-two-origins.md)
- [Lp norm](lp-norm.md)
- [Odd part of a positive integer](odd-part-of-a-positive-integer.md)
- [One-sided representatives of a one-dimensional BV function](one-sided-representatives-of-a-one-dimensional-bv-function.md)
- [Orbit (group theory)](orbit-group-theory.md)
- [Partition of a set](partition-of-a-set.md)
- [Solution](past-exam-of-the-geometry-course-of-the-university-of-oxford/2010/a/1/ii/solution.md)
- [Solution](past-exam-of-the-geometry-of-surfaces-course-of-the-university-of-oxford/2023/1/b/solution.md)
- [Solution](past-exam-of-the-geometry-of-surfaces-course-of-the-university-of-oxford/2023/1/c/solution.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2023/3/a/ii/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2007/a/4/iii/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/10/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/2c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/2c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-20/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-12/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/2d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/2d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-9/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/2d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/5e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/5e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/23j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/1/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/3/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/2d/a/solution.md)
- [Solution](past-exam-of-the-model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford/2007/b/5/ii/solution.md)
- [Solution](past-exam-of-the-model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford/2007/b/7/iv/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/e/e2/a/iii/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/e/e2/b/ii/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/e/e2/b/iii/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2013/e/2/a/i/solution.md)
- [Solution](past-exam-of-the-options-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/e/2/a/i/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2004/e/e4/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/e/e4/a/iii/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/e/e4/b/i/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2012/b/b2/e/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2012/e/e4/a/iv/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2012/e/e4/b/ii/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2007/e/4/a/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/e/e4/a/iii/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/e/e4/b/i/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/e/e4/c/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2014/1/c/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2015/2/c/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2015/2/c/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2015/2/c/iii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2017/2/b/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/2/a/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/2/a/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/3/b/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/3/b/iii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/3/c/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2021/3/c/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/i/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/a/iii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/ii/solution.md)
- [Solution](past-exam-of-the-topology-course-of-the-university-of-oxford/2023/2/b/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation/6/b/v/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/discrete-mathematics-probability-and-continuous-mathematics/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/discrete-mathematics-probability-and-continuous-mathematics/3/e/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/discrete-mathematics-probability-and-continuous-mathematics/3/e/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability-resit/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/discrete-mathematics-continuous-mathematics-and-probability/1/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/discrete-mathematics/3/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/discrete-mathematics/3/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/discrete-mathematics/3/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/1/d/ii/solution.md)
- [Path component](path-component.md)
- [Periodic common refinement of floor-quotient partitions](periodic-common-refinement-of-floor-quotient-partitions.md)
- [Point-evaluation kernel is not closed in the integral norm](point-evaluation-kernel-is-not-closed-in-the-integral-norm.md)
- [Prime-support equivalence relation](prime-support-equivalence-relation.md)
- [Quantum state ray](quantum-state-ray.md)
- [Quotient set](quotient-set.md)
- [Quotient topological space](quotient-topological-space.md)
- [Quotient topology](quotient-topology.md)
- [Residue class](residue-class.md)
- [Saturation of a subset](saturation-of-a-subset.md)
- [Semidecidable least-representative transversal](semidecidable-least-representative-transversal.md)
- [Set partition](set-partition.md)
- [Smooth hyperbolic polygon gluing criterion](smooth-hyperbolic-polygon-gluing-criterion.md)
- [Sphere with its equator collapsed](sphere-with-its-equator-collapsed.md)
- [Unreduced rational representation](unreduced-rational-representation.md)
- [Vertex link in a polygonal schema](vertex-link-in-a-polygonal-schema.md)
- [Zeroth law of thermodynamics](zeroth-law-of-thermodynamics.md)
