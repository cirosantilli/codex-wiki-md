<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Maintain the reciprocal [factorial](../../../../../factorial.md) term rather than calculating large [factorials](../../../../../factorial.md) separately:

```
def eb(n: Int): Double = {
  require(n > 0)
  var i = 0
  var term = 1.0
  var sum = 1.0
  while (i < n) {
    i += 1
    term /= i.toDouble
    sum += term
  }
  sum
}
```

The exact-arithmetic [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq n$, $term=1/i!$, and $sum=\sum_{k=0}^{i}1/k!$. It holds for $i=0$ because $0!=1$. Dividing by the new index produces the next reciprocal [factorial](../../../../../factorial.md); adding it extends the partial sum. The [loop variant](../../../../../loop-variant.md) is $n-i$. At exit the sum includes **all terms from $0$ through $n$**, using exactly $n$ divisions and no multiplications in the loop. In particular, the initial `1.0` accounts for the zero-index term. The work bound is $O(n)$, with constant [auxiliary space](../../../../../auxiliary-space.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
