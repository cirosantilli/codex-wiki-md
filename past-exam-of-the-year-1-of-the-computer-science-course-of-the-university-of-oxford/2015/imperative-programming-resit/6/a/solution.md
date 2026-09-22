<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an immutable [list](../../../../../list-abstract-data-type.md) as private storage and cache its length. This makes the [data refinement](../../../../../data-refinement.md) transparent without depending on library-specific [dynamic array](../../../../../dynamic-array.md) costs:
```
class DocImpl extends Doc {
  private var chars: List[Char] = Nil
  private var length: Int = 0

  def size: Int = length

  def insert(x: Char, pos: Int): Unit = {
    require(0 <= pos && pos <= length)
    val parts = chars.splitAt(pos)
    chars = parts._1 ::: (x :: parts._2)
    length += 1
  }

  def delete(pos: Int): Char = {
    require(0 <= pos && pos < length)
    val parts = chars.splitAt(pos)
    val old = parts._2.head
    chars = parts._1 ::: parts._2.tail
    length -= 1
    old
  }

  def read(pos: Int): Char = {
    require(0 <= pos && pos < length)
    chars(pos)
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is $\mathrm{length}=\operatorname{length}(\mathrm{chars})\geq0$, with `chars` representing the abstract document [sequence](../../../../../sequence.md). `splitAt(pos)` isolates exactly the prefix before the selected [array index](../../../../../array-index.md)-style position. Insertion retains that prefix and the old suffix, placing the new character between them. Deletion returns the old suffix head and retains its tail. Updating the cached length by one preserves the [representation invariant](../../../../../representation-invariant.md). `read` and `size` preserve the abstract state.

$$
\boxed{\operatorname{size}:\Theta(1);\qquad\operatorname{insert},\operatorname{delete},\operatorname{read}:O(n+1).}
$$

The [preconditions](../../../../../precondition.md) permit insertion at the end, including position zero in an empty document, but forbid reading or deleting at the end.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
