<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set aside the selected pivot at the end, [array partitioning](../../../../../two-way-array-partition.md) the other entries, then move the pivot to the separation index:
```
def partition(l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  def swap(i: Int, j: Int): Unit = {
    val t = a(i); a(i) = a(j); a(j) = t
  }
  val chosen = bestIndex(l, r)
  val x = a(chosen)
  swap(chosen, r - 1)
  var p = l
  var j = l
  while (j < r - 1) {
    if (a(j) < x) {
      swap(p, j)
      p += 1
    }
    j += 1
  }
  swap(p, r - 1)
  p
}
```
The [loop invariant](../../../../../loop-invariant.md) is $l\leq p\leq j\leq r-1$, $a[l,p)<x$, $a[p,j)\geq x$, and $a(r-1)=x$. The segment's [multiset](../../../../../multiset.md) is unchanged and all entries outside it are unchanged. A low entry is swapped into the low segment; a high entry simply extends the high segment. The [loop variant](../../../../../loop-variant.md) is $r-1-j$. At exit, exchanging the reserved pivot with `a(p)` gives **$a[l,p)<x$, $a(p)=x$, and $a[p+1,r)\geq x$**. The displaced value at the old pivot position was already at least $x$. Length one is handled by self-swaps and an empty loop. Duplicate pivot values belong to the high side. This costs $\Theta(r-l)$ time and $O(1)$ auxiliary space.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
