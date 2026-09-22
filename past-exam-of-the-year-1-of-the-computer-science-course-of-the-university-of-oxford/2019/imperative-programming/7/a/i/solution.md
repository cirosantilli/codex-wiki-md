<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Encapsulation](../../../../../../encapsulation-computer-programming.md) exposes operations with contracts while hiding representation details and controlling changes to state. In a text editor, a document object can privately store text and cursor position and expose `insert`, `delete` and `moveCursor`. Clients cannot directly splice internal storage or set a cursor outside the document. **The document's methods enforce its [representation invariant](../../../../../../representation-invariant.md)**, and the implementation can later replace a character [array](../../../../../../array-data-structure.md) by a different text representation without changing the public editing interface. Merely declaring a field private is insufficient if an accessor returns the mutable representation itself.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
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
