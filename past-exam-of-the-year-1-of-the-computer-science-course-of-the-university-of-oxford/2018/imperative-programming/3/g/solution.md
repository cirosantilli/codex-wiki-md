<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use the [sorted sparse dot product](../../../../../sorted-sparse-dot-product.md) merge, processing a coordinate only when it appears in both [supports of a vector](../../../../../support-of-a-vector.md):
```
def dotProduct(vec1: Node, vec2: Node): Double = {
  require(vec1 != null && vec2 != null)
  require(vec1.index == vec2.index)
  var p = vec1.next
  var q = vec2.next
  var result = 0.0
  while ((p ne vec1) && (q ne vec2)) {
    if (p.index < q.index) p = p.next
    else if (q.index < p.index) q = q.next
    else {
      result += p.value * q.value
      p = p.next
      q = q.next
    }
  }
  result
}
```
Both structures must satisfy the [representation invariant](../../../../../representation-invariant.md); equal dimension is checked explicitly. The [loop invariant](../../../../../loop-invariant.md) says that `result` contains exactly the products for all matching indices already passed, and that every skipped unequal index has zero in the other [vector](../../../../../vector.md). The latter follows from sortedness: if `p.index < q.index`, that index cannot appear at `q` or later, and all earlier entries of the other [vector](../../../../../vector.md) have already been settled. Equality contributes its product exactly once. The total number of remaining ordinary entries is a [loop variant](../../../../../loop-variant.md); every iteration advances at least one cursor. Once either cursor reaches its header, all remaining entries pair with zeros. Thus **the exact-arithmetic result is $\sum_i vec1_i vec2_i$**. With $k_1,k_2$ stored entries, [time complexity](../../../../../time-complexity.md) is $O(k_1+k_2+1)$ and [auxiliary space](../../../../../auxiliary-space.md) is constant. Floating-point products and additions may round or overflow even when input coordinates are finite; no exact real-arithmetic accuracy claim is made for `Double`.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
