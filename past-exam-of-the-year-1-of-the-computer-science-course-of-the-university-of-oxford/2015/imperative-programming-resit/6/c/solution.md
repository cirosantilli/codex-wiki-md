<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply capitalization before delegating insertion:
```
trait CapitalisePlugIn extends Doc {
  abstract override def insert(x: Char, pos: Int): Unit = {
    super.insert(x.toUpper, pos)
  }
}
```
[Scala](../../../../../scala.md)'s `Char.toUpper` implements the hinted conversion and leaves ordinary nonletters unchanged. The [stackable trait modification](../../../../../stackable-trait-modification.md) intercepts insertion without changing the position, result type or deletion behavior.

$$
\boxed{\text{The next trait or class receives the capitalized character}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
