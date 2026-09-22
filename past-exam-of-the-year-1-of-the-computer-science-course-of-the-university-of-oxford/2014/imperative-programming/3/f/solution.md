<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Identify the first matching node at level zero, then bypass **that node** wherever it appears. Comparing keys alone at higher levels could accidentally remove links to a different occurrence with the same key.
```
def delete(x: Int): Unit = {
  if (x != Int.MinValue && x != Int.MaxValue) {
    val preds = findPreds(x)
    val victim = preds(0).nexts(0)
    if ((victim ne tail) && victim.datum == x) {
      for (level <- 0 until NumLevels) {
        if (preds(level).nexts(level) eq victim) {
          preds(level).nexts(level) = victim.nexts(level)
        }
      }
    }
  }
}
```
Because higher-level chains are subsequences of level zero, the predecessor found for any level containing `victim` points directly to it: no earlier equal-valued node can intervene before the first level-zero occurrence. Bypassing it preserves the order and nesting of all the [linked lists](../../../../../linked-list.md). Levels lacking it are unchanged. Thus

$$
\boxed{\text{Delete exactly one occurrence of }x\text{ if present; otherwise leave the list unchanged}.}
$$

The additional work is $O(\mathrm{NumLevels})$. With the usual level cap and random heights, updates have the expected logarithmic [time complexity](../../../../../time-complexity.md) associated with a [skip list](../../../../../skip-list.md).

## ↑ Ancestors (12)

1. [F](../f.md)
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
