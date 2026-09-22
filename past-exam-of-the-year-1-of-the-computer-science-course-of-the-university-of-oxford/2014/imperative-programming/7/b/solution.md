<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep 26 cached counts, updating them after a successful delegated edit. Count exactly lowercase letters; the query alphabet does not make uppercase letters the same character.
```
trait CharTrackPlugIn extends Doc {
  private val counts = Array.fill[Int](26)(0)
  private def lower(x: Char): Boolean = 'a' <= x && x <= 'z'
  abstract override def insert(x: Char, pos: Int): Unit = {
    super.insert(x, pos)
    if (lower(x)) counts(x - 'a') += 1
  }
  abstract override def delete(pos: Int): Char = {
    val x = super.delete(pos)
    if (lower(x)) counts(x - 'a') -= 1
    x
  }
  def getCount(x: Char): Int = {
    assert(lower(x))
    counts(x - 'a')
  }
}
```
For an initially empty underlying document that stores inserted arguments unchanged, the [representation invariant](../../../../../representation-invariant.md) is

$$
\boxed{\mathrm{counts}(c-\texttt{'a'})=\#\{i:\mathrm{read}(i)=c\}\quad(c=\texttt{'a'},\ldots,\texttt{'z'}).}
$$

Insertion increments precisely the inserted lowercase character's count. Deletion uses the returned character, avoiding an extra indexed read and decrementing the character actually removed. Updating after `super` means a rejected edit leaves the counts unchanged. Both the added update work and `getCount` use $O(1)$ [time complexity](../../../../../time-complexity.md) and fixed storage.

The `abstract override` methods implement a [stackable trait modification](../../../../../stackable-trait-modification.md): they require a concrete document implementation further along the delegation chain. The invariant above depends on subsequent layers preserving inserted characters. Part (d) deliberately composes a transforming layer that can break this assumption; that is the [transform-sensitive trait frequency counter](../../../../../transform-sensitive-trait-frequency-counter.md) phenomenon.

## ↑ Ancestors (12)

1. [B](../b.md)
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
