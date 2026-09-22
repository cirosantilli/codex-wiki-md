<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The missing [preconditions](../../../../../../precondition.md) are **$0\leq pos\leq|d|$ for insertion** and **$0\leq pos<|d|$ for deletion and indexing**. The inclusive endpoint permits appending; deletion or access at the length is invalid. Specify the initial state, for example $d=[]$, as well as the read-only [frame conditions](../../../../../../frame-condition.md): indexing returns the indicated character and preserves $d$, while `length` returns $|d|$ and preserves $d$.

The insertion and deletion clauses already describe the new [sequence](../../../../../../sequence.md), but their returned values and effects should be interpreted against the old state. For a machine-sized length, insertion also requires $|d|<Int.MaxValue$. These clauses complete the document [abstract data type](../../../../../../abstract-data-type.md) without prescribing one storage representation.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
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
