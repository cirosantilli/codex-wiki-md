<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compare every unordered pair of distinct starting positions:

```
def longestRepeated(): (Int, Int, Int) = {
  require(N >= 2)
  var besti = 0
  var bestj = 1
  var bestk = 0
  var i = 0
  while (i < N - 1) {
    var j = i + 1
    while (j < N) {
      val k = longestFrom(i, j)
      if (k > bestk) {
        besti = i; bestj = j; bestk = k
      }
      j += 1
    }
    i += 1
  }
  (besti, bestj, bestk)
}
```

After each comparison, the stored triple attains the largest common-prefix length among pairs processed so far; its positions remain distinct. The nested [while loops](../../../../../while-loop.md) enumerate exactly $N(N-1)/2$ pairs. Reversing the two positions does not change their common-prefix length, so no omitted ordered pair could improve the answer. Initialization also supplies a valid length-zero answer if no character repeats.

Write $K$ for the final maximal length. Each comparison takes $O(K+1)$ time, including a possible first mismatch. Hence **time is $O(N^2(K+1))$, at worst $O(N^3)$**, and auxiliary space is $O(1)$. Writing merely $O(N^2K)$ would miss the $K=0$ case. The explicit [precondition](../../../../../precondition.md) excludes [arrays](../../../../../array-data-structure.md) with fewer than two valid starting positions; the requested distinct-position triple has no answer there under this domain convention.

## ↑ Ancestors (12)

1. [B](../b.md)
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
