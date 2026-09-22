<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Check entries against their own indices, stopping on the first mismatch:
```
def isIdentity: Boolean = {
  var i = 0
  while (i < game.length && game(i) == i) {
    i += 1
  }
  i == game.length
}
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq game.length$ and $game(j)=j$ for every $j<i$. The [loop variant](../../../../../loop-variant.md) is $game.length-i$. A false guard means either every position has passed or the next position is wrong, so **the returned Boolean is true exactly for the identity [permutation](../../../../../permutation.md)**. Neither the game nor its history is changed. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) protects the final indexed comparison.

## ↑ Ancestors (12)

1. [A](../a.md)
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
