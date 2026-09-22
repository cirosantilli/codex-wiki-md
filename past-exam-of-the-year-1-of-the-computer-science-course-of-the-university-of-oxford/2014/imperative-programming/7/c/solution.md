<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Convert lowercase alphabet letters before passing them to the next implementation. Already uppercase letters and other characters pass through unchanged.
```
trait CapitalisePlugIn extends Doc {
  abstract override def insert(x: Char, pos: Int): Unit = {
    val y = if ('a' <= x && x <= 'z') ('A' + (x - 'a')).toChar else x
    super.insert(y, pos)
  }
}
```
The character conversion uses the paper's contiguous lowercase and uppercase Latin ranges. Thus

$$
\boxed{\texttt{insert('a',pos)}\text{ delegates as }\texttt{insert('A',pos)}.}
$$

Deletion, reading, and size need no overrides.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
