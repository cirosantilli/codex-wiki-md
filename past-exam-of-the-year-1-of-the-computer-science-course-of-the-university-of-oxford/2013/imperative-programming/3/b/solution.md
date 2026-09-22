<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [three-way quicksort](../../../../../three-way-quicksort.md). Fix the pivot value before moving any entries, and group equal entries together so that none needs a recursive call. These helpers and the sorter belong inside an enclosing scope containing `a`.
```
def swap(i: Int, j: Int): Unit = {
  val t = a(i); a(i) = a(j); a(j) = t
}

def split(l: Int, r: Int): (Int, Int) = {
  // Pre: 0 <= l < r <= a.length.
  val p = a(l)
  var lt = l
  var i = l
  var gt = r
  while (i < gt) {
    if (a(i) < p) {
      swap(lt, i)
      lt += 1
      i += 1
    } else if (a(i) > p) {
      gt -= 1
      swap(i, gt)
    } else {
      i += 1
    }
  }
  (lt, gt)
}

def quicksort(l: Int, r: Int): Unit = {
  require(0 <= l && l <= r && r <= a.length)
  if (r - l > 1) {
    val (lt, gt) = split(l, r)
    quicksort(l, lt)
    quicksort(gt, r)
  }
}

// Sort the whole array with quicksort(0, a.length).
```
The [array partitioning](../../../../../two-way-array-partition.md) [loop invariant](../../../../../loop-invariant.md) is

$$
l\leq lt\leq i\leq gt\leq r,\qquad
a[l..lt)<p,\quad a[lt..i)=p,\quad a[gt..r)>p,
$$

with $a[i..gt)$ unclassified. Swaps preserve the segment's [array multiset](../../../../../array-multiset.md) and leave all entries outside it unchanged. The [loop variant](../../../../../loop-variant.md) $gt-i$ decreases in every branch. When swapping an entry from the right into `i`, do not increment `i`, since the incoming entry still needs classification. At termination,

$$
\boxed{a[l..lt)<p=a[lt..gt)<a[gt..r).}
$$

Here the middle segment is nonempty because the original pivot occurs somewhere in the preserved [array multiset](../../../../../array-multiset.md). Both recursive segments therefore have length strictly smaller than $r-l$. [Mathematical induction](../../../../../mathematical-induction.md) on segment length proves that the two recursive calls sort their segments, and their ordering relative to the middle segment proves the complete [sorting](../../../../../sorting.md) [postcondition](../../../../../postcondition.md).

There is no additional [array](../../../../../array-data-structure.md). The call stack and returned boundary pairs still use [auxiliary space](../../../../../auxiliary-space.md). An all-equal input takes one linear scan and no nontrivial recursive calls, so its [time complexity](../../../../../time-complexity.md) is $\Theta(N)$ for $N\geq1$. Balanced partitions give $O(N\log N)$ [time complexity](../../../../../time-complexity.md); a fixed first pivot can still give $O(N^2)$ on adversarial distinct inputs. The worst-case call stack has $O(N)$ entries.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
