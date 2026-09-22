<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent the [set](../../../../../set-split.md) by a private [list](../../../../../list-abstract-data-type.md) containing each value once. Normalize the constructor input as well as checking future insertions; otherwise duplicate initial entries would violate the intended [set](../../../../../set-split.md) behavior.
```
class Set[T](contents: List[T]) {
  protected var elems: List[T] = contents.distinct

  def add(x: T): Unit = {
    if (!elems.contains(x)) elems = x :: elems
  }

  def delete(): T = {
    require(elems.nonEmpty)
    val x = elems.head
    elems = elems.tail
    x
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is that `elems` contains no duplicates under the chosen stable value equality; the [abstraction function](../../../../../abstraction-function.md) forgets its ordering and returns its [set](../../../../../set-split.md) of elements. The protected field allows the subclass in part (d) to inspect its contents; that subclass is responsible for preserving the [representation invariant](../../../../../representation-invariant.md) if it mutates them.

Insertion makes the represented [set](../../../../../set-split.md) $S\cup\{x\}$. Deletion requires $S\ne\varnothing$, returns some $x\in S$, and leaves $S\setminus\{x\}$. Thus

$$
\boxed{add(x):S'=S\cup\{x\};\qquad delete():x\in S,\ S'=S\setminus\{x\}.}
$$

Deletion does not promise to choose a [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md). With this [linked list](../../../../../linked-list.md) representation, insertion takes $O(|S|)$ [time complexity](../../../../../time-complexity.md) because of its membership check, while deletion takes $O(1)$. Values should not mutate in a way that changes their equality while stored.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
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
