<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**A [function](../../../../../../function-split.md) accepting every `Base` can safely be used where only `Derived` inputs will be supplied. The reverse direction is unsafe.** A `Derived` argument is already a valid `Base` argument; restricting the possible callers introduces no new obligation for the [function](../../../../../../function-split.md). This is the contravariant input rule of [function](../../../../../../function-split.md) [subtyping](../../../../../../subtyping.md).

The printed [trait](../../../../../../trait.md) has [generic type invariance](../../../../../../generic-type-invariance.md), so [Scala](../../../../../../scala.md) does not directly permit either parameter-changing assignment. The safe behavior can be exposed using an explicit adapter without changing that [trait](../../../../../../trait.md):

```
def restrictInput(f: Fun[Base, Base]): Fun[Derived, Base] =
  new Fun[Derived, Base] {
    def apply(x: Derived): Base = f(x)
  }
```

For the unsafe direction, take illustrative classes in which a derived [software object](../../../../../../software-object.md) has an extra operation:

```
class Base
class Derived extends Base { def special(): Int = 1 }
val narrow = new Fun[Derived, Base] {
  def apply(x: Derived): Base = { x.special(); x }
}
def broadClient(f: Fun[Base, Base]): Base = f(new Base)
// broadClient(narrow) must be rejected.
```

If that substitution were accepted, the client could pass an ordinary base [software object](../../../../../../software-object.md) to code that calls `special`, which that [software object](../../../../../../software-object.md) does not support. The rejected call is intentional counterexample code, not a promised compilable application. Variance annotations are needed to make sound direct conversions part of the generic [trait](../../../../../../trait.md)'s declared [subtyping](../../../../../../subtyping.md) relation.[Variance Annotations: missing annotation is invariant; method-input positions reverse variance](../../../../../../scala-2-13-variance-annotations-specification.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
