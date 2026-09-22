<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add a generic mapping method inside the supplied trait. Snapshot the finitely many source masses, and sum masses when different entries have the same image:
```
def map[U](f: T => U): FiniteDist[U] = {
  val entries = getDom.map(x => (f(x), getProb(x)))
  val support = entries.map(_._1).distinct

  new FiniteDist[U] {
    def getDom: List[U] = support
    def getProb(y: U): Double =
      entries.foldLeft(0.0) { case (sum, (image, mass)) =>
        if (image == y) sum + mass else sum
      }
  }
}
```
Here the mapping is a mathematical [function](../../../../../function-split.md), and keys are assumed to have stable equality consistent with their intended identity. Each source atom is evaluated once when the new distribution is constructed. The distinct image [list](../../../../../list-abstract-data-type.md) is exactly the finite support because all listed source atoms have positive mass. Summing collisions, rather than overwriting a previous mass, implements the [probability](../../../../../probability.md) pushforward.

The sets of source atoms with a fixed image partition the original support. Hence nonnegativity is preserved and, in exact [probability](../../../../../probability.md) arithmetic,

$$
\sum_y p_2(y)=\sum_y\sum_{x:f(x)=y}p_1(x)=\sum_xp_1(x)=1.
$$

Thus the result is a [finite probability distribution](../../../../../finite-probability-distribution.md). For a constant mapping, every atom merges into one outcome of mass one. Floating-point [additions](../../../../../addition.md) in the implementation can introduce rounding error, so numerical tests of normalization should use a suitable tolerance rather than demand exact equality of `Double` sums.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
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
