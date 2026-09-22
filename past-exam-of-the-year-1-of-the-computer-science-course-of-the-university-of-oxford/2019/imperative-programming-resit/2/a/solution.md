<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let `a` be the given enclosing [array](../../../../../array-data-structure.md). A [two-way array partition](../../../../../two-way-array-partition.md) needs only one scan, and does not require the pivot to occur in the [array](../../../../../array-data-structure.md):
```
def partition(l: Int, r: Int, p: Int): Int = {
  require(0 <= l && l <= r && r <= a.length)
  var k = l
  var j = l
  while (j < r) {
    if (a(j) < p) {
      val t = a(k)
      a(k) = a(j)
      a(j) = t
      k += 1
    }
    j += 1
  }
  k
}
```
The [loop invariant](../../../../../loop-invariant.md) is $l\leq k\leq j\leq r$, every entry of $a[l,k)$ is less than $p$, every entry of $a[k,j)$ is at least $p$, and the segment's [multiset](../../../../../multiset.md) is unchanged. Entries outside $[l,r)$ are unchanged. When `a(j)<p`, swapping it into position `k` extends the low part; if `k<j`, the displaced entry was in the high part and remains there after `j` advances. If `k==j`, the self-swap is harmless. The other branch simply extends the high part. The [loop variant](../../../../../loop-variant.md) is $r-j$. At exit $j=r$, so **the returned $k$ has the required separation property**, including empty segments and arbitrarily many duplicate entries. The [time complexity](../../../../../time-complexity.md) is $\Theta(r-l+1)$ and auxiliary [space complexity](../../../../../space-complexity.md) is $O(1)$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
