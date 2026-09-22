<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Place these methods inside the `LLBuffer` class. The two private insertion methods operate on physical endpoints; the public methods interpret logical endpoints using the reversal flag.
```
private def addFirst(x: Int): Unit = {
  val q = new Node(x)
  q.next = first
  if (first == null) last = q else first.prev = q
  first = q
  size += 1
}

private def addLast(x: Int): Unit = {
  val q = new Node(x)
  q.prev = last
  if (last == null) first = q else last.next = q
  last = q
  size += 1
}

def append(x: Int): Unit = {
  if (backwards) addFirst(x) else addLast(x)
}

def prepend(x: Int): Unit = {
  if (backwards) addLast(x) else addFirst(x)
}

def get(i: Int): Int = {
  require(0 <= i && i < size)
  val j = if (backwards) size - 1 - i else i
  var q: Node = null
  if (j <= size - 1 - j) {
    q = first
    var k = 0
    while (k < j) { q = q.next; k += 1 }
  } else {
    q = last
    var k = size - 1
    while (k > j) { q = q.prev; k -= 1 }
  }
  val x = q.value
  if (q.prev == null) first = q.next else q.prev.next = q.next
  if (q.next == null) last = q.prev else q.next.prev = q.prev
  q.prev = null
  q.next = null
  size -= 1
  x
}

def rev: Unit = { backwards = !backwards }
```
In the forward traversal, the [loop invariant](../../../../../../loop-invariant.md) is that `q` is physical node $k$, with $0\leq k\leq j$; its [loop variant](../../../../../../loop-variant.md) is $j-k$. In the backward traversal, `q` is physical node $k$, with $j\leq k<size$; its [loop variant](../../../../../../loop-variant.md) is $k-j$. Thus both locate physical index $j$, which is exactly logical index $i$ under the [abstraction function](../../../../../../abstraction-function.md).

Deletion bypasses the chosen [linked list node](../../../../../../linked-list-node.md) in both directions. Deleting the first or last [linked list node](../../../../../../linked-list-node.md) updates the corresponding endpoint; deleting the only [linked list node](../../../../../../linked-list-node.md) sets both endpoints to null. The surviving values keep their physical relative order, so the [abstraction function](../../../../../../abstraction-function.md) gives precisely the required logical deletion. Each insertion preserves reciprocal links and adds its value at the physical end corresponding to the required logical end. Toggling the flag changes $s$ to its [list reversal](../../../../../../list-reversal.md) without moving any [linked list nodes](../../../../../../linked-list-node.md). Consequently

$$
\boxed{append,prepend,rev:O(1),\qquad get(i):O(1+\min(i,size_0-1-i)).}
$$

These are worst-case [time complexity](../../../../../../time-complexity.md) bounds in the constant-cost pointer model; total storage is $O(size)$ and each operation uses constant [auxiliary space](../../../../../../auxiliary-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
