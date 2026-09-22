<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The history is built by prepending, so reverse it when displaying chronological moves:
```
override def toString: String =
  game.mkString("[", ", ", "]") +
    "    history of flips: " + flips.reverse.toString
```
Thus a reverse-stored history `[3,2,4]` is displayed as **`List(4, 2, 3)`**. The initial empty history remains `List()`. Neither traversal mutates the game or the immutable history. Displaying the stored list without reversing it would describe the moves backwards.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
