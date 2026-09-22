<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is [lower-bound search](../../../../../lower-bound-search.md): return the first position whose value is at least the target, allowing the result to equal the [array](../../../../../array-data-structure.md) length. The notation for an empty suffix is vacuously true, so this also covers a target larger than every entry and the empty [array](../../../../../array-data-structure.md). Assume a stable [sorted array](../../../../../sorted-array.md), ordered nondecreasingly.

```
def ternarySearch(a: Array[Int], x: Int): Int = {
  var lo = 0
  var hi = a.length
  while (lo < hi) {
    val third = (hi - lo) / 3
    val m1 = lo + third
    val m2 = hi - 1 - third
    if (a(m1) >= x) hi = m1
    else if (a(m2) < x) lo = m2 + 1
    else {
      lo = m1 + 1
      hi = m2
    }
  }
  lo
}
```

The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq lo\leq hi\leq N,\qquad (\forall k<lo)\ a(k)<x,\qquad (\forall k\geq hi,\ k<N)\ a(k)\geq x.
$$

Initially the excluded prefix and suffix are empty, so both quantified assertions hold. During an iteration, $lo\leq m_1\leq m_2<hi$. If $a(m_1)\geq x$, [sortedness](../../../../../sortedness.md) makes every later value at least $x$, so replacing `hi` by `m1` preserves the right assertion. If the first test failed and $a(m_2)<x$, every earlier value is below $x$, so replacing `lo` by `m2 + 1` preserves the left assertion. Otherwise $a(m_1)<x\leq a(m_2)$; both new exclusions are valid, and `lo = m1 + 1; hi = m2` retains exactly the unresolved middle. In that branch $m_1<m_2$, since a single value cannot satisfy both strict and nonstrict inequalities in opposite directions.

The nonnegative [loop variant](../../../../../loop-variant.md) `hi - lo` strictly decreases. In fact, with old length $d$ and $q=\lfloor d/3\rfloor$, the three possible new lengths are $q,q,d-2q-2$, with the middle branch feasible only when nonnegative; each is at most $\lfloor d/3\rfloor$. At exit `lo == hi`, and the [loop invariant](../../../../../loop-invariant.md) is exactly the desired partition. **The result is the unique lower-bound index, including the first equal entry when duplicates occur.** This [ternary lower-bound search](../../../../../ternary-lower-bound-search.md) uses $O(\log(N+1))$ comparisons and $O(1)$ [auxiliary space](../../../../../auxiliary-space.md), in the [Big O notation](../../../../../big-o-notation.md) word-operation model. The index formulas also avoid computing an overflowing `2 * length`.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
