<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Search for the predecessor of the matching [linked list node](../../../../../linked-list-node.md), or for the last [linked list node](../../../../../linked-list-node.md) if there is no match. This helper makes deletion uniform:
```
class LinkedBook extends Book {
  private val header = new Node("", "", null)

  // Pre: name != null.
  // Post: result is header or a real node.
  // All real nodes through result have names different from name.
  // result.next is null or has name equal to name.
  // No state is changed.
  private def findPrev(name: String): Node = {
    require(name != null)
    var p = header
    while (p.next != null && p.next.name != name) {
      p = p.next
    }
    p
  }

  def store(name: String, number: String): Unit = {
    require(name != null && number != null)
    val p = findPrev(name)
    if (p.next == null)
      p.next = new Node(name, number, null)
    else
      p.next.number = number
  }

  def recall(name: String): String = {
    require(name != null)
    val p = findPrev(name)
    require(p.next != null, "Name is not in the book")
    p.next.number
  }

  def isInBook(name: String): Boolean = {
    require(name != null)
    findPrev(name).next != null
  }

  def delete(name: String): Boolean = {
    require(name != null)
    val p = findPrev(name)
    if (p.next == null) false
    else {
      p.next = p.next.next
      true
    }
  }
}
```
The search [loop invariant](../../../../../loop-invariant.md) says that `p` is the header or a reachable real [linked list node](../../../../../linked-list-node.md), and every real [linked list node](../../../../../linked-list-node.md) from the start through `p` has a name different from the requested name. The [linked list](../../../../../linked-list.md) has not been changed. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) protects `p.next.name` when the end is reached. The [loop variant](../../../../../loop-variant.md) is the number of real [linked list nodes](../../../../../linked-list-node.md) strictly after `p`; finiteness and acyclicity make it a nonnegative decreasing [integer](../../../../../integer-split.md). Consequently the helper's stated [postcondition](../../../../../postcondition.md) holds.

For `store`, a found name changes only its number; an absent name adds exactly one fresh binding at the end, maintaining uniqueness. For `delete`, unlinking the found [linked list node](../../../../../linked-list-node.md) removes exactly the requested binding; absence returns false without mutation. Both query operations preserve the [abstraction function](../../../../../abstraction-function.md). Non-null [preconditions](../../../../../precondition.md) are checked at entry; **`recall` additionally checks membership using the one completed search**, avoiding a redundant whole-list membership scan. The helper is the only additional operation and its complete behavioral contract is stated above.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
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
