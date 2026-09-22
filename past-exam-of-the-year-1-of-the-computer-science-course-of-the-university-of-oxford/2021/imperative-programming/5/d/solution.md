<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Find the entry once and check the abstract membership [precondition](../../../../../precondition.md) on that result:

```
def recall(name: String): String = {
  val entry = find(name, table(hash(name)))
  require(entry != null, "name is not in the book")
  entry.number
}
```

The check turns an invalid call into an explicit [precondition](../../../../../precondition.md) failure rather than an accidental null dereference or an invented default number. For a valid call, the unique matching entry contains exactly the mapped value, so **the stored number is returned and the map is unchanged**. Testing membership by calling `isInBook` first would traverse the same bucket twice; retaining the found reference avoids that redundant work.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
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
