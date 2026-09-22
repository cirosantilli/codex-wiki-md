<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Protected access](../../../../../protected-access.md) makes `size` available to subclasses implementing the set operations, while preventing ordinary outside clients from assigning arbitrary values to it. The implementations need to update the count when membership changes; clients should affect membership only through the public operations. A publicly writable count could make an emptiness query disagree with the stored elements.

**Protection supports [encapsulation](../../../../../encapsulation-computer-programming.md) but does not prove the [representation invariant](../../../../../representation-invariant.md).** Subclasses can still update the field incorrectly and must maintain its relationship to the actual set [cardinality](../../../../../cardinality.md). In particular, subclass code does not obtain unrestricted access to the protected field of every unrelated set [software object](../../../../../software-object.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
