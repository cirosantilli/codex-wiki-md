<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The proposed condition is not a [loop invariant](../../../../../loop-invariant.md) at the loop head.** It holds initially and on entry to every executed body, but the iteration starting with `i == 10` finishes with `i == 11`. Control then returns to the condition with the proposed upper bound false. A suitable numerical [loop invariant](../../../../../loop-invariant.md) is **$1\leq i\leq11$**. If the number of printed lines matters, strengthen it to “exactly $i-1$ lines have been printed.” At exit, this and `i > 10` give exactly ten printed lines. The nonnegative [loop variant](../../../../../loop-variant.md) $11-i$ decreases by one on every iteration.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
