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

## ↑ Ancestors (7)

1. [Equivalence relation](equivalence-relation.md)
2. [Binary relation](binary-relation.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (59)

- [Canonical projection of a quotient set](canonical-projection-of-a-quotient-set.md)
- [Communicating class](communicating-class.md)
- [Connected component](connected-component.md)
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
- [Lp norm](lp-norm.md)
- [Odd part of a positive integer](odd-part-of-a-positive-integer.md)
- [One-sided representatives of a one-dimensional BV function](one-sided-representatives-of-a-one-dimensional-bv-function.md)
- [Orbit (group theory)](orbit-group-theory.md)
- [Partition of a set](partition-of-a-set.md)
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
- [Path component](path-component.md)
- [Point-evaluation kernel is not closed in the integral norm](point-evaluation-kernel-is-not-closed-in-the-integral-norm.md)
- [Prime-support equivalence relation](prime-support-equivalence-relation.md)
- [Quantum state ray](quantum-state-ray.md)
- [Quotient set](quotient-set.md)
- [Quotient topological space](quotient-topological-space.md)
- [Quotient topology](quotient-topology.md)
- [Residue class](residue-class.md)
- [Semidecidable least-representative transversal](semidecidable-least-representative-transversal.md)
- [Set partition](set-partition.md)
- [Unreduced rational representation](unreduced-rational-representation.md)
- [Zeroth law of thermodynamics](zeroth-law-of-thermodynamics.md)
