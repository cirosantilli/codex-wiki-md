<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Allocate a distinct game and copy every destination entry from the corresponding source position:
```
def flip(k: Int): Flip = {
  require(1 < k && k <= game.length)
  val result = new Flip(game.length)
  var i = 0
  while (i < game.length) {
    val source = if (i < k) k - 1 - i else i
    result.game(i) = game(source)
    i += 1
  }
  result.flips = k :: flips
  result
}
```
The [loop invariant](../../../../../loop-invariant.md) says that the receiver is unchanged and destination positions before `i` equal the reversal of the first $k$ source entries followed by the untouched suffix. The [loop variant](../../../../../loop-variant.md) is $game.length-i$. At exit the copying is complete. Reversal is a bijection on positions, so the destination remains a [permutation](../../../../../permutation.md). **The returned object's [array](../../../../../array-data-structure.md) is independent of the receiver's [array](../../../../../array-data-structure.md)**, while the immutable tail of its history [list](../../../../../list-abstract-data-type.md) can safely be shared. The source's only supplied constructor randomizes the new [array](../../../../../array-data-structure.md) before the copy; that work is redundant but does not affect correctness. An additional private constructor could avoid it without changing the required result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
