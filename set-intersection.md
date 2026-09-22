# Set intersection

↑ **Parent:** [Set](set-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_(set_theory))

The intersection $A\cap B$ keeps exactly the [set elements](element-of-a-set.md) common to both [sets](set-split.md):

$$
A\cap B=\{x:x\in A\text{ and }x\in B\},\qquad x\in A\cap B\iff(x\in A)\wedge(x\in B).
$$

Membership in an [intersection](set-intersection.md) therefore uses [logical conjunction](logical-conjunction.md) (AND). For $A=\{1,2,3\}$ and $B=\{3,4\}$, the only shared member is $3$, so $A\cap B=\{3\}$. The [Venn diagram](venn-diagram.md) in [set union](set-union.md) shades only the overlap for this operation.

An [intersection](set-intersection.md) is useful when every requirement must hold. If $A$ and $B$ are the [sets](set-split.md) of database records passing two separate conditions, their [intersection](set-intersection.md) gives the records passing both. Similarly, satisfying two [equations](equation.md) requires belonging to the [intersection](set-intersection.md) of their [solution sets](solution-set.md). The same membership rule applies even when the objects have entirely different meanings.

For a family of [sets](set-split.md), the [intersection](set-intersection.md) $\bigcap_{i\in I}A_i$ contains exactly the [set elements](element-of-a-set.md) belonging to every [set](set-split.md) $A_i$:

$$
x\in\bigcap_{i\in I}A_i\iff\forall i\in I:\ x\in A_i.
$$

Here [universal quantification](universal-quantification.md) expresses “every”. If all the [sets](set-split.md) lie within a fixed [universal set](universal-set.md) $U$, the [intersection](set-intersection.md) over no indexing members is defined to be $U$: there are no requirements to fail. This convention depends on specifying $U$. By contrast, intersecting with the [empty set](empty-set.md) always gives $A\cap\varnothing=\varnothing$.

**Table of contents**

- [Finite intersection](finite-intersection.md)
- [Disjoint sets](disjoint-sets.md)
- [Countable intersection](countable-intersection.md)

## ↑ Ancestors (6)

1. [Set](set-split.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Axis-aligned bounding box](axis-aligned-bounding-box.md)
- [Boolean operations on events](boolean-operations-on-events.md)
- [Bounding volume](bounding-volume.md)
- [Conservative enclosure test](conservative-enclosure-test.md)
- [Constructive solid geometry](constructive-solid-geometry.md)
- [Continuity into a product space](continuity-into-a-product-space.md)
- [Coprime integers](coprime-integers.md)
- [Finite-coordinate basis for the product topology](finite-coordinate-basis-for-the-product-topology.md)
- [List-based set representation](list-based-set-representation.md)
- [Open rectangles in a finite product](open-rectangles-in-a-finite-product.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/geometric-modelling/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/geometric-modelling/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/geometric-modelling/1/f/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/12/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation/3/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/1/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/1/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/1/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/1/d/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability-resit/1/a/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability-resit/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/discrete-mathematics-continuous-mathematics-and-probability/1/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/discrete-mathematics-continuous-mathematics-and-probability/1/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/1/a/solution.md)
- [Sv39 page table](sv39-page-table.md)
- [Two-level address translation](two-level-address-translation.md)
