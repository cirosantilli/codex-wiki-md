<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[First-come-first-served disk scheduling](../../../../../../first-come-first-served-disk-scheduling.md) follows the arrival order:
```
133 -> 76 -> 157 -> 91 -> 142 -> 97 -> 135 -> 112 -> 23
```
The total [seek distance](../../../../../../seek-distance.md) is

$$
\boxed{57+81+66+51+45+38+23+89=450\text{ tracks}.}
$$

The initial position is 133; the earlier completed request at 135 is used to determine direction for the elevator policy, not added again to this total.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
