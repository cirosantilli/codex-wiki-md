<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reuse the machinery with the digit interval:

```
trait DigitCountPlugIn extends CharCountPlugin {
  override protected def firstCounted: Char = '0'
  override protected def numberCounted: Int = 10
}
```

Its `count` [precondition](../../../../../../precondition.md) is now **`'0' <= ch && ch <= '9'`**. It counts digits while permitting all characters to be stored. This is an alternative configured counter, rather than a second independent lowercase counter in the same object; simultaneous independent alphabets would require separate counters or a combined mapping.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
