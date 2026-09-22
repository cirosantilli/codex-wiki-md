<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [interval containment order](../../../../../interval-containment-order.md) compares the lower endpoints in reverse and the upper endpoints in their ordinary order. The smallest containing [integer interval](../../../../../integer-interval.md) uses the smaller lower endpoint and the larger upper endpoint.
```
class Interval(val l: Int, val u: Int) extends Ordered[Interval] {
  require(l <= u)
  def <=(that: Interval): Boolean = that.l <= l && u <= that.u
  def lub(that: Interval): Interval =
    new Interval(math.min(l, that.l), math.max(u, that.u))
}
```
Endpoint comparison immediately proves [reflexivity](../../../../../reflexive-relation.md), [transitivity](../../../../../transitive-relation.md), and [antisymmetry](../../../../../antisymmetry.md) on interval values. If two separately allocated instances have the same endpoints, they denote the same abstract [interval](../../../../../interval-mathematics.md); object identity is not the mathematical equality used by this [partial order](../../../../../partially-ordered-set.md).

The returned [interval](../../../../../interval-mathematics.md) contains both operands. Every other containing [interval](../../../../../interval-mathematics.md) has a lower endpoint at most both original lower endpoints and an upper endpoint at least both original upper endpoints, so it also contains the returned hull. Hence

$$
\boxed{[l,u]\vee[l',u']=[\min(l,l'),\max(u,u')].}
$$

This [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) need not equal the ordinary [union](../../../../../set-union.md): the hull of $[1,2]$ and $[5,6]$ is $[1,6]$, including the gap.

## ↑ Ancestors (12)

1. [A](../a.md)
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
