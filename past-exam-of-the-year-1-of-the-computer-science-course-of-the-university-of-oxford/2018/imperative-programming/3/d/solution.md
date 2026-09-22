<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume `vector` already satisfies the full [representation invariant](../../../../../representation-invariant.md) in part (b). Check the local bounds and value [preconditions](../../../../../precondition.md), then find the first index not smaller than the requested one:
```
def setElement(vector: Node, value: Double, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  require(value != 0.0 && !java.lang.Double.isNaN(value) &&
          !java.lang.Double.isInfinite(value))
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) p.value = value
  else {
    val left = p.prev
    val fresh = new Node(value, index, left, p)
    left.next = fresh
    p.prev = fresh
  }
}
```
The search [loop invariant](../../../../../loop-invariant.md) says that the structure is unchanged and every ordinary [linked list node](../../../../../linked-list-node.md) passed has index smaller than `index`; `p` is the next candidate. The number of unpassed ordinary entries is a [loop variant](../../../../../loop-variant.md). The [short-circuit evaluation](../../../../../short-circuit-evaluation.md) prevents testing the header index as an ordinary entry. If an equal index exists, changing only its nonzero value preserves the [representation invariant](../../../../../representation-invariant.md). Otherwise `left` and `p` delimit the unique insertion position: initializing both new links before redirecting their neighbors preserves reciprocal links and strict index order. **Exactly the requested coordinate changes.** With $k$ stored entries, the search costs $O(k+1)$ and the splice costs [constant time](../../../../../constant-time.md); checking the whole input structure is a caller obligation, rather than an unmentioned scan inside each call.

## ↑ Ancestors (12)

1. [D](../d.md)
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
