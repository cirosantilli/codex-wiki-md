<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a proposed [loop invariant](../../../../../loop-invariant.md) $I$, initial condition $P$, guard $B$, body $S$, and [postcondition](../../../../../postcondition.md) $Q$, establish these [Hoare logic](../../../../../hoare-logic.md) obligations:

$$
P\Rightarrow I,\qquad \{I\land B\}\ S\ \{I\},\qquad
I\land\neg B\Rightarrow Q.
$$

The first establishes $I$ before the loop; the second preserves it after each iteration; the third derives the desired result when the guard is false. Together they prove **[partial correctness](../../../../../partial-correctness.md)**. For **[total correctness](../../../../../total-correctness.md)**, also prove [algorithm termination](../../../../../algorithm-termination.md), for example by a nonnegative [integer](../../../../../integer-split.md) [loop variant](../../../../../loop-variant.md) that strictly decreases whenever the body executes. The [loop invariant](../../../../../loop-invariant.md) need not be the [postcondition](../../../../../postcondition.md): it generally describes completed and unfinished work together.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
