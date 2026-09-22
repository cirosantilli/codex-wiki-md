<h1 id="7/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Prefer the first [sequence](../../../../../../sequence.md) whenever it is nonempty, otherwise delegate to the second:

```
def cat[T](t: Iter[T], u: Iter[T]): Iter[T] = new Iter[T] {
  def hasNext: Boolean = t.hasNext || u.hasNext
  def next(): T = {
    if (t.hasNext) t.next()
    else {
      require(u.hasNext, "empty iterator")
      u.next()
    }
  }
}

def cat[T](t: Cursor[T], u: Cursor[T]): Cursor[T] = new Cursor[T] {
  def hasCurrent: Boolean = t.hasCurrent || u.hasCurrent
  def current: T = {
    if (t.hasCurrent) t.current
    else {
      require(u.hasCurrent, "empty cursor")
      u.current
    }
  }
  def next(): Unit = {
    if (t.hasCurrent) t.next()
    else {
      require(u.hasCurrent, "empty cursor")
      u.next()
    }
  }
}
```

Assume the two destructive inputs have noninterfering states; in particular, passing the same [iterator](../../../../../../iterator.md) twice does not create a replayable copy of its original [sequence](../../../../../../sequence.md). Fresh independent [iterators](../../../../../../iterator.md) provide that behavior. Under this ownership condition, the [abstraction function](../../../../../../abstraction-function.md) is always the concatenation `t.seq ++ u.seq`. Consumption from `t` removes the concatenation's head; once `t` is empty, consumption from `u` does so. Availability tests short-circuit, so an infinite first [sequence](../../../../../../sequence.md) never unnecessarily touches the second.

For finite lengths $p,q$, under a client loop with one availability test and one advance per element, the [iterator](../../../../../../iterator.md) version directly invokes `t.hasNext` **$2(p+q)+1$ times**, including the final false test. For a [cursor](../../../../../../cursor.md) client with one availability test, one `current` read and one advance per element, the corresponding count is **$3(p+q)+1$**. These count calls made by the shown adapters, not extra checks hidden inside arbitrary underlying methods. A client can repeat availability/current queries arbitrarily often, so no bound depending only on $p,q$ applies without such a client protocol.

Cache a permanent “first input exhausted” flag after the first negative test to avoid repeated queries to `t` while traversing `u`; this reduces the dependence to $O(p+1)$ first-input queries under the same protocols. Availability caching can reduce additional repeated checks. The flag is sound because an [iterator](../../../../../../iterator.md)'s consumed [sequence](../../../../../../sequence.md) does not spontaneously grow again.

## ↑ Ancestors (13)

1. [V](../v.md)
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
