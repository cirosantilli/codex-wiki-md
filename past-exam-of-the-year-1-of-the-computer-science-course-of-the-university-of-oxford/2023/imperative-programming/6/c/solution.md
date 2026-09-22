<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [mixin](../../../../../mixin.md) is reusable behavior supplied by a [trait](../../../../../trait.md) and composed into a [class in object-oriented programming](../../../../../class-programming.md). Scala allows only one direct superclass, so [mixins](../../../../../mixin.md) allow several independently reusable capabilities without multiple concrete-class inheritance. A [trait](../../../../../trait.md) can provide implemented methods and require abstract members from its host class.

```
trait Named {
  def name: String
}
trait Greeting extends Named {
  def greeting: String = "Welcome, " + name
}
class Account(val name: String)
class WelcomedAccount(name: String) extends Account(name) with Greeting

val example = new WelcomedAccount("reader")
assert(example.greeting == "Welcome, reader")
```

Here the single superclass supplies `name`, and the [mixin](../../../../../mixin.md) supplies the derived greeting. The same behavior can be mixed into another unrelated host that satisfies `Named`. [Mixin](../../../../../mixin.md) composition uses a defined linearization and requires incompatible concrete member conflicts to be resolved; it does not make arbitrary combinations of concrete superclasses legal.[A class has one superclass and can include several traits](../../../../../class-composition-with-mixins-in-the-scala-documentation.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
