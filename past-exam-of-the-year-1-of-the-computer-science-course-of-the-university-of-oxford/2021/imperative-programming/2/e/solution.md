<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Sort [string suffix](../../../../../string-suffix.md) starting positions, then examine only adjacent entries:

```
def longestRepeated(): (Int, Int, Int) = {
  require(N >= 2)
  val suffixes = (0 until N).toArray.sortWith(before)
  var besti = suffixes(0)
  var bestj = suffixes(1)
  var bestk = 0
  var t = 1
  while (t < N) {
    val i = suffixes(t - 1)
    val j = suffixes(t)
    val k = longestFrom(i, j)
    if (k > bestk) {
      besti = i; bestj = j; bestk = k
    }
    t += 1
  }
  (besti, bestj, bestk)
}
```

The [while loop](../../../../../while-loop.md) retains a best triple among adjacent pairs already visited. All [string suffix](../../../../../string-suffix.md) starting positions are distinct, and the adjacent-suffix characterization proves that considering these $N-1$ pairs suffices. The two definitions named `longestRepeated` in parts b and e are alternatives, not duplicate members of one [software class](../../../../../class-programming.md).

Assuming a comparison sort using $O(N\log N)$ comparator calls, sorting takes $O(N\log N(K+1))$ time, because each comparison scans characters. The final pass takes $O(N(K+1))$. Thus **overall time is $O(N\log N(K+1))$, at worst $O(N^2\log N)$**, with $O(N)$ auxiliary storage for indices and ordinary sorting workspace. Merely storing indices does not make [string suffix](../../../../../string-suffix.md) comparisons constant-time; claiming $O(N\log N)$ here would omit their cost. Faster suffix-array constructions require additional machinery beyond this comparator-based solution.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
