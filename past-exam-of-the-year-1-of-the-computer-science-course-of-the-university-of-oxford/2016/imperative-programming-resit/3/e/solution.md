<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**A directly self-recursive procedure can be replaced by a simple loop when every recursive call is a [tail call](../../../../../tail-call.md).** This is [tail recursion](../../../../../tail-recursion.md): no operation, including an update or cleanup action, remains to be performed after the call returns. The loop tests the same cases, performs the same nonrecursive work, and replaces the current parameters by the next call's arguments. Argument values must be computed before assignments if their expressions depend on old parameter values; by-reference bindings also need preserving.

A traversal that must return to explore another child is not in this form. It can still be implemented iteratively with an explicit [stack](../../../../../stack-data-structure.md), but that is a different transformation and generally retains the deferred work.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
