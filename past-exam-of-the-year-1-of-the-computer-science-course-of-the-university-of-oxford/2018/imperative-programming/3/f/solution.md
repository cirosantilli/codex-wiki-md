<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Append entries in increasing index order, keeping a tail reference so that repeated searches do not make construction quadratic:
```
def makeVector(elems: Array[Double]): Node = {
  require(elems != null)
  val h = makeZeroVector(elems.length)
  var tail = h
  var i = 0
  while (i < elems.length) {
    val v = elems(i)
    require(!java.lang.Double.isNaN(v) &&
            !java.lang.Double.isInfinite(v))
    if (v != 0.0) {
      val fresh = new Node(v, i, tail, h)
      tail.next = fresh
      h.prev = fresh
      tail = fresh
    }
    i += 1
  }
  h
}
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq elems.length$, a valid circular representation of the nonzero entries in `elems[0..i)`, a fixed header dimension `elems.length`, and `tail eq h.prev`. The next nonzero index is greater than every stored index; appending the fresh [linked list node](../../../../../linked-list-node.md) preserves reciprocal links, including `tail.next eq h`. The [loop variant](../../../../../loop-variant.md) is `elems.length-i`. At exit **the [abstraction function](../../../../../abstraction-function.md) yields exactly the input [array](../../../../../array-data-structure.md) as a [vector](../../../../../vector.md)**. There is one pass and constant work per entry: $\Theta(n)$ [time complexity](../../../../../time-complexity.md) for $n>0$, $O(n+1)$ including emptiness, and $O(k+1)$ output storage for $k$ nonzero entries. Both signs of floating-point zero are represented by absence.

## ↑ Ancestors (12)

1. [F](../f.md)
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
