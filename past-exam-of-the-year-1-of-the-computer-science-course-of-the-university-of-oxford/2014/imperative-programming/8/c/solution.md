<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Store the [minimal elements](../../../../../minimal-element-of-a-partially-ordered-set.md) of the finite generating [set](../../../../../set-split.md). The represented [upper set](../../../../../upper-set.md) itself may be infinite; the code manipulates its finite basis.
```
class UpSet[T <: Ordered[T]](c: Set[T]) extends Ordered[UpSet[T]] {
  private val basis: Set[T] = minimal(c)
  def contains(x: T): Boolean = basis.exists(a => a <= x)
  def intersection(that: UpSet[T]): UpSet[T] = {
    val generators: Set[T] =
      for (a <- basis; b <- that.basis) yield a.lub(b)
    new UpSet[T](generators)
  }
  def <=(that: UpSet[T]): Boolean = basis.forall(a => that.contains(a))
  def lub(that: UpSet[T]): UpSet[T] =
    new UpSet[T](basis union that.basis)
}
```
The [abstraction function](../../../../../abstraction-function.md) and [representation invariant](../../../../../representation-invariant.md) are

$$
\boxed{\alpha(B)=\uparrow B=\{x:\exists b\in B,\ b\leq x\},\qquad B\text{ finite with no strictly comparable distinct values}.}
$$

Removing nonminimal generators preserves the upward closure: in a finite generating [set](../../../../../set-split.md), repeatedly descending below any discarded element must reach a retained [minimal element](../../../../../minimal-element-of-a-partially-ordered-set.md). Thus the constructor represents exactly the required [finitely generated upper set](../../../../../finitely-generated-upper-set.md).

Membership follows directly from the [abstraction function](../../../../../abstraction-function.md). For [intersection](../../../../../set-intersection.md), an element $x$ lies above some $a\in B$ and some $b\in C$ exactly when it lies above their [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md):

$$
(a\leq x\land b\leq x)\iff a\vee b\leq x.
$$

The forward implication is the defining leastness property; the reverse uses that $a\vee b$ is an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) and [transitivity](../../../../../transitive-relation.md). Consequently

$$
\uparrow B\cap\uparrow C=\uparrow\{a\vee b:a\in B,b\in C\}.
$$

Recomputing [minimal elements](../../../../../minimal-element-of-a-partially-ordered-set.md) therefore yields a finite basis for the exact [intersection](../../../../../set-intersection.md).

For [subset](../../../../../subset.md) inclusion, it suffices that every generator of the left-hand [upper set](../../../../../upper-set.md) belongs to the right-hand [upper set](../../../../../upper-set.md). Necessity holds because each generator belongs to its own closure by [reflexivity](../../../../../reflexive-relation.md). Sufficiency holds because the right-hand [set](../../../../../set-split.md) is upward closed. Finally,

$$
\boxed{\uparrow B\subseteq\uparrow C\iff\forall b\in B,\ \exists c\in C,\ c\leq b,\qquad (\uparrow B)\vee(\uparrow C)=\uparrow(B\cup C).}
$$

Thus `lub` computes [union](../../../../../set-union.md), which is the [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) under [subset](../../../../../subset.md) inclusion. The empty basis represents the empty [set](../../../../../set-split.md); all four methods handle it without a special case. As in part (a), two distinct Scala objects may denote the same abstract ordered value. Retaining several equivalent representatives is harmless: they generate the same upward closure, and the strict-comparison test removes only genuinely nonminimal values.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
