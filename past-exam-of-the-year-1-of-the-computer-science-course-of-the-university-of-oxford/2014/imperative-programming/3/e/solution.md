<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Pick the new node's highest level once, and splice the same node into every level up to that height. `pickLevel` must return a value in `0 until NumLevels`.
```
def add(x: Int): Unit = {
  require(Int.MinValue < x && x < Int.MaxValue)
  val preds = findPreds(x)
  val highest = pickLevel
  require(0 <= highest && highest < NumLevels)
  val n = new Node(x)
  for (level <- 0 to highest) {
    n.nexts(level) = preds(level).nexts(level)
    preds(level).nexts(level) = n
  }
}
```
The fresh [array](../../../../../array-data-structure.md) contains `null` above the chosen height. At each changed level the new node lies after a smaller value and before a value at least `x`. Every new occurrence is placed before all previous equal-valued nodes, consistently across levels. Therefore the [representation invariant](../../../../../representation-invariant.md) is preserved and

$$
\boxed{\alpha_{\mathrm{new}}=\alpha_{\mathrm{old}}\text{ with one extra occurrence of }x.}
$$

The splice work is $O(\mathrm{highest}+1)$ in addition to one [skip list](../../../../../skip-list.md) search.

## ↑ Ancestors (12)

1. [E](../e.md)
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
