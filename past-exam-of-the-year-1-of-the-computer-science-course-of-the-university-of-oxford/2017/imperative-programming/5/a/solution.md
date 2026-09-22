<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [prototype pattern](../../../../../prototype-pattern.md) is a [creational pattern](../../../../../creational-pattern.md): a client asks a configured object to clone itself through a common [object interface](../../../../../object-interface.md), and concrete prototypes implement the cloning operation. The client can thereby create objects without naming their concrete classes at every creation site.

Use it when the required configuration or concrete type is chosen at runtime, or when reconstructing expensive initial state is less convenient than copying a prepared example. A [deep copy](../../../../../deep-copy.md) may be needed for independently mutable nested data; merely duplicating outer fields can leave [reference aliasing](../../../../../reference-aliasing.md). The cloning contract determines what is copied and what may safely be shared.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
