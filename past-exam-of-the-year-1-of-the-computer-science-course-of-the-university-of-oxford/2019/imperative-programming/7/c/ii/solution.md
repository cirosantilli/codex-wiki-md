<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

One base-class implementation changes the private fields directly:
```
def flip(): Unit = {
  val oldH = _h
  _h = _w
  _w = oldH
}
```
The completed operation leaves the area unchanged. It calls no overriding setters, so the logging subclass's count stays unchanged and **does not need an override**. The invariant is about completed public updates, not transient internal states between the two assignments.

A second implementation uses public setters:
```
def flip(): Unit = {
  val oldH = height
  val oldW = width
  height = oldW
  width = oldH
}
```
These setter calls use [dynamic dispatch](../../../../../../dynamic-dispatch.md) on a logging receiver. Starting at height two and width three, the first call increases the temporary area from six to nine and wrongly increments the count, while the final area returns to six. **This version needs a subclass override**. With the counter name from part (i), the following override discards the internal setter contributions:
```
override def flip(): Unit = {
  val before = increases
  super.flip()
  increases = before
}
```
For this specified base implementation the two assignments complete normally and the final area equals the initial area, so restoring the saved count is correct. Another design could suppress logging during the compound operation. The difference between the two base implementations illustrates the [fragile base class problem](../../../../../../fragile-base-class-problem.md): an internal refactoring can change subclass behavior through newly introduced virtual calls.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
