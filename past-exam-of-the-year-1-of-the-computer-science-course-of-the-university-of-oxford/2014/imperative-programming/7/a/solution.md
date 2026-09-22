<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Store characters in a mutable [dynamic array](../../../../../dynamic-array.md). Its length is maintained by the collection, giving constant-time `size`.
```
class DocImpl extends Doc {
  private val text = scala.collection.mutable.ArrayBuffer.empty[Char]
  def insert(x: Char, pos: Int): Unit = {
    require(0 <= pos && pos <= text.length)
    text.insert(pos, x)
  }
  def delete(pos: Int): Char = {
    require(0 <= pos && pos < text.length)
    text.remove(pos)
  }
  def read(pos: Int): Char = {
    require(0 <= pos && pos < text.length)
    text(pos)
  }
  def size: Int = text.length
}
```
The [representation invariant](../../../../../representation-invariant.md) requires a nonnull private [dynamic array](../../../../../dynamic-array.md) containing a finite [sequence](../../../../../sequence.md) of characters, with its internal collection invariant maintained by the library. The [abstraction function](../../../../../abstraction-function.md) is

$$
\boxed{\alpha(\mathrm{text})=\langle\mathrm{text}(0),\ldots,\mathrm{text}(\mathrm{length}-1)\rangle.}
$$

Insertion allows the end position and shifts the suffix right; deletion returns exactly the removed character and shifts the suffix left. `read` leaves the abstract state unchanged. `size` equals the abstract [sequence](../../../../../sequence.md) length in $O(1)$ [time complexity](../../../../../time-complexity.md). Indexed reads are also constant time; insertion and deletion may take linear time, which the question permits.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
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
