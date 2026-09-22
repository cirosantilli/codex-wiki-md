<h1 id="8/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Constructing channel implementations, decorators and adapters allocates [software objects](../../../../../../software-object.md) that hold state and references to other [software objects](../../../../../../software-object.md). As configurations and temporary processing chains are replaced, some old [software objects](../../../../../../software-object.md) become unreachable. A typical [Scala](../../../../../../scala.md) program on a managed runtime relies on [garbage collection](../../../../../../garbage-collection.md) to recycle that storage; otherwise unreclaimed allocation can exhaust the available [heap memory](../../../../../../heap-memory.md).

**A reachable wrapper keeps its wrapped component reachable.** Sharing a channel among several wrappers can extend its lifetime until all relevant references disappear. Many [software objects](../../../../../../software-object.md) alone do not imply that collection can free them: if the program deliberately retains every channel, those [software objects](../../../../../../software-object.md) remain live. The reason [garbage collection](../../../../../../garbage-collection.md) is useful is repeated allocation combined with changing reachability, not an assumption that the integer-returning `apply` operation allocates a fresh channel on every call.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [8](../../../8.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
