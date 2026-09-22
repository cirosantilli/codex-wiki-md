<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Scan the two suffixes until a mismatch or an endpoint:

```
def longestFrom(i: Int, j: Int): Int = {
  require(0 <= i && i <= N && 0 <= j && j <= N)
  var k = 0
  while (k < N - i && k < N - j && a(i + k) == a(j + k)) {
    k += 1
  }
  k
}
```

The [loop invariant](../../../../../loop-invariant.md) is $0\leq k\leq\min(N-i,N-j)$ and equality of the two [array](../../../../../array-data-structure.md) segments of length $k$. The [loop variant](../../../../../loop-variant.md) is $\min(N-i,N-j)-k$, which decreases whenever the [while loop](../../../../../while-loop.md) runs. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) checks both bounds before indexing. On exit either a [string suffix](../../../../../string-suffix.md) has ended or the next characters differ, so no longer common [string prefix](../../../../../string-prefix.md) is possible. Thus **the returned value is the [longest common prefix](../../../../../longest-common-prefix.md) length**. Overlap is allowed: the code only reads the [array](../../../../../array-data-structure.md), so the two matching segments need not occupy disjoint storage.

## ↑ Ancestors (12)

1. [A](../a.md)
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
