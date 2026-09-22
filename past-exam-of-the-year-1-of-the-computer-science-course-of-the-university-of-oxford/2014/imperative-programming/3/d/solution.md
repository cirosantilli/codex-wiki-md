<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The level-zero successor of the predecessor is the first node whose value is at least `x`. Thus only one equality test remains.
```
def contains(x: Int): Boolean = {
  if (x == Int.MinValue || x == Int.MaxValue) false
  else {
    val n = findPreds(x)(0).nexts(0)
    (n ne tail) && n.datum == x
  }
}
```
In particular, the tail is never reported as a genuine member:

$$
\boxed{x\text{ occurs}\iff\mathrm{preds}(0).\mathrm{nexts}(0)\ne\mathrm{tail}\ \land\ \mathrm{datum}=x.}
$$

The additional work after the [skip list](../../../../../skip-list.md) search is constant.

## ↑ Ancestors (12)

1. [D](../d.md)
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
