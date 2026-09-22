<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use [sparse dot product by merging indices](../../../../../sparse-dot-product-by-merging-indices.md): only equal coordinate indices can contribute, so merge the two increasing index streams:

```
def dotProduct(vec1: Node, vec2: Node): Double = {
  require(vec1 != null && vec2 != null)
  require(vec1.index == vec2.index, "dimension mismatch")
  var p = vec1.next
  var q = vec2.next
  var answer = 0.0
  while ((p ne vec1) && (q ne vec2)) {
    if (p.index < q.index) p = p.next
    else if (q.index < p.index) q = q.next
    else {
      answer += p.value * q.value
      p = p.next
      q = q.next
    }
  }
  answer
}
```

The [loop invariant](../../../../../loop-invariant.md) states that the accumulator contains all common-coordinate products already passed, while no unprocessed smaller coordinate can acquire a future partner. If one current index is smaller, the other list has no remaining entry at that index, so its product is zero. Equal indices add their product and advance both. Once either list ends, all remaining coordinates of the other have zero partners.

Thus the code computes the [dot product](../../../../../dot-product.md) in coordinate order, subject to [floating-point rounding](../../../../../floating-point-rounding.md), using **$O(k_1+k_2)$ time and constant auxiliary storage**. It does not scan implicit zeros or alter either vector, and it also handles both arguments referring to the same header.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [4](../../4.md)
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
