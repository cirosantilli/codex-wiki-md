<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maintain the required boundary between entries strictly above the target and entries at most the target:
```
def search(u: Array[Int], z: Int): Boolean = {
  var a = 0
  var b = u.length
  while (a < b) {
    val middle = a + (b - a) / 2
    if (u(middle) > z) a = middle + 1
    else b = middle
  }
  a < u.length && u(a) == z
}
```
The full [invariant](../../../../../invariant-mathematics.md) is $0\leq a\leq b\leq n$, every entry before $a$ is greater than $z$, and every entry at or after $b$ is at most $z$. The [array](../../../../../array-data-structure.md) remains unchanged. Descending order justifies each update: if the middle value is greater, all earlier values are greater too; otherwise all values from the middle onward are at most the target.

The nonnegative [loop variant](../../../../../loop-variant.md) $b-a$ strictly decreases, with each update retaining at most half the old candidate length. On termination $a=b$, which is the first index whose value could be at most $z$. Equality at that index is therefore necessary and sufficient for presence. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) makes the final test safe when $a=n$, including the empty-[array](../../../../../array-data-structure.md) case. The time is **$O(\log(n+1))$**, using constant [auxiliary space](../../../../../auxiliary-space.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
