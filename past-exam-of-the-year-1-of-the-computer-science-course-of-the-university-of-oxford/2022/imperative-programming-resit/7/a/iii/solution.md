<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Map a pure, terminating function only when a value is demanded; use the adapters to obtain the [cursor](../../../../../../cursor.md) form with caching:

```
def map[T, U](f: T => U, it: Iter[T]): Iter[U] = new Iter[U] {
  def hasNext: Boolean = it.hasNext
  def next(): U = {
    require(it.hasNext, "empty iterator")
    f(it.next())
  }
}

def map[T, U](f: T => U, cur: Cursor[T]): Cursor[U] =
  asCursor(map(f, asIter(cur)))
```

Each demanded output is the function applied to the corresponding input, preserving order and lazy access even for an infinite [sequence](../../../../../../sequence.md). The [cursor](../../../../../../cursor.md) adapter caches its mapped current value, so repeated reads need not recompute `f`. Totality/purity of `f` is the usual assumption for the mathematical [sequence](../../../../../../sequence.md)-map [postcondition](../../../../../../postcondition.md); an exception-throwing or state-changing function would need additional behavioral clauses.

**Both functions may be named `map` because their second parameter types differ**, `Iter[T]` versus `Cursor[T]`. [Method overloading](../../../../../../method-overloading.md) selects the applicable signature; its distinction is not based solely on the return type.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
