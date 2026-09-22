<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

These operations consume the receiver, as expected for this destructive [iterator](../../../../../iterator.md) interface. `exists` stops immediately after the first successful test.
```
trait RichIter[T] extends Iter[T] {
  def foreach(f: T => Unit): Unit = {
    while (hasNext) f(next())
  }

  def exists(p: T => Boolean): Boolean = {
    while (hasNext) {
      if (p(next())) return true
    }
    false
  }

  def foldLeft[U](x: U)(f: (U, T) => U): U = {
    var acc = x
    while (hasNext) acc = f(acc, next())
    acc
  }
}
```
For `foreach`, after $k$ iterations the supplied [function](../../../../../function-split.md) has been applied in order to exactly the first $k$ entries. For `exists`, every consumed entry has failed the [predicate](../../../../../predicate.md) unless the method is returning true. For the [left fold](../../../../../left-fold.md), the [loop invariant](../../../../../loop-invariant.md) after consuming $k$ entries is

$$
acc=f(\cdots f(f(x,a_1),a_2)\cdots,a_k).
$$

Each iteration extends the expression by the next entry on the right. For a finite remaining [sequence](../../../../../sequence.md), its unconsumed length is a common [loop variant](../../../../../loop-variant.md). Thus

$$
\boxed{foreach\text{ visits in order};\quad exists\text{ short-circuits};\quad foldLeft\text{ associates to the left}.}
$$

An empty [iterator](../../../../../iterator.md) invokes no callback, gives false for `exists`, and returns $x$ from the [left fold](../../../../../left-fold.md). On an infinite [iterator](../../../../../iterator.md), `exists` can terminate when it finds a match; the other two operations ordinarily do not terminate. With constant-cost callbacks, finite input of length $n$ takes $O(n)$ [time complexity](../../../../../time-complexity.md) and constant [auxiliary space](../../../../../auxiliary-space.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
