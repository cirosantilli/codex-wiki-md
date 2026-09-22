<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep precisely those elements with no strictly smaller element in the input. Express strictness using the [partial order](../../../../../partially-ordered-set.md) itself, avoiding reliance on Scala reference equality.
```
def minimal[T <: Ordered[T]](xs: Set[T]): Set[T] =
  xs.filter { x =>
    !xs.exists(y => (y <= x) && !(x <= y))
  }
```
In a [partial order](../../../../../partially-ordered-set.md), $y<x$ means $y\leq x$ and $x\not\leq y$. Therefore

$$
\boxed{\mathrm{minimal}(X)=\{x\in X:\nexists y\in X,\ y<x\}.}
$$

The empty [set](../../../../../set-split.md) produces the empty [set](../../../../../set-split.md). An incomparable pair is retained in full; a [minimal element](../../../../../minimal-element-of-a-partially-ordered-set.md) need not be a least element. At most $O(|X|^2)$ order comparisons are needed, and only the supplied F-bounded generic interface is required.

## ↑ Ancestors (12)

1. [B](../b.md)
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
