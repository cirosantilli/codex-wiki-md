<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start at the highest level. Move right only while the next key is strictly smaller than `x`, then descend without returning to `head`.
```
def findPreds(x: Int): Array[Node] = {
  require(Int.MinValue < x && x < Int.MaxValue)
  val preds = new Array[Node](NumLevels)
  var n = head
  var level = NumLevels - 1
  while (level >= 0) {
    while (n.nexts(level).datum < x) {
      n = n.nexts(level)
    }
    preds(level) = n
    level -= 1
  }
  preds
}
```
At each inner loop head, `n` belongs to the current level and has key below `x`. Every node already passed has key below `x`. The [representation invariant](../../../../../representation-invariant.md) ensures that `n` also belongs to the next lower level. Stopping just before a key at least `x` therefore gives

$$
\boxed{\mathrm{preds}(h).\mathrm{datum}<x\leq\mathrm{preds}(h).\mathrm{nexts}(h).\mathrm{datum}.}
$$

The tail prevents a null dereference during the comparison. Strict comparison makes the predecessor lie before the first occurrence of `x`, including duplicates. On the source diagram, `findPreds(14)` yields data $[11,9,9,-\infty]$, in increasing level order.[p. 4, skiplist diagram and Question 3(c)](../../../../../imperative-programming-examination-paper-by-the-university-of-oxford-2014.md)

With the customary random-level policy this has expected logarithmic [time complexity](../../../../../time-complexity.md) for a suitably sized level cap; an unlucky [skip list](../../../../../skip-list.md) can require a linear scan. No deterministic logarithmic guarantee is claimed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
