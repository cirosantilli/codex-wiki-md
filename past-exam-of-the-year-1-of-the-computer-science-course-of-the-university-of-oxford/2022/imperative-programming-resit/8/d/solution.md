<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Nonnegative count functions form a valid subtype of the immutable value interface, but they are not closed under its exact subtraction. Preserve the inherited result type rather than silently changing the subtraction contract:

```
trait MultiSet[T] extends CompleteMultiSet[T] {
  // Additional invariant: count(t) >= 0 for every t.
  // Inherited arithmetic still returns CompleteMultiSet[T].
}

class MultiSetImp[T](initial: Map[T, Int])
    extends CompleteMultiSetImp[T](initial) with MultiSet[T] {
  require(initial.values.forall(_ >= 0), "negative multiplicity")
}

def ms[T](ts: T*): MultiSet[T] =
  new MultiSetImp[T](ts.distinct.map(t => (t, 1)).toMap)
```

**The invariant guarantees nonnegative multiplicities in every `MultiSet` object**, and the factory gives each supplied element exactly one occurrence. Since the objects are immutable, inherited operations cannot invalidate that invariant in the receiver. Their declared result is a [complete multiset](../../../../../signed-multiset.md), which can legitimately contain negative counts; for example, subtracting a positive count from zero produces a signed result.

If an ordinary [multiset](../../../../../multiset.md)-only difference is desired, introduce a separate operation with count $\max(0,a(t)-b(t))$, or an interface whose subtraction explicitly has that contract. Replacing the parent's exact difference by truncated difference under the same signature would violate [behavioral subtyping](../../../../../behavioral-subtyping.md); strengthening its [precondition](../../../../../precondition.md) to forbid negative results would also fail to implement the parent's unrestricted mathematical contract. Retaining the complete result type above reuses every correct default without that substitution error.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
