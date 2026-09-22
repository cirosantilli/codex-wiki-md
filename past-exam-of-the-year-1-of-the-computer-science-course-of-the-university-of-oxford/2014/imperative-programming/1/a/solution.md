<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maintain a processed prefix split into values below the pivot and values at least the pivot. The remaining suffix has not yet been classified. Here `a` and `N` are the given [array](../../../../../array-data-structure.md) and its length.
```
def partition(l: Int, r: Int, p: Int): Int = {
  require(0 <= l && l <= r && r <= N)
  var k = l
  var j = l
  while (j < r) {
    if (a(j) < p) {
      val t = a(k); a(k) = a(j); a(j) = t
      k += 1
    }
    j += 1
  }
  k
}
```
The [loop invariant](../../../../../loop-invariant.md) is

$$
l\leq k\leq j\leq r,\qquad a[l..k)<p,\qquad a[k..j)\geq p.
$$

In addition, the active segment remains a [permutation](../../../../../permutation.md) of its original contents, and every entry outside it remains unchanged. If `a(j) < p`, swapping it with `a(k)` extends the first region; the displaced entry, when the two positions differ, already belongs in the second region. Otherwise only the second region grows. The [loop variant](../../../../../loop-variant.md) is $r-j$. At termination $j=r$, so

$$
\boxed{a[l..k)<p\leq a[k..r),\qquad\text{return }k.}
$$

There are exactly $r-l$ iterations, giving $O(r-l+1)$ [time complexity](../../../../../time-complexity.md) and constant [auxiliary space](../../../../../auxiliary-space.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
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
