<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define an [implicit conversion](../../../../../implicit-conversion.md) in the scope where client code uses the added methods:
```
import scala.language.implicitConversions

implicit def stringToDist(s: String): DistFromString =
  new DistFromString(s)
```
Then, for example,
```
val support = "Scala".getDom
val p = "Scala".getProb('a')
```
The [Scala](../../../../../scala.md) [compiler](../../../../../compiler.md) can convert the receiver to `DistFromString` when the requested member is absent from `String`. The conversion must be imported or otherwise visible, and constructing the [finite probability distribution](../../../../../finite-probability-distribution.md) retains the nonempty-[string](../../../../../string.md) [precondition](../../../../../precondition.md) of part (b).

$$
\boxed{\texttt{implicit def stringToDist(s: String): DistFromString}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
