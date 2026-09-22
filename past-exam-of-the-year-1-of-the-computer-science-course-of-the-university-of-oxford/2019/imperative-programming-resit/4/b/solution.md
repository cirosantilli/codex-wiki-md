<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Store the bottom of the [stack](../../../../../stack-data-structure.md) at index zero and the top at the last occupied index:
```
class Stack {
  private val MAX = 1000
  private val data = new Array[Tree](MAX)
  private var used = 0

  // Pre: used < MAX.
  def push(t: Tree): Unit = {
    require(used < MAX, "Stack full")
    data(used) = t
    used += 1
  }

  // Pre: used > 0.
  def pop: Tree = {
    require(used > 0, "Stack empty")
    used -= 1
    val result = data(used)
    data(used) = null
    result
  }

  // Pre: true.
  def isEmpty: Boolean = used == 0
}
```
The [representation invariant](../../../../../representation-invariant.md) is that `data.length==MAX`, $0\leq used\leq MAX$, and unused slots from `used` onwards contain null references. Occupied slots contain the stored `Tree` references; the [stack](../../../../../stack-data-structure.md) itself need not forbid null values. The [abstraction function](../../../../../abstraction-function.md), written with the first [sequence](../../../../../sequence.md) element at the top, is

$$
\alpha(data,used)=[data(used-1),data(used-2),\ldots,data(0)].
$$

Initially this is the empty [sequence](../../../../../sequence.md). `push` prepends its argument, `pop` removes and returns the first abstract element, and `isEmpty` reports whether the abstract [sequence](../../../../../sequence.md) is empty. These [postconditions](../../../../../postcondition.md) follow directly from the index changes. Clearing a popped slot avoids retaining an otherwise unused [tree](../../../../../tree-graph-theory-split.md) reference. All three operations take **$O(1)$ time**. No loops are needed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
